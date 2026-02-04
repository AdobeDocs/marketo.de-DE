---
unique-page-id: 4720433
description: Konfigurieren von Protokollen für Marketo Engage – Marketo Engage-Dokumente – Produktdokumentation
title: Konfigurieren von Protokollen für Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 100%

---

# Konfigurieren von Protokollen für Marketo Engage{#configure-protocols-for-marketo-engage}

Wenn Sie oder Ihr Unternehmen einschränkende Firewall- oder Proxy-Server-Einstellungen verwenden, müssen Sie oder Ihre bzw. Ihr Netzwerkadmin möglicherweise bestimmte Domains und IP-Adressbereiche auf die Zulassungsliste setzen, um sicherzustellen, dass Adobe Marketo Engage erwartungsgemäß funktioniert.

Wenn Sie Hilfe bei der Implementierung der folgenden Protokolle benötigen, teilen Sie diesen Artikel bitte mit Ihrer IT-Abteilung. Wenn diese Web-Zugriff mithilfe einer Zulassungsliste einschränkt, bitten Sie sie, die folgenden Domains (einschließlich des Sternchens) hinzuzufügen, um alle Marketo-Ressourcen und -Websockets zuzulassen:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Schritt 1: Erstellen von DNS-Einträgen für Landingpages und E-Mails {#step-create-dns-records-for-landing-pages-and-email}

**Tracking-Link-CNAMEs**

Ihr Marketing-Team sollte Ihnen zwei Anfragen für neue CNAME-Einträge gesendet haben. Der erste gilt für Landingpage-URLs, damit die Landingpages in URLs angezeigt werden, die Ihre Domain und nicht Marketo Engage widerspiegeln (der eigentliche Host). Der zweite betrifft Tracking-Links, die in den von Marketo Engage gesendeten E-Mails enthalten sind.

`1` **Hinzufügen von CNAME für Landingpages**

Fügen Sie den erhaltenen Landingpage-CNAME zu Ihrem DNS-Eintrag hinzu, sodass `[YourLandingPageCNAME]` auf die eindeutige Kontozeichenfolge verweist, die Ihren Marketo Engage-Landingpages zugewiesen ist. Melden Sie sich bei der Site Ihrer Domain-Registrierungsstelle an und geben Sie den Landingpage-CNAME und die Kontozeichenfolge ein. Normalerweise gibt es drei Felder:

* Alias: Geben Sie `[YourLandingPageCNAME]` ein (bereitgestellt vom Marketing-Team)
* Typ: CNAME
* Verweist auf: Geben Sie `[MunchkinID].mktoweb.com` ein (bereitgestellt vom Marketing-Team)

`2` **Hinzufügen von CNAME für E-Mail-Tracking-Links**

Fügen Sie den vom Marketing-Team gesendeten E-Mail-CNAME hinzu, sodass `[YourEmailCNAME]` im folgenden Format auf [MktoTrackingLink] (den von Marketo Engage zugewiesenen Standard-Tracking-Link) verweist:
`[YourEmailCNAME].[YourDomain].com` IN CNAME-`[MktoTrackingLink]`

Beispiel:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` muss der standardmäßigen Branding-Domain entsprechen.

`3` **Benachrichtigen des Marketing-Teams**

Benachrichtigen Sie Ihr Marketing-Team, wenn Sie diesen Prozess abgeschlossen haben.

`4` **Kontaktieren des [Adobe-Supports](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"} zum Starten des Prozesses der Bereitstellung eines SIL-Zertifikats.**

Dieser Prozess kann bis zu 3 Werktage dauern.

## Schritt 2: Hinzufügen von Marketo Engage-IPs zur Zulassungsliste {#step-allowlist-marketo-ips}

Wenn Ihre Marketing-Gruppe Marketo Engage zum Senden von Test-E-Mails verwendet (eine Best Practice vor dem Senden von Massen-E-Mail), werden die Test-E-Mails manchmal von Anti-Spam-Systemen blockiert, die zum Überprüfen der Gültigkeit der E-Mail auf Absender-IP-Adressen angewiesen sind. Um sicherzustellen, dass diese Test-E-Mails ankommen, fügen Sie Marketo Engage Ihrer Zulassungsliste hinzu.

Fügen Sie diese IP-Adressen der Zulassungsliste Ihres Unternehmens hinzu:

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Einige Anti-Spam-Systeme verwenden für das Hinzufügen zur Zulassungsliste das Feld des E-Mail-Rücksendepfads anstelle der IP-Adresse. In diesen Fällen ist der beste Ansatz, „&#42;.mktomail.com“ der Zulassungsliste hinzuzufügen, da Marketo Engage mehrere Mailbox-Subdomains verwendet. Andere Anti-Spam-Systeme verwenden für das Hinzufügen zur Zulassungsliste die Absenderadresse. In diesen Fällen müssen Sie alle Versand-Domains („Von“) einbeziehen, die Ihre Marketing-Gruppe für die Kommunikation mit Personen/Leads verwendet.

>[!NOTE]
>
>Postini verwendet eine einzigartige Technologie und erfordert das Hinzufügen von IP-Bereichen zur Zulassungsliste. Weitere Informationen finden Sie unter [Hinzufügen zur Zulassungsliste mit Postini](https://nation.marketo.com/docs/DOC-1066).

## Schritt 3: Einrichten von SPF und DKIM {#step-set-up-spf-and-dkim}

Ihr Marketing-Team sollte Ihnen die DKIM-Informationen (Domain Keys Identified Mail) senden, die Ihrem DNS-Ressourceneintrag hinzugefügt werden sollen (auch unten aufgelistet). Führen Sie die Schritte aus, um DKIM und SPF (Sender Policy Framework) erfolgreich zu konfigurieren, und benachrichtigen Sie nach der Aktualisierung Ihr Marketing-Team.

1. Fügen Sie zur SPF-Einrichtung den DNS-Einträgen die folgende Zeile hinzu:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   Wenn bereits ein SPF-Eintrag im DNS-Eintrag vorhanden ist, fügen Sie einfach Folgendes hinzu:
include: mktomail.com

   Ersetzen Sie „CompanyDomain“ durch die Haupt-Domain Ihrer Website (z. B. „`(company.com/)`“) und „CorpIP“ durch die IP-Adresse des E-Mail-Servers Ihres Unternehmens (z. B. „255.255.255.255“). Wenn Sie E-Mails von mehreren Domains über Marketo Engage senden möchten, sollte Ihr IT-Team diese Zeile für jede Domain hinzufügen (in einer Zeile).

1. Erstellen Sie für DKIM DNS-Ressourceneinträge für jede Domain, die eingerichtet werden soll. Nachfolgend finden Sie die Host-Einträge und TXT-Werte für jede Domain, die signiert werden soll: 

   `[DKIMDomain1]`: Der Host-Eintrag lautet `[HostRecord1]` und der TXT-Wert `[TXTValue1]`.

   `[DKIMDomain2]`: Der Host-Eintrag lautet `[HostRecord2]` und der TXT-Wert `[TXTValue2]`.

   Kopieren Sie den Host-Eintrag und den TXT-Wert für jede DKIM-Domain, die Sie eingerichtet haben, nachdem Sie die [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"} befolgt haben. Vergessen Sie nicht, jede Domain unter „Administrator“ > „E-Mail“ > „DKIM“ zu überprüfen, nachdem Ihr IT-Team diesen Schritt abgeschlossen hat.

## Schritt 4: Einrichten von DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) ist ein Authentifizierungsprotokoll, mit dem Unternehmen ihre Domain vor nicht autorisierter Verwendung schützen können. DMARC erweitert die bestehenden Authentifizierungsprotokolle wie SPF und DKIM, um Empfangs-Server über die Maßnahmen zu informieren, die bei einem Authentifizierungsfehler in ihrer Domain zu ergreifen sind. Obwohl DMARC derzeit optional ist, wird seine Verwendung dringend empfohlen, da es die Marke und den Ruf Ihres Unternehmens besser schützt. Bedeutende Anbieter wie Google und Yahoo verlangen seit Februar 2024, dass DMARC bei massenhaft versendeten Nachrichten verwendet wird.

Damit DMARC funktioniert, müssen Sie über mindestens einen der folgenden DNS-TXT-Einträge verfügen:

* Einen gültigen SPF-Eintrag
* Einen gültigen DKIM-Eintrag für Ihre FROM-Domain (empfohlen für Marketo Engage)

Darüber hinaus müssen Sie über einen DMARC-spezifischen DNS-TXT-Eintrag für Ihre FROM-Domain verfügen. Optional kann eine E-Mail-Adresse Ihrer Wahl definiert werden, um anzugeben, wohin DMARC-Berichte innerhalb Ihres Unternehmens übermittelt sollen, damit Sie Berichte überwachen können.

Als Best Practice wird empfohlen, die DMARC-Implementierung langsam einzuführen, indem Sie Ihre DMARC-Richtlinie von „p=none“ über „p=quarantine“ zu „p=reject“ eskalieren, um Einblick in die potenziellen Auswirkungen von DMARC zu erhalten, und Ihre DMARC-Richtlinie auf eine entspannte Ausrichtung auf SPF und DKIM einstellen.

### Beispiel für einen DMARC-Workflow {#dmarc-example-workflow}

1. Wenn Sie konfiguriert haben, dass Sie DMARC-Berichte erhalten, sollten Sie wie folgt vorgehen …

   I. Analysieren Sie das Feedback und die Berichte, die Sie erhalten, und verwenden Sie „(p=none)“. Dadurch wird der Empfangs-Server angewiesen, keine Aktionen gegen Nachrichten durchzuführen, bei denen die Authentifizierung fehlschlägt, aber dennoch E-Mail-Berichte an den Absender-Server zu senden.

   II. Überprüfen und beheben Sie Probleme mit SPF/DKIM, wenn die Authentifizierung für legitime Nachrichten fehlschlägt.

   III. Prüfen Sie, ob SPF oder DKIM entsprechend abgestimmt sind und die Authentifizierungsprüfung für alle legitimen E-Mails bestehen.

   IV. Überprüfen Sie Berichte, um sicherzustellen, dass die Ergebnisse den Erwartungen gemäß Ihren SPF/DKIM-Richtlinien entsprechen.

1. Stellen Sie nun die Richtlinie auf „(p=quarantine)“ ein. Dadurch wird der empfangende E-Mail-Server angewiesen, E-Mails, die nicht authentifiziert werden können, unter Quarantäne zu stellen (in der Regel werden diese Nachrichten im Spam-Ordner abgelegt).

   I. Überprüfen Sie Berichte, um sicherzustellen, dass die Ergebnisse den Erwartungen entsprechen.

1. Wenn Sie mit dem Verhalten von Nachrichten auf der Ebene „p=quarantine“ zufrieden sind, können Sie die Richtlinie auf „(p=reject)“ einstellen. Die Richtlinie „p=reject“ weist den Empfangs-Server an, jede E-Mail für die Domain, bei der die Authentifizierung fehlschlägt, komplett zu verweigern (Bounce). Wenn diese Richtlinie aktiviert ist, haben nur zu 100 % von Ihrer Domain authentifizierte E-Mails überhaupt die Möglichkeit, im Posteingang zu landen.

>[!CAUTION]
>
>Verwenden Sie diese Richtlinie mit Vorsicht und ermitteln Sie, ob sie für Ihre Organisation geeignet ist.

### DMARC-Reporting {#dmarc-reporting}

DMARC bietet die Möglichkeit, Berichte zu E-Mails zu erhalten, bei denen SPF/DKIM fehlschlägt. Es gibt zwei verschiedene Berichte, die von ISP-Dienstleistern als Teil des Authentifizierungsprozesses generiert werden und die Absenderinnen und Absender über die RUA/RUF-Tags in ihrer DMARC-Richtlinie empfangen können.

* Aggregierte Berichte (RUA): Enthalten keine personenbezogenen Daten (PII), die möglicherweise unter die DSGVO (Datenschutz-Grundverordnung) fallen.

* Forensische Berichte (RUF): Enthalten E-Mail-Adressen, die unter die DSGVO fallen. Prüfen Sie vor der Verwendung intern, wie am besten mit Informationen umgegangen werden soll, die DSGVO-konform sein müssen.

Diese Berichte dienen hauptsächlich dazu, einen Überblick über die E-Mails mit Spoofing-Versuchen zu erhalten. Es handelt sich um hochtechnische Berichte, die am besten über das Tool eines Drittanbieters verarbeitet werden können.

### Beispiel für DMARC-Einträge {#example-dmarc-records}

* Mindesteintrag: `v=DMARC1; p=none`

* Eintrag, der zum Empfang von Berichten an eine E-Mail-Adresse weiterleitet: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC-Tags und ihre Funktionen {#dmarc-tags-and-what-they-do}

DMARC-Einträge umfassen mehrere Komponenten, die als DMARC-Tags bezeichnet werden. Jedes Tag hat einen Wert, der einen bestimmten Aspekt von DMARC festlegt.

<table>
<thead>
  <tr>
    <th>Tag-Name </th>
    <th>Erforderlich/Optional </th>
    <th>Funktion </th>
    <th>Beispiel </th>
    <th>Standardwert </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>Erforderlich</td>
    <td>Dieses DMARC-Tag gibt die Version an. Es gibt derzeit nur eine Version, daher hat diese einen festen Wert von „v=DMARC1“</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Erforderlich</td>
    <td>Zeigt die ausgewählte DMARC-Richtlinie an, die den Empfangs-Server anweist, E-Mails mit fehlgeschlagener Authentifizierungsprüfung zu melden, unter Quarantäne zu stellen oder abzulehnen.</td>
    <td>„p=none“, „p=quarantine“ oder „p=reject“</td>
    <td>–</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Optional</td>
    <td>Ermöglicht der oder dem Domain-Verantwortlichen das Festlegen von Berichtsoptionen.</td>
    <td>0: Generieren eines Berichts, wenn alles fehlschlägt
    <br>1: Generieren eines Berichts, wenn etwas fehlschlägt
    <br>d: Generieren eines Berichts, wenn DKIM fehlschlägt
    <br>s: Generieren eines Berichts, wenn SPF fehlschlägt</td>
    <td>1 (empfohlen für DMARC-Berichte)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Optional</td>
    <td>Gibt den Prozentsatz der Nachrichten an, die gefiltert werden.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Optional (empfohlen)</td>
    <td>Gibt an, wohin aggregierte Berichte gesendet werden.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>–</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Optional (empfohlen)</td>
    <td>Gibt an, wohin forensische Berichte gesendet werden.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>–</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Optional</td>
    <td>Gibt die DMARC-Richtlinie für Subdomains der übergeordneten Domain an.</td>
    <td>sp=reject</td>
    <td>–</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Optional</td>
    <td>Kann entweder strikt (s) oder locker (r) sein. Eine lockere Ausrichtung bedeutet, dass die in der DKIM-Signatur verwendete Domain eine Subdomain der Absenderadresse sein kann. Eine strikte Ausrichtung bedeutet, dass die in der DKIM-Signatur verwendete Domain exakt mit der in der Absenderadresse verwendeten Domain übereinstimmen muss.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Optional</td>
    <td>Kann entweder strikt (s) oder locker (r) sein. Eine lockere Ausrichtung bedeutet, dass die Domain des Rücksendepfads eine Subdomain der Absenderadresse sein kann. Eine strikte Ausrichtung bedeutet, dass die Domain des Rücksendepfads exakt mit der Absenderadresse übereinstimmen muss.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Ausführliche Informationen zu DMARC und allen zugehörigen Optionen finden Sie unter [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC und Marketo Engage {#dmarc-and-marketo-engage}

Es gibt zwei Arten der Ausrichtung für DMARC: DKIM-Ausrichtung und SPF-Ausrichtung.

>[!NOTE]
>
>Es wird empfohlen, die DMARC-Ausrichtung auf DKIM vs. SPF für Marketo Engage durchzuführen.

* Auf DKIM ausgerichtetes DMARC: Zum Einrichten von auf DKIM ausgerichtetes DMARC müssen Sie folgende Schritte vornehmen:

   * Richten Sie DKIM für die FROM-Domain Ihrer Nachricht ein. Befolgen Sie die Anweisungen [in diesem Artikel](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Konfigurieren Sie DMARC für die zuvor konfigurierte FROM/DKIM-Domain.

* Auf DMARC ausgerichtetes SPF: Zum Einrichten von auf DMARC ausgerichtetes SPF über den Rücksendepfad mit Branding müssen Sie folgende Schritte vornehmen:

   * Richten Sie die Rücksendepfad-Domain mit Branding ein.
      * Konfigurieren Sie den entsprechenden SPF-Eintrag.
      * Ändern Sie den MX-Eintrag so, dass er auf Standard-MX für das Rechenzentrum verweist, von dem aus Ihre E-Mails gesendet werden.

   * Konfigurieren Sie DMARC für die Rücksendepfad-Domain mit Branding.

* Wenn Sie E-Mails von Marketo Engage über eine dedizierte IP-Adresse senden und noch keinen Rücksendepfad mit Branding implementiert haben oder sich nicht sicher sind, ob dies der Fall ist, erstellen Sie ein Ticket beim [Adobe-Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"}.

* Wenn Sie E-Mails von Marketo Engage über einen gemeinsam genutzten Pool an IP-Adressen senden, können Sie [hier](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"} überprüfen, ob Sie für eine vertrauenswürdige IP-Adresse qualifiziert sind. Der Rücksendepfad mit Branding wird denjenigen kostenlos angeboten, die E-Mails von vertrauenswürdigen Marketo Engage-IP-Adressen senden. Wenn Ihr Antrag für eine Teilnahme an diesem Programm genehmigt wurde, wenden Sie sich an den Adobe-Support, um den Rücksendepfad mit Branding einzurichten.

   * Vertrauenswürdige IP-Adressen: Ein gemeinsam genutzter Pool an IP-Adressen, die für Benutzende mit geringerem Sendevolumen von weniger als 75.000 Nachrichten pro Monat reserviert sind, die nicht für eine dedizierte IP-Adresse qualifiziert sind. Diese Benutzenden müssen auch die Best-Practice-Anforderungen erfüllen.

* Wenn Sie E-Mails von Marketo Engage über gemeinsam genutzte IP-Adressen senden, nicht für vertrauenswürdige IP-Adressen qualifiziert sind und monatlich mehr als 100.000 Nachrichten senden, müssen Sie sich an das Adobe-Accountteam (Ihre Kundenbetreuung) wenden, um eine dedizierte IP zu erwerben.

* Eine strikte SPF-Ausrichtung wird für Marketo Engage weder unterstützt noch empfohlen.

## Schritt 5: Einrichten von MX-Einträgen für Ihre Domain {#step-set-up-mx-records-for-your-domain}

Ein MX-Eintrag ermöglicht es Ihnen, E-Mails über die Domain zu empfangen, von der aus Sie E-Mails senden, um Antworten und Abwesenheitsnachrichten zu verarbeiten. Wenn Sie E-Mails von Ihrer Unternehmens-Domain aus senden, haben Sie dies wahrscheinlich bereits konfiguriert. Falls nicht, können Sie dies in der Regel so einrichten, dass eine Zuordnung zum MX-Eintrag Ihrer Unternehmens-Domain erfolgt.

## Ausgehende IP-Adressen {#outbound-ip-addresses}

Eine ausgehende Verbindung ist eine Verbindung, die Marketo Engage in Ihrem Namen zu einem Server im Internet herstellt. Einige Partner/Anbieter, mit denen Sie zusammenarbeiten, oder Ihre eigene IT-Organisation verwenden möglicherweise Zulassungslisten, um den Zugriff auf Server zu beschränken. In diesem Fall müssen Sie ihnen die Blöcke ausgehender Marketo Engage-IP-Adressen bereitstellen, damit sie sie ihren Zulassungslisten hinzufügen können.

**Webhooks**

Marketo Engage-[Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} sind ein ausgehender Integrationsmechanismus. Wenn eine Flussaktion des Typs [Webhook aufrufen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} als Teil einer intelligenten Kampagne ausgeführt wird, wird eine HTTP-Anfrage an einen externen Webservice gesendet. Wenn der Herausgeber des Webservice eine Zulassungsliste in der Firewall des Netzwerks verwendet, in dem sich der externe Webservice befindet, muss der Herausgeber die unten aufgeführten IP-Adressblöcke zu seiner Zulassungsliste hinzufügen.

**CRM-Synchronisierung**

[Salesforce CRM-Synchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} und [Microsoft Dynamics-Synchronisierung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} von Marketo Engage sind Integrationsmechanismen, die ausgehende HTTP-Anfragen an APIs senden, die von Ihrem CRM-Anbieter veröffentlicht wurden. Sie müssen sicherstellen, dass Ihre IT-Organisation keinen der unten aufgeführten IP-Adressblöcke vom Zugriff auf Ihre CRM-Anbieter-APIs blockiert.

**Ausgehende IP-Adressblöcke für Marketo Engage**

In den folgenden Tabellen sind alle Marketo Engage-Server aufgeführt, die ausgehende Aufrufe ausführen. Verwenden Sie die folgenden Listen zum Konfigurieren von IP-Zulassungslisten, Servern, Firewalls, Zugriffssteuerungslisten, Sicherheitsgruppen oder Drittanbieterdiensten für den Empfang ausgehender Verbindungen von Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>IP-Block (CIDR-Notation)</th>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
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
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>Einzelne IP-Adresse</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
