---
unique-page-id: 4720433
description: Konfigurieren von Protokollen für Marketo - Marketo Docs - Produktdokumentation
title: Protokolle für Marketo konfigurieren
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 3f0ccfcb22e0b84c6d1e60b750af955cb442bd36
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 2%

---

# Protokolle für Marketo konfigurieren {#configure-protocols-for-marketo}

Wenn Sie oder Ihr Unternehmen restriktive Firewall- oder Proxy-Server-Einstellungen verwenden, müssen Sie oder Ihr Netzwerkadministrator möglicherweise bestimmte Domänen und IP-Adressbereiche in Zulassungslisten eintragen, um sicherzustellen, dass Adobe Marketo Engage erwartungsgemäß funktioniert.

## Einstiegsseiten und E-Mails für Markenkampagnen {#branded-campaign-landing-pages-and-emails}

Ihre Marketing-Gruppe verwendet Marketo, um Landingpages und E-Mails für Markenkampagnen zu erstellen. Um sicherzustellen, dass diese Landingpages und E-Mails funktionieren, benötigen sie ein wenig Hilfe von der IT. Bitte richten Sie die folgenden Protokolle ein, mit den Informationen, die Ihre Marketing-Gruppe Ihnen per E-Mail geschickt haben sollte.

Dieser Artikel sollte an die IT-Abteilung des Unternehmens weitergegeben werden, das diese Protokolle implementieren möchte.

