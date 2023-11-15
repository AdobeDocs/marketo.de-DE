---
description: Aktualisierte Konfiguration von Protokollen Doc - Marketo Docs - Produktdokumentation
title: Aktualisiertes Dokument zum Konfigurieren von Protokollen
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 10458ed8bc6553e11686d00dacc1ba36d683ab56
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 3%

---

# Aktualisiertes Dokument zum Konfigurieren von Protokollen {#updated-configure-protocols-doc}

Wenn Sie oder Ihr Unternehmen restriktive Firewall- oder Proxy-Server-Einstellungen verwenden, müssen Sie oder Ihr Netzwerkadministrator möglicherweise bestimmte Domänen und IP-Adressbereiche in Zulassungslisten eintragen, um sicherzustellen, dass Adobe Marketo Engage erwartungsgemäß funktioniert.

Wenn Sie Hilfe bei der Implementierung der folgenden Protokolle benötigen, teilen Sie diesen Artikel mit Ihrer IT-Abteilung. Wenn der Webzugriff über eine Zulassungsliste eingeschränkt wird, stellen Sie sicher, dass die folgenden Domänen (einschließlich des Sternchens) hinzugefügt werden, um alle Marketo-Ressourcen und -Websockets zuzulassen:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Schritt 1: DNS-Einträge für Landingpages und E-Mails erstellen {#step-create-dns-records-for-landing-pages-and-email}

**Tracking-Link-CNAMEs**

Ihr Marketing-Team sollte Ihnen zwei Anfragen für neue CNAME-Einträge gesendet haben. Die erste bezieht sich auf Landingpage-URLs, sodass die Landingpages in URLs angezeigt werden, die Ihre Domäne und nicht Marketo (der eigentliche Host) widerspiegeln. Die zweite betrifft die Tracking-Links, die in den von Marketo gesendeten E-Mails enthalten sind.

`1` **Hinzufügen von CNAME für Einstiegsseiten**

Fügen Sie den CNAME der Landingpage hinzu, den Sie an Ihren DNS-Eintrag gesendet haben, sodass `[YourLandingPageCNAME]` verweist auf die eindeutige Kontozeichenfolge, die Ihren Marketo-Landingpages zugewiesen ist. Melden Sie sich bei der Site Ihres Domänenregistrierers an und geben Sie den CNAME und die Kontozeichenfolge der Landingpage ein. In der Regel umfasst dies drei Felder:

* Alias: Enter `[YourLandingPageCNAME]` (durch die Vermarktung bereitgestellt)
* Typ: CNAME
* Point to: Enter `[MunchkinID].mktoweb.com` (durch die Vermarktung bereitgestellt)

`2` **Hinzufügen von CNAME für E-Mail-Tracking-Links**

Fügen Sie das von Ihnen gesendete E-Mail-CNAME-Marketing hinzu, damit `[YourEmailCNAME]` weist auf [MktoTrackingLink], den standardmäßigen Tracking-Link, den Marketo im folgenden Format zugewiesen hat:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Beispiel:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` muss die Standard-Branding-Domäne sein.

`3` **Benachrichtigung für Ihr Marketing-Team**

Benachrichtigen Sie Ihr Marketing-Team, wenn Sie diesen Vorgang abgeschlossen haben.

`4` **Kontakt [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} , um die Bereitstellung eines SSL-Zertifikats zu starten.**

Dieser Vorgang kann bis zu drei Werktage dauern.

## Schritt 2: Zulassungsliste der Marketo-IPs {#step-allowlist-marketo-ips}

Wenn Ihre Marketing-Gruppe Marketo zum Versand von Test-E-Mails verwendet (eine Best Practice vor dem Versand von E-Mail-Nachrichten), werden die Test-E-Mails manchmal von Anti-Spam-Systemen blockiert, die zur Überprüfung der Gültigkeit der E-Mail auf Absender-IP-Adressen angewiesen sind. Um sicherzustellen, dass diese Test-E-Mails eintreffen, fügen Sie Marketo zu Ihrer Zulassungsliste hinzu.

Fügen Sie diese IP-Adressen zu Ihrer Unternehmens-Zulassungsliste hinzu:

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Einige Anti-Spam-Systeme verwenden für die Zulässigkeit das Feld Rückkehrpfad der E-Mail anstelle der IP-Adresse. In diesen Fällen ist der beste Ansatz die Zulassungsliste &quot;&#42;.mktomail.com&#39;, da Marketo mehrere Postfach-Subdomains verwendet. Andere Anti-Spam-Systeme werden basierend auf der Absenderadresse auf die Zulassungsliste gesetzt. Stellen Sie in diesen Situationen sicher, dass Sie alle sendenden (&quot;Von&quot;) Domänen einschließen, die Ihre Marketing-Gruppe zur Kommunikation mit Personen/Leads verwendet.

>[!NOTE]
>
>Postini setzt eine einzigartige Technologie ein und erfordert den auf die Zulassungsliste setz von IP-Bereichen. Siehe [Auf die Zulassungsliste setz mit Postini](https://nation.marketo.com/docs/DOC-1066).

## Schritt 3: Einrichten von SPF und DKIM {#step-set-up-spf-and-dkim}

Ihr Marketing-Team sollte Ihnen auch DKIM-Informationen (Domain Keys Identified Mail) gesendet haben, die zu Ihrem DNS-Ressourcendatensatz hinzugefügt werden sollen (ebenfalls unten aufgeführt). Führen Sie die Schritte aus, um DKIM und SPF (Sender Policy Framework) erfolgreich zu konfigurieren, und benachrichtigen Sie dann Ihr Marketing-Team, dass dies aktualisiert wurde.

1. Um SPF einzurichten, fügen Sie unseren DNS-Einträgen die folgende Zeile hinzu:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Wenn wir bereits einen vorhandenen SPF-Eintrag in unserem DNS-Eintrag haben, fügen Sie einfach Folgendes hinzu:\
   include: mktomail.com

   Ersetzen Sie CompanyDomain durch die Hauptdomäne Ihrer Website (z. B.: &quot;`(company.com/)`&quot;) und CorpIP mit der IP-Adresse Ihres Unternehmens-E-Mail-Servers (z. B. &quot;255.255.255.255&quot;). Wenn Sie E-Mails von mehreren Domänen über Marketo versenden möchten, sollten Ihre IT-Mitarbeiter diese Zeile für jede Domäne hinzufügen (in einer Zeile).

1. Erstellen Sie für DKIM DNS-Ressourcendatensätze für jede Domäne, die wir einrichten möchten. Im Folgenden finden Sie die Hostdatensätze und TXT-Werte für jede Domäne, für die wir Signieren werden:

   `[DKIMDomain1]`: Hostdatensatz ist `[HostRecord1]` und der TXT-Wert `[TXTValue1]`.

   `[DKIMDomain2]`: Hostdatensatz ist `[HostRecord2]` und der TXT-Wert `[TXTValue2]`.

   Kopieren Sie den HostRecord und den TXTValue für jede DKIMDomain, die Sie eingerichtet haben, nachdem Sie der [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Vergessen Sie nicht, jede Domäne unter Admin > E-Mail > DKIM zu überprüfen, nachdem Ihre IT-Mitarbeiter diesen Schritt abgeschlossen haben.

## Schritt 4: Einrichten von DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) {#set-up-dmarc}

DMARC ist ein Authentifizierungsprotokoll, das Unternehmen dabei unterstützt, ihre Domain vor unbefugter Verwendung zu schützen. DMARC erweitert die vorhandenen Authentifizierungsprotokolle wie SPF und DKIM, um Empfängerserver darüber zu informieren, welche Aktionen sie ergreifen sollten, wenn bei ihrer Domäne ein Authentifizierungsfehler auftritt. DMARC ist zwar derzeit optional, wird jedoch dringend empfohlen, da es die Marke und Reputation Ihres Unternehmens besser schützt. Wichtige Anbieter wie Google und Yahoo werden ab Februar 2024 die Verwendung von DMARC für Massensender benötigen.

Damit DMARC funktioniert, muss mindestens einer der folgenden DNS-TXT-Einträge vorhanden sein:

* Eine gültige SPF
* Ein gültiger DKIM-Datensatz für Ihre FROM: Domain (empfohlen für Marketo Engage)

Darüber hinaus müssen Sie einen DMARC-spezifischen DNS-TXT-Eintrag für Ihre FROM: Domain haben. Optional kann eine E-Mail-Adresse Ihrer Wahl definiert werden, um anzugeben, wohin DMARC-Berichte in Ihrem Unternehmen untergebracht werden sollen, damit Sie Berichte überwachen können.

Als Best Practice wird empfohlen, die DMARC-Implementierung langsam einzuführen, indem Sie Ihre DMARC-Richtlinie von p=none auf p=quarantine eskalieren, p=reject ändern, sobald Sie die potenziellen Auswirkungen von DMARC verstehen, und Ihre DMARC-Richtlinie auf eine entspannte Ausrichtung auf SPF und DKIM festlegen.

### DMARC-Beispiel-Workflow {#dmarc-example-workflow}

1. Wenn Sie für den Empfang von DMARC-Berichten konfiguriert sind, sollten Sie Folgendes tun..

   I. Analysieren Sie das Feedback und die Berichte, die Sie erhalten und verwenden (p=none), wodurch der Empfänger angewiesen wird, keine Aktionen für Nachrichten durchzuführen, die die Authentifizierung nicht befolgen, aber trotzdem E-Mail-Berichte an den Absender senden senden.

   II. Überprüfen und beheben Sie Probleme mit SPF/DKIM, wenn die Authentifizierung bei legitimen Nachrichten fehlschlägt.

   III. Bestimmen Sie, ob SPF oder DKIM abgestimmt sind, und übergeben Sie die Authentifizierung für alle legitimen E-Mails.

   IV. Überprüfen Sie Berichte, um sicherzustellen, dass die Ergebnisse basierend auf Ihren SPF/DKIM-Richtlinien erwartet werden.

1. Fahren Sie fort, um die Richtlinie auf (p=quarantine) anzupassen, wodurch der E-Mail-Empfangs-Server angewiesen wird, E-Mails unter Quarantäne zu stellen, bei denen die Authentifizierung fehlschlägt (dies bedeutet normalerweise, dass diese Nachrichten im Spam-Ordner abgelegt werden).

   I. Prüfen Sie die Berichte, um sicherzustellen, dass die Ergebnisse Ihren Erwartungen entsprechen.

1. Wenn Sie mit dem Verhalten von Nachrichten auf der Ebene p=quarantine zufrieden sind, können Sie die Richtlinie auf (p=reject) anpassen. Die p=reject-Richtlinie weist den Empfänger an, jede E-Mail für die Domain, bei der die Authentifizierung fehlschlägt, vollständig zu verweigern (Bounce). Wenn diese Richtlinie aktiviert ist, haben nur E-Mails, die zu 100 % von Ihrer Domain authentifiziert wurden, sogar die Möglichkeit, die Platzierung im Posteingang vorzunehmen.

>[!CAUTION]
>
>Verwenden Sie diese Richtlinie mit Vorsicht und stellen Sie fest, ob sie für Ihre Organisation geeignet ist.

### DMARC-Berichterstellung {#dmarc-reporting}

DMARC bietet die Möglichkeit, Berichte zu E-Mails zu erhalten, die SPF/DKIM nicht unterstützen. Es gibt zwei verschiedene Berichte, die von ISP-Dienstern im Rahmen des Authentifizierungsprozesses generiert werden und die Absender über die RUA/RUF-Tags in ihrer DMARC-Richtlinie empfangen können.

* Aggregate Reports (RUA): Enthält keine personenbezogenen Daten, die bei DSGVO (Datenschutz-Grundverordnung) berücksichtigt werden.

* Kriminalitätsberichte (RUF): Enthält E-Mail-Adressen, die DSGVO-konform sind. Vor der Verwendung sollten Sie intern überprüfen, wie mit Informationen umgegangen werden soll, die DSGVO-konform sein müssen.

Diese Berichte dienen hauptsächlich dazu, einen Überblick über E-Mails zu erhalten, die versucht werden, Nachrichten zu spoofing zu senden. Dies sind hochtechnische Berichte, die am besten mit einem Tool von Drittanbietern aufbereitet werden.

### Beispiele für DMARC-Aufzeichnungen {#example-dmarc-records}

* Standardmäßige Mindestaufzeichnungen: `v=DMARC1; p=none`

* Datensatz, der sich an eine E-Mail-Adresse richtet, um Berichte zu erhalten: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC-Tags und ihre Aufgaben {#dmarc-tags-and-what-they-do}

DMARC-Datensätze verfügen über mehrere Komponenten, die DMARC-Tags genannt werden. Jedes Tag verfügt über einen Wert, der einen bestimmten Aspekt von DMARC angibt.

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
    <td>Dieses DMARC-Tag gibt die Version an. Derzeit gibt es nur eine Version. Daher hat diese den festen Wert v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Erforderlich</td>
    <td>Zeigt die ausgewählte DMARC-Richtlinie an und weist den Empfänger an, E-Mails zu melden, unter Quarantäne zu stellen oder abzulehnen, die bei Authentifizierungsprüfungen fehlschlagen.</td>
    <td>p=none, quarantine or reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Optional</td>
    <td>Ermöglicht es dem Domäneninhaber, Berichtsoptionen anzugeben.</td>
    <td>0: Bericht erstellen, wenn alles fehlschlägt 
    <br>1: Bericht erstellen, wenn alles fehlschlägt 
    <br>d: Bericht erstellen, wenn DKIM fehlschlägt 
    <br>s: Bericht erstellen, wenn SPF fehlschlägt</td>
    <td>1 (empfohlen für DMARC-Berichte)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Optional</td>
    <td>Teilt den Prozentsatz der Nachrichten mit, die gefiltert werden sollen.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Optional (empfohlen)</td>
    <td>Gibt an, wo aggregierte Berichte bereitgestellt werden.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Optional (empfohlen)</td>
    <td>Gibt an, wo forensische Berichte bereitgestellt werden.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Optional</td>
    <td>Gibt die DMARC-Richtlinie für Subdomänen der übergeordneten Domäne an.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Optional</td>
    <td>Kann entweder streng (s) oder Relaxed ® sein. Eine verzögerte Ausrichtung bedeutet, dass die in der DKIM-Signatur verwendete Domain eine Subdomäne der "Von"-Adresse sein kann. Eine strikte Ausrichtung bedeutet, dass die in der DKIM-Signatur verwendete Domain exakt mit der in der Absenderadresse verwendeten Domain übereinstimmen muss.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Optional</td>
    <td>Kann entweder streng (s) oder Relaxed ® sein. Eine verzögerte Ausrichtung bedeutet, dass die Domäne "ReturnPath"eine Subdomäne der "From Address"sein kann. Eine strikte Ausrichtung bedeutet, dass die Domäne "Return-Path"exakt mit der Absenderadresse übereinstimmen muss.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Ausführliche Informationen zu DMARC und all seinen Optionen finden Sie unter [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC und Marketo Engage {#dmarc-and-marketo-engage}

Es gibt zwei Arten der Ausrichtung für DMARC: DKIM-Ausrichtung und SPF-Ausrichtung.

>[!NOTE]
>
>Es wird empfohlen, die DMARC-Ausrichtung auf DKIM im Vergleich zu SPF für Marketo durchzuführen.

* DKIM-angepasstes DMARC: Um DKIM-angepasstes DMARC einzurichten, müssen Sie:

   * Richten Sie DKIM für die Domäne &quot;FROM: Domain&quot;Ihrer Nachricht ein. Anleitung verwenden [in diesem Artikel](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Konfigurieren Sie DMARC für die zuvor konfigurierte Domäne &quot;FROM:/DKIM&quot;

* DMARC-angepasste SPF: Um DMARC-angepasste SPF über einen gebrandeten Rückkehrpfad einzurichten, müssen Sie:

   * Einrichten der Branded-Return-Path-Domäne
      * Konfigurieren des entsprechenden SPF-Datensatzes
      * Ändern Sie den MX-Datensatz so, dass er auf den Standard-MX für das Rechenzentrum verweist, aus dem Ihre E-Mail gesendet wird.

   * Konfigurieren von DMARC für die Domäne &quot;Branded Return Path&quot;

* Wenn Sie E-Mails von Marketo über eine dedizierte IP versenden und den Branded-Return-Pfad noch nicht implementiert haben oder nicht sicher sind, ob Sie dies getan haben, öffnen Sie bitte ein Ticket mit [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Wenn Sie E-Mails von Marketo über einen freigegebenen IP-Pool senden, können Sie sehen, ob Sie sich für vertrauenswürdige IPs qualifizieren durch [hier anwenden](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. Der Branded-Rückkehrpfad wird denjenigen, die von vertrauenswürdigen IPs von Marketo senden, kostenlos angeboten. Wenn Sie für dieses Programm genehmigt wurden, wenden Sie sich an den Marketo-Support , um einen Branded-Return-Pfad einzurichten.

   * Vertrauenswürdige IPs: Ein freigegebener IP-Pool, der für Benutzer mit niedrigem Volumen reserviert ist, die &lt;75 K/Monat senden und sich nicht für eine dedizierte IP-Adresse qualifizieren. Diese Benutzer müssen auch die Best-Practice-Anforderungen erfüllen.

* Wenn Sie E-Mails von Marketo über freigegebene IPs versenden und sich nicht für vertrauenswürdige IPs qualifizieren und monatlich mehr als 100.000 Nachrichten senden, müssen Sie sich an das Adobe Account Team (Ihren Kundenbetreuer) wenden, um eine dedizierte IP zu erwerben.

* Eine strikte SPF-Ausrichtung wird in Marketo weder unterstützt noch empfohlen.

## Schritt 5: Einrichten von MX-Datensätzen für Ihre Domäne {#step-set-up-mx-records-for-your-domain}

Ein MX-Datensatz ermöglicht es Ihnen, E-Mails an die Domain zu erhalten, von der Sie E-Mails senden, um Antworten und Autoreaktoren zu verarbeiten. Wenn Sie von Ihrer Unternehmensdomäne aus senden, ist diese wahrscheinlich bereits konfiguriert. Andernfalls können Sie es normalerweise so einrichten, dass es dem MX-Datensatz Ihrer Unternehmensdomäne zugeordnet wird.

## Ausgehende IP-Adressen {#outbound-ip-addresses}

Eine ausgehende Verbindung wird durch Marketo Engage an einen Server im Internet in Ihrem Namen hergestellt. Einige Partner/Anbieter, mit denen Sie zusammenarbeiten, oder Ihre eigene IT-Organisation können Zulassungslisten verwenden, um den Zugriff auf Server zu beschränken. In diesem Fall müssen Sie ihnen ausgehende IP-Adressblöcke mit Marketo Engage zur Verfügung stellen, um sie zu ihren auf die Zulassungsliste setz hinzuzufügen.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} die Flow-Aktion im Rahmen einer Smart-Kampagne ausgeführt wird, wird eine HTTP-Anfrage an einen externen Webdienst gesendet. Wenn der Webdienst-Herausgeber eine Zulassungsliste in der Firewall des Netzwerks verwendet, in dem sich der externe Webdienst befindet, muss der Herausgeber die unten aufgeführten IP-Adressblöcke zu seiner Zulassungsliste hinzufügen.

**CRM-Synch**

Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} sind Integrationsmechanismen, die ausgehende HTTP-Anfragen an APIs senden, die von Ihrem CRM-Anbieter veröffentlicht werden. Sie müssen sicherstellen, dass Ihre IT-Organisation den Zugriff auf Ihre CRM-Anbieter-APIs nicht durch einen der unten stehenden IP-Adressblöcke blockiert.

**Marketo Engage Ausgehende IP-Adressblöcke**

Die folgenden Tabellen decken alle Marketo Engage-Server ab, die ausgehende Aufrufe durchführen. Verwenden Sie die folgenden Listen, wenn Sie IP-Zulassungslisten, Server, Firewall, Zugriffssteuerungsliste, Sicherheitsgruppe oder Dienste von Drittanbietern konfigurieren, um ausgehende Verbindungen von Marketo Engage zu empfangen.

<table>
 <tbody>
  <tr>
   <th>IP-Block (CIDR-Notation)</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
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
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
 </tbody>
</table>
