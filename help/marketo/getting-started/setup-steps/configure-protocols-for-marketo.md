---
unique-page-id: 4720433
description: Protokolle für Marketing - Marketing - Docs - Produktdokumentation konfigurieren
title: Protokolle für Marketing konfigurieren
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 1%

---


# Protokolle für Marketing konfigurieren {#configure-protocols-for-marketo}

Ihre Marketinggruppe verwendet Marketo, um Landingpages und E-Mails zu Kampagnen zu erstellen. Um sicherzustellen, dass diese Landingpages und E-Mails funktionieren, benötigen sie eine kleine Hilfe von der IT. Bitte richten Sie die folgenden Protokolle mit den Informationen ein, die Ihnen Ihre Marketinggruppe per E-Mail zukommen lassen sollte.

>[!NOTE]
>
>Dieser Artikel ist für die IT-Abteilung der Firma gedacht, die diese Protokolle implementieren möchte.

## Schritt 1: DNS-Datensätze für Landingpages und E-Mail erstellen {#step-create-dns-records-for-landing-pages-and-email}

**Tracking-Link-CNAMEs**

Ihr Marketing-Team sollte Ihnen zwei Anfragen nach neuen CNAME-Aufzeichnungen senden. Die erste ist für Landingpages-URLs gedacht, sodass die Landingpages in URLs angezeigt werden, die Ihre Domäne und nicht Marketo (der eigentliche Host) widerspiegeln. Der zweite betrifft die Links zur Verfolgung, die in den E-Mails enthalten sind, die sie von Marketing senden.

1 - **Hinzufügen CNAME für Landingpages**

hinzufügen der Landingpage CNAME, die Sie an Ihren DNS-Datensatz gesendet haben, sodass `[YourLandingPageCNAME]` auf die eindeutige Kontozeichenfolge verweist, die Ihren Marketo-Landingpages zugewiesen ist. Melden Sie sich bei der Site Ihrer Domänenregistrierungsstelle an und geben Sie den CNAME und die Kontozeichenfolge der Landingpage ein. Normalerweise umfasst dies drei Felder:

・ Alias: Geben Sie `[YourLandingPageCNAME]` (je nach Marketing) ・ Typ ein: CNAME\
・ Verweis auf: Eingabe `[MarketoAccountString].mktoweb.com` (durch Marketing bereitgestellt)

2 - **Hinzufügen CNAME für E-Mail-Tracking-Links**

hinzufügen Sie vom E-Mail-CNAME-Marketing gesendet wurden, sodass `[YourEmailCNAME]` Sie auf [MktoTrackingLink], den standardmäßigen Verfolgungslink, den Marketo zugewiesen hat, im folgenden Format zeigen:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Beispiel:

`pages.abc.com IN CNAME mkto-a0244.com`

3 - Ihr Marketing-Team **benachrichtigen**

Benachrichtigen Sie Ihr Marketingteam, wenn Sie diesen Vorgang abgeschlossen haben.

## Schritt 2: Zulassungsliste Marketo IPs {#step-allowlist-marketo-ips}

Wenn Ihre Marketing-Gruppe mit Marketo Test-E-Mails sendet (eine bewährte Methode, bevor E-Mails gesendet werden), werden die Test-E-Mails manchmal von Spam-Systemen blockiert, die zur Überprüfung der Gültigkeit der E-Mail auf IP-Adressen von Absendern angewiesen sind. Um sicherzustellen, dass diese Test-E-Mails eingehen, fügen Sie Ihrer Zulassungsliste Marketo hinzu.

hinzufügen dieser IP-Adressen auf Ihre Corporate Zulassungsliste:

199.15.212.0/22\
192.28.144.0/20\
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Einige Anti-Spam-Systeme verwenden das Feld Rückkehrpfad der E-Mail anstelle der IP-Adresse für die Zulässigkeit. In diesen Fällen ist der beste Ansatz die Zulassungsliste &quot;*.mktomail.com&quot;, da Marketo mehrere Mailbox-Subdomänen verwendet. Andere Anti-Spam-Systeme werden auf Grundlage der &quot;Von&quot;-Adresse auf die Zulassungsliste gesetzt. Achten Sie in diesen Situationen darauf, alle sendenden (&quot;Von&quot;) Domänen einzuschließen, die Ihre Marketing-Gruppe zur Kommunikation mit Personen/Interessenten verwendet.

>[!NOTE]
>
>Postini verwendet eine einzigartige Technologie und erfordert den Zulassungsauflistung von IP-Bereichen. Siehe [Auf die Zulassungsliste setz mit Postini](http://nation.marketo.com/docs/DOC-1066).

## Schritt 3: Einrichten von SPF und DKIM {#step-set-up-spf-and-dkim}

Ihr Marketing-Team sollte Ihnen auch DKIM-Informationen geschickt haben, die Sie zu Ihrem DNS-Ressourcendatensatz hinzufügen können (siehe auch unten). Gehen Sie wie folgt vor, um DKIM und SPF erfolgreich zu konfigurieren, und teilen Sie Ihrem Marketing-Team dann mit, dass dies aktualisiert wurde.

1. Um SPF einzurichten, fügen Sie unseren DNS-Einträgen die folgende Zeile hinzu:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   umfassen: [mktomail.com](http://mktomail.com/) ~all

   Wenn wir bereits einen SPF-Datensatz in unserem DNS-Eintrag haben, fügen Sie einfach Folgendes hinzu:\
   umfassen: [mktomail.com](http://mktomail.com)

   Ersetzen Sie CompanyDomain durch die Hauptdomäne Ihrer Website (z. B: &quot;`(company.com/)`&quot;) und CorpIP mit der IP-Adresse Ihres Unternehmens-E-Mail-Servers (z. B. &quot;255.255.255.255&quot;). Wenn Sie E-Mails von mehreren Domänen über Marketo senden möchten, sollten Ihre IT-Mitarbeiter diese Zeile für jede Domäne (in einer Zeile) hinzufügen.

1. Erstellen Sie für DKIM DNS-Ressourcendatensätze für jede Domäne, die wir einrichten möchten. Nachfolgend finden Sie die Hostdatensätze und TXT-Werte für jede Domäne, für die wir unterschreiben werden:

   `[DKIMDomain1]`: Host Record ist `[HostRecord1]` und der TXT-Wert ist `[TXTValue1]`.

   `[DKIMDomain2]`: Host Record ist `[HostRecord2]` und der TXT-Wert ist `[TXTValue2]`.

   Kopieren Sie den HostRecord und TXTValue für jede DKIMDomain, die Sie eingerichtet haben, nachdem Sie die [Anweisungen hier](https://docs.marketo.com/display/public/DOCS/Set+up+a+Custom+DKIM+Signature)befolgt haben. Vergessen Sie nicht, jede Domäne unter Admin > E-Mail > DKIM zu überprüfen, nachdem Ihr IT-Personal diesen Schritt abgeschlossen hat.

## Schritt 4: Einrichten von MX-Aufzeichnungen für Ihre Domäne {#step-set-up-mx-records-for-your-domain}

Ein MX-Datensatz ermöglicht es Ihnen, E-Mails an die Domäne zu senden, von der Sie E-Mails senden, um Antworten zu verarbeiten und Autoreparenten. Wenn Sie von Ihrer Unternehmensdomäne aus senden, haben Sie diese wahrscheinlich bereits konfiguriert. Ist dies nicht der Fall, können Sie es normalerweise so einrichten, dass es dem MX-Datensatz Ihrer Unternehmensdomäne zugeordnet wird.