>[!NOTE]
>
>Wenn Ihr IT-Team den Webzugriff mithilfe einer Zulassungsliste einschränkt, bitten Sie sie, die folgenden Domänen hinzuzufügen (einschließlich des Sternchens), um alle Marketo-Ressourcen und -Websockets zuzulassen:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`

## Schritt 1: DNS-Einträge für Einstiegsseiten und E-Mail erstellen {#step-create-dns-records-for-landing-pages-and-email}

**Tracking-Link-CNAMEs**

Ihr Marketing-Team sollte Ihnen zwei Anfragen für neue CNAME-Einträge gesendet haben. Die erste bezieht sich auf Landingpage-URLs, sodass die Landingpages in URLs angezeigt werden, die Ihre Domäne und nicht Marketo (der eigentliche Host) widerspiegeln. Die zweite betrifft die Tracking-Links, die in den von Marketo gesendeten E-Mails enthalten sind.

`1` **Hinzufügen von CNAME für Einstiegsseiten**

Fügen Sie den CNAME der Landingpage hinzu, den Sie an Ihren DNS-Eintrag gesendet haben, sodass `[YourLandingPageCNAME]` verweist auf die eindeutige Kontozeichenfolge, die Ihren Marketo-Landingpages zugewiesen ist. Melden Sie sich bei der Site Ihres Domänenregistrierers an und geben Sie den CNAME und die Kontozeichenfolge der Landingpage ein. In der Regel umfasst dies drei Felder:

* Alias: Eingabe `[YourLandingPageCNAME]` (durch die Vermarktung bereitgestellt)
* Typ: CNAME
* Verweis auf: Eingabe `[MarketoAccountString].mktoweb.com` (durch die Vermarktung bereitgestellt)

`2` **Hinzufügen von CNAME für E-Mail-Tracking-Links**

Fügen Sie das von Ihnen gesendete E-Mail-CNAME-Marketing hinzu, damit `[YourEmailCNAME]` weist auf [MktoTrackingLink], den standardmäßigen Tracking-Link, den Marketo im folgenden Format zugewiesen hat:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Zum Beispiel:

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Benachrichtigung für Ihr Marketing-Team**

Benachrichtigen Sie Ihr Marketing-Team, wenn Sie diesen Vorgang abgeschlossen haben.

`4` **Kontakt [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;}, um den Prozess der Bereitstellung eines SSL-Zertifikats zu starten.**

Dieser Vorgang kann bis zu drei Werktage dauern.

## Schritt 2: Marketo-IPs der Zulassungsliste {#step-allowlist-marketo-ips}

Wenn Ihre Marketing-Gruppe Marketo zum Versand von Test-E-Mails verwendet (eine Best Practice vor dem Versand von E-Mail-Nachrichten), werden die Test-E-Mails manchmal von Anti-Spam-Systemen blockiert, die zur Überprüfung der Gültigkeit der E-Mail auf Absender-IP-Adressen angewiesen sind. Um sicherzustellen, dass diese Test-E-Mails eintreffen, fügen Sie Marketo zu Ihrer Zulassungsliste hinzu.

Fügen Sie diese IP-Adressen zu Ihrer Unternehmens-Zulassungsliste hinzu:

199.15.212.0/22\
192.28.144.0/20 192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Einige Anti-Spam-Systeme verwenden für die Zulässigkeit das Feld Rückkehrpfad der E-Mail anstelle der IP-Adresse. In diesen Fällen ist der beste Ansatz die Zulassungsliste &quot;&#42;.mktomail.com&quot;, da Marketo mehrere Postfach-Subdomains verwendet. Andere Anti-Spam-Systeme werden basierend auf der Absenderadresse auf die Zulassungsliste gesetzt. Stellen Sie in diesen Situationen sicher, dass Sie alle sendenden (&quot;Von&quot;) Domänen einschließen, die Ihre Marketing-Gruppe zur Kommunikation mit Personen/Leads verwendet.

>[!NOTE]
>
>Postini setzt eine einzigartige Technologie ein und erfordert den auf die Zulassungsliste setz von IP-Bereichen. Siehe [Auf die Zulassungsliste setz mit Postini](https://nation.marketo.com/docs/DOC-1066).

## Schritt 3: Einrichten von SPF und DKIM {#step-set-up-spf-and-dkim}

Ihr Marketing-Team sollte Ihnen auch DKIM-Informationen gesendet haben, die zu Ihrem DNS-Ressourcendatensatz hinzugefügt werden sollen (ebenfalls unten aufgeführt). Führen Sie die Schritte aus, um DKIM und SPF erfolgreich zu konfigurieren, und benachrichtigen Sie dann Ihr Marketing-Team, dass dies aktualisiert wurde.

1. Um SPF einzurichten, fügen Sie unseren DNS-Einträgen die folgende Zeile hinzu:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Wenn wir bereits einen vorhandenen SPF-Eintrag in unserem DNS-Eintrag haben, fügen Sie einfach Folgendes hinzu:\
   include: mktomail.com

   Ersetzen Sie CompanyDomain durch die Hauptdomäne Ihrer Website (z. B.: &quot;`(company.com/)`&quot;) und CorpIP mit der IP-Adresse Ihres Unternehmens-E-Mail-Servers (z. B. &quot;255 255 255 255 255&quot;). Wenn Sie E-Mails von mehreren Domänen über Marketo versenden möchten, sollten Ihre IT-Mitarbeiter diese Zeile für jede Domäne hinzufügen (in einer Zeile).

1. Erstellen Sie für DKIM DNS-Ressourcendatensätze für jede Domäne, die wir einrichten möchten. Im Folgenden finden Sie die Hostdatensätze und TXT-Werte für jede Domäne, für die wir Signieren werden:

   `[DKIMDomain1]`: Hostdatensatz ist `[HostRecord1]` und der TXT-Wert `[TXTValue1]`.

   `[DKIMDomain2]`: Hostdatensatz ist `[HostRecord2]` und der TXT-Wert `[TXTValue2]`.

   Kopieren Sie den HostRecord und den TXTValue für jede DKIMDomain, die Sie eingerichtet haben, nachdem Sie der folgenden [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target=&quot;_blank&quot;}. Vergessen Sie nicht, jede Domäne unter Admin > E-Mail > DKIM zu überprüfen, nachdem Ihre IT-Mitarbeiter diesen Schritt abgeschlossen haben.

## Schritt 4: Einrichten von MX-Datensätzen für Ihre Domäne {#step-set-up-mx-records-for-your-domain}

Ein MX-Datensatz ermöglicht es Ihnen, E-Mails an die Domain zu erhalten, von der Sie E-Mails senden, um Antworten und Autoreaktoren zu verarbeiten. Wenn Sie von Ihrer Unternehmensdomäne aus senden, ist dies wahrscheinlich bereits konfiguriert. Andernfalls können Sie es normalerweise so einrichten, dass es dem MX-Datensatz Ihrer Unternehmensdomäne zugeordnet wird.

## Ausgehende IP-Adressen {#outbound-ip-addresses}

Eine ausgehende Verbindung erfolgt per Marketo Engage an einen Server im Internet in Ihrem Namen. Einige Partner/Anbieter, mit denen Sie zusammenarbeiten, oder Ihre eigene IT-Organisation können Zulassungslisten verwenden, um den Zugriff auf Server zu beschränken. In diesem Fall müssen Sie ihnen ausgehende IP-Adressblöcke aus dem Marketo Engage bereitstellen, um sie ihren auf die Zulassungsliste setz hinzuzufügen.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;} sind ein ausgehender Integrationsmechanismus. Wenn eine [Webhook aufrufen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md)Die Flussaktion {target=&quot;_blank&quot;} wird im Rahmen einer intelligenten Kampagne ausgeführt. Eine HTTP-Anfrage wird an einen externen Webdienst gesendet. Wenn der Webdienst-Herausgeber eine Zulassungsliste in der Firewall des Netzwerks verwendet, in dem sich der externe Webdienst befindet, muss der Herausgeber die unten aufgeführten IP-Adressblöcke zu seiner Zulassungsliste hinzufügen.

**CRM-Synch.**

Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;} und [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;} sind Integrationsmechanismen, die ausgehende HTTP-Anfragen an APIs senden, die von Ihrem CRM-Anbieter veröffentlicht werden. Sie müssen sicherstellen, dass Ihre IT-Organisation den Zugriff auf Ihre CRM-Anbieter-APIs nicht durch einen der unten stehenden IP-Adressblöcke blockiert.

**Ausgehende IP-Adressblöcke aus Marketo Engage**

Die folgende Tabelle enthält alle Marketo Engage-Server, die ausgehende Aufrufe durchführen. Verwenden Sie diese Liste, wenn Sie IP-Zulassungsliste, Server, Firewall, Zugriffssteuerungsliste, Sicherheitsgruppe oder Dienste von Drittanbietern konfigurieren, um ausgehende Verbindungen von Marketo Engage zu empfangen.

<table>
 <tbody>
  <tr>
   <th>IP-Block (CIDR-Notation)</th>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
   <tr>
   <td>192.28.160.0/19</td>
  </tr>
   <tr>
   <td>199.15.212.0/22</td>
  </tr>
   <tr>
   <td>185.28.196.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
 </tbody>
</table>