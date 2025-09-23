---
unique-page-id: 4720433
description: Konfigurieren von Protokollen für Marketo Engage - Marketo Engage-Dokumente - Produktdokumentation
title: Konfigurieren von Protokollen für Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 9%

---

# Konfigurieren von Protokollen für Marketo Engage{#configure-protocols-for-marketo-engage}

Auf die Zulassungsliste setzen Wenn Sie oder Ihr Unternehmen restriktive Firewall- oder Proxy-Server-Einstellungen verwenden, müssen Sie bzw. Ihr Netzwerkadministrator möglicherweise bestimmte Domains und IP-Adressbereiche ändern, um sicherzustellen, dass Adobe Marketo Engage erwartungsgemäß funktioniert.

Wenn Sie Hilfe bei der Implementierung der folgenden Protokolle benötigen, teilen Sie diesen Artikel bitte mit Ihrer IT-Abteilung. Wenn der Web-Zugriff mithilfe einer -Zulassungsliste eingeschränkt wird, stellen Sie sicher, dass die folgenden Domains (einschließlich des Sternchens) hinzugefügt werden, um alle Marketo Engage-Ressourcen und -Websockets zuzulassen:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Schritt 1: DNS-Einträge für Landingpages und E-Mails erstellen {#step-create-dns-records-for-landing-pages-and-email}

**Tracking-Link-CNAMEs**

Ihr Marketing-Team hätte Ihnen zwei Anfragen für neue CNAME-Einträge senden sollen. Der erste gilt für Landingpage-URLs, damit die Landingpages in URLs angezeigt werden, die Ihre Domain widerspiegeln, und nicht in Marketo Engage (der eigentliche Host). Der zweite betrifft Tracking-Links, die in den von Marketo Engage gesendeten E-Mails enthalten sind.

`1` **CNAME für Landingpages hinzufügen**

Fügen Sie den Landingpage-CNAME, den sie Ihnen gesendet haben, zu Ihrem DNS-Eintrag hinzu, sodass `[YourLandingPageCNAME]` auf die eindeutige Kontozeichenfolge verweist, die Ihren Marketo Engage-Landingpages zugewiesen ist. Melden Sie sich bei der Website Ihrer Domain-Registrierungsstelle an und geben Sie den CNAME der Landingpage und die Kontozeichenfolge ein. Normalerweise umfasst dies drei Felder:

* Alias: `[YourLandingPageCNAME]` eingeben (bereitgestellt von Marketing)
* Typ: CNAME
* Point to: Enter `[MunchkinID].mktoweb.com` (provided by marketing)

`2` **CNAME für E-Mail-Tracking-Links hinzufügen**

Fügen Sie die von CNAME-Marketing gesendete E-Mail hinzu, sodass `[YourEmailCNAME]` auf [MktoTrackingLink], den von Marketo Engage zugewiesenen Standard-Tracking-Link, im folgenden Format verweist:
`[YourEmailCNAME].[YourDomain].com` IN CNAME-`[MktoTrackingLink]`

Beispiel:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` muss die Standard-Branding-Domain sein.

`3` **Benachrichtigen Sie Ihr Marketing-Team**

Benachrichtigen Sie Ihr Marketing-Team, wenn Sie diesen Prozess abgeschlossen haben.

`4` **Wenden Sie sich an den [Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}Support, um mit der Bereitstellung eines SSL-Zertifikats zu beginnen.**

Dieser Vorgang kann bis zu 3 Werktage dauern.

## Auf die Zulassungsliste setzen Schritt 2: Marketo Engages der IPs {#step-allowlist-marketo-ips}

Wenn Ihre Marketing-Gruppe Marketo Engage zum Senden von Test-E-Mails verwendet (eine Best Practice vor dem Senden von E-Mail-Blasts), werden die Test-E-Mails manchmal von Anti-Spam-Systemen blockiert, die auf Absender-IP-Adressen angewiesen sind, um die Gültigkeit der E-Mail zu überprüfen. Um sicherzustellen, dass diese Test-E-Mails ankommen, fügen Sie Ihrer Marketo Engages auf die Zulassungsliste setzen hinzu.

Auf die Zulassungsliste setzen Fügen Sie diese IP-Adressen zu Ihrer Unternehmensadresse hinzu:

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Einige Anti-Spam-Systeme verwenden für die Zulassungsauflistung das Feld E-Mail-Rückgabepfad anstelle der IP-Adresse. In diesen Fällen ist der beste Ansatz die Zulassungsliste von &quot;&#42;.mktomail.com“, da Marketo Engage mehrere Postfach-Subdomains verwendet. Andere Anti-Spam-Systeme werden anhand der Absenderadresse auf die Zulassungsliste gesetzt. In diesen Fällen müssen Sie alle Versand- („Von„) Domains einbeziehen, die Ihre Marketing-Gruppe für die Kommunikation mit Personen/Leads verwendet.

>[!NOTE]
>
>Postini verwendet eine einzigartige Technologie und erfordert die Zulassungsauflistung von IP-Bereichen. Siehe [Zulassungsauflistung mit Postini](https://nation.marketo.com/docs/DOC-1066).

## Schritt 3: Einrichten von SPF und DKIM {#step-set-up-spf-and-dkim}

Ihr Marketing-Team hätte Ihnen auch Informationen zu DKIM (Domain Keys Identified Mail) senden sollen, die Ihrem DNS-Ressourceneintrag (auch unten aufgeführt) hinzugefügt werden sollen. Führen Sie die Schritte aus, um DKIM und SPF (Sender Policy Framework) erfolgreich zu konfigurieren, und benachrichtigen Sie dann Ihr Marketing-Team, dass dies aktualisiert wurde.

1. Fügen Sie den DNS-Einträgen die folgende Zeile hinzu, um SPF einzurichten:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
Include: mktomail.com ~all

   Wenn wir bereits einen SPF-Eintrag in unserem DNS-Eintrag haben, fügen Sie einfach Folgendes hinzu:
Einschließen: mktomail.com

   Ersetzen Sie CompanyDomain durch die Haupt-Domain Ihrer Website (z.B.: &quot;`(company.com/)`„) und CorpIP durch die IP-Adresse Ihres Unternehmens-E-Mail-Servers (z.B. &quot;255.255.255.255„) Wenn Sie E-Mails von mehreren Domains über Marketo Engage senden möchten, sollten Ihre IT-Mitarbeiter diese Zeile für jede Domain hinzufügen (in einer Zeile).

1. Erstellen Sie für DKIM DNS-Ressourceneinträge für jede Domain, die wir einrichten möchten. Nachfolgend finden Sie die Host-Einträge und TXT-Werte für jede Domain, die wir signieren werden:

   `[DKIMDomain1]`: Der Host-Eintrag lautet `[HostRecord1]` und der TXT-Wert `[TXTValue1]`.

   `[DKIMDomain2]`: Der Host-Eintrag lautet `[HostRecord2]` und der TXT-Wert `[TXTValue2]`.

   Kopieren Sie den HostRecord und den TXTValue für jede DKIMDomain, die Sie eingerichtet haben, nachdem Sie die [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"} befolgt haben. Vergessen Sie nicht, jede Domain unter Admin > E-Mail > DKIM zu überprüfen, nachdem Ihr IT-Personal diesen Schritt abgeschlossen hat.

## Schritt 4: Einrichten von DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance - Domain-basierte Nachrichtenauthentifizierung, Berichterstellung und Konformität) ist ein Authentifizierungsprotokoll, das Unternehmen dabei hilft, ihre Domain vor unbefugter Verwendung zu schützen. DMARC erweitert die bestehenden Authentifizierungsprotokolle wie SPF und DKIM, um Empfängerserver darüber zu informieren, welche Aktionen sie ausführen sollten, wenn bei der Authentifizierung auf ihrer Domain ein Fehler auftritt. Obwohl DMARC derzeit optional ist, wird dies dringend empfohlen, da es die Marke und den Ruf Ihres Unternehmens besser schützt. Wichtige Anbieter wie Google und Yahoo werden ab Februar 2024 die Verwendung von DMARC für Massenversender erfordern.

Damit DMARC funktioniert, müssen Sie über mindestens einen der folgenden DNS-TXT-Einträge verfügen:

* Einen gültigen SPF-Eintrag
* Ein gültiger DKIM-Eintrag für Ihre VON-Domain: (empfohlen für Marketo Engage)

Darüber hinaus müssen Sie über einen DMARC-spezifischen DNS-TXT-Eintrag für Ihre FROM: -Domain verfügen. Optional kann eine E-Mail-Adresse Ihrer Wahl definiert werden, um anzugeben, wohin DMARC-Berichte innerhalb Ihres Unternehmens gehen sollen, damit Sie Berichte überwachen können.

Als Best Practice wird empfohlen, die DMARC-Implementierung langsam einzuführen, indem Sie Ihre DMARC-Richtlinie von p=none nach p=Quarantäne oder p=Ablehnen eskalieren, um Einblick in die potenziellen Auswirkungen von DMARC zu erhalten, und Ihre DMARC-Richtlinie auf eine entspannte Ausrichtung auf SPF und DKIM einstellen.

### Beispiel für einen DMARC-Workflow {#dmarc-example-workflow}

1. Wenn Sie für den Empfang von DMARC-Berichten konfiguriert sind, sollten Sie die folgenden Schritte ausführen…

   I. Analysieren Sie das Feedback und die Berichte, die Sie erhalten und verwenden (p=none). Dadurch wird der Empfänger angewiesen, keine Aktionen gegen Nachrichten durchzuführen, bei denen die Authentifizierung fehlschlägt, aber dennoch E-Mail-Berichte an den Absender zu senden.

   II. Überprüfen und beheben Sie Probleme mit SPF/DKIM, wenn die Authentifizierung für legitime Nachrichten fehlschlägt.

   III. Prüfen Sie, ob SPF oder DKIM entsprechend abgestimmt sind und die Authentifizierungsprüfung für alle legitimen E-Mails bestehen.

   IV. Überprüfen Sie Berichte, um sicherzustellen, dass die Ergebnisse den Erwartungen entsprechen, die Sie basierend auf Ihren SPF-/DKIM-Richtlinien haben.

1. Passen Sie dann die Richtlinie entsprechend an (p=Quarantäne). Dadurch wird der empfangende E-Mail-Server angewiesen, E-Mails mit fehlgeschlagener Authentifizierung unter Quarantäne zu stellen (dies bedeutet in der Regel, dass diese Nachrichten im Spam-Ordner abgelegt werden müssen).

   I. Überprüfen Sie die Berichte, um sicherzustellen, dass die Ergebnisse Ihren Erwartungen entsprechen.

1. Wenn Sie mit dem Verhalten von Nachrichten auf der Ebene p=Quarantäne zufrieden sind, können Sie die Richtlinie an (p=Ablehnen) anpassen. Die p=Ablehnungsrichtlinie weist den Empfänger an, jede E-Mail für die Domain, bei der die Authentifizierung fehlschlägt, vollständig abzulehnen (Bounce). Wenn diese Richtlinie aktiviert ist, haben nur E-Mails, die zu 100 % von Ihrer Domain authentifiziert wurden, überhaupt eine Chance auf die Platzierung im Posteingang.

>[!CAUTION]
>
>Verwenden Sie diese Richtlinie mit Vorsicht und ermitteln Sie, ob sie für Ihre Organisation geeignet ist.

### DMARC-Berichte {#dmarc-reporting}

DMARC bietet die Möglichkeit, Berichte zu E-Mails zu erhalten, bei denen SPF/DKIM fehlschlägt. Es gibt zwei verschiedene Berichte, die von ISP-Services im Rahmen des Authentifizierungsprozesses generiert werden und die Absender über die RUA/RUF-Tags in ihrer DMARC-Richtlinie erhalten können.

* Aggregierte Berichte (RUA): enthalten keine personenbezogenen Daten (Personally Identifiable Information), die für die DSGVO (Datenschutz-Grundverordnung) relevant wären.

* Forensische Berichte (RUF): Enthält E-Mail-Adressen, die DSGVO-sensibel sind. Vor der Nutzung von sollten Sie sich intern erkundigen, wie Sie mit Informationen umgehen, die die DSGVO einhalten müssen.

Diese Berichte dienen hauptsächlich dazu, einen Überblick über die E-Mails mit Spoofing-Versuchen zu erhalten. Hierbei handelt es sich um hochtechnische Berichte, die am besten über ein Tool eines Drittanbieters verdaut werden können.

### Beispiel für DMARC-Einträge {#example-dmarc-records}

* Bare Minimum Record: `v=DMARC1; p=none`

* Datensatz, der an eine E-Mail-Adresse weitergeleitet wird, um Berichte zu erhalten: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC-Tags und ihre Funktionen {#dmarc-tags-and-what-they-do}

DMARC-Datensätze enthalten mehrere Komponenten, die als DMARC-Tags bezeichnet werden. Jedes Tag hat einen Wert, der einen bestimmten Aspekt von DMARC festlegt.

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
    <td>Dieses DMARC-Tag gibt die Version an. Es gibt derzeit nur eine Version, daher hat diese einen festen Wert von v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Erforderlich</td>
    <td>Zeigt die ausgewählte DMARC-Richtlinie an und leitet den Empfänger zu Berichten, Quarantänen oder Ablehnungen von E-Mails um, die bei Authentifizierungsprüfungen fehlschlagen.</td>
    <td>p=Keine, Quarantäne oder Zurückweisung</td>
    <td>–</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Optional</td>
    <td>Ermöglicht der oder dem Domain-Verantwortlichen das Festlegen von Berichtsoptionen.</td>
    <td>0: Generieren eines Berichts, wenn alles fehlschlägt
    <br>1: Generieren eines Berichts, wenn etwas fehlschlägt
    <br>d: Generieren eines Berichts, wenn DKIM fehlschlägt
    <br>s: Bericht generieren, wenn SPF fehlschlägt</td>
    <td>1 (empfohlen für DMARC-Berichte)</td>
  </tr>
  <tr>
    <td>PCT</td>
    <td>Optional</td>
    <td>Gibt den Prozentsatz der Nachrichten an, die gefiltert werden sollen.</td>
    <td>PCT=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>Rua</td>
    <td>Optional (empfohlen)</td>
    <td>Gibt an, wo aggregierte Berichte bereitgestellt werden.</td>
    <td>RUA=mailto:aggrep@example.com</td>
    <td>–</td>
  </tr>
  <tr>
    <td>Ruf</td>
    <td>Optional (empfohlen)</td>
    <td>Gibt an, wo forensische Berichte bereitgestellt werden.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>–</td>
  </tr>
  <tr>
    <td>SP</td>
    <td>Optional</td>
    <td>Gibt eine DMARC-Richtlinie für Subdomains der übergeordneten Domain an.</td>
    <td>SP=Zurückweisung</td>
    <td>–</td>
  </tr>
  <tr>
    <td>Adkim</td>
    <td>Optional</td>
    <td>Kann entweder Streng (s) oder Relaxed ® sein. Eine entspannte Ausrichtung bedeutet, dass die in der DKIM-Signatur verwendete Domain eine Subdomain der „Von“-Adresse sein kann. Strenge Ausrichtung bedeutet, dass die in der DKIM-Signatur verwendete Domain genau mit der in der Absenderadresse verwendeten Domain übereinstimmen muss.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>ASPF</td>
    <td>Optional</td>
    <td>Kann entweder Streng (s) oder Relaxed ® sein. Eine entspannte Ausrichtung bedeutet, dass die Domain „ReturnPath“ eine Subdomain der Absenderadresse sein kann. Strenge Ausrichtung bedeutet, dass die Domain des Rücksendepfads exakt mit der Absenderadresse übereinstimmen muss.</td>
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

* DKIM-abgestimmte DMARC - Zum Einrichten von DKIM-abgestimmter DMARC müssen Sie Folgendes tun:

   * Richten Sie DKIM für die Von-Domain Ihrer Nachricht ein. Verwenden Sie die Anweisungen [in diesem Artikel](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Konfigurieren Sie DMARC für die zuvor konfigurierte Domain „FROM:/DKIM&quot;

* DMARC-abgestimmte SPF - Um DMARC-abgestimmte SPF über den gebrandeten Rückgabepfad einzurichten, müssen Sie:

   * Einrichten einer markenspezifischen Rückgabepfad-Domain
      * Konfigurieren des entsprechenden SPF-Eintrags
      * Ändern Sie den MX-Eintrag so, dass er auf den Standard-MX für das Rechenzentrum verweist, von dem Ihre E-Mail gesendet werden soll.

   * Konfigurieren von DMARC für die gebrandete Rückgabepfad-Domain

* Wenn Sie E-Mails von Marketo Engage über eine dedizierte IP-Adresse senden und den gebrandeten Rückgabepfad noch nicht implementiert haben oder nicht sicher sind, ob Sie dies haben, eröffnen Sie bitte ein Ticket beim [Adobe-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Wenn Sie E-Mails von Marketo Engage über einen freigegebenen IP-Pool senden, können Sie durch [hier ](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"} sehen, ob Sie sich für vertrauenswürdige IPs qualifizieren. Der gebrandete Rückgabepfad wird denjenigen kostenlos angeboten, die von vertrauenswürdigen Marketo Engage-IPs senden. Wenden Sie sich bei Genehmigung für dieses Programm an den Adobe-Support, um einen gebrandeten Rückgabepfad einzurichten.

   * Vertrauenswürdige IPs: Ein freigegebener IP-Pool, der Benutzern mit einem geringeren Volumen vorbehalten ist, die weniger als 75 KB/Monat senden und sich nicht für eine dedizierte IP qualifizieren. Diese Benutzenden müssen auch die Best-Practice-Anforderungen erfüllen.

* Wenn Sie E-Mails von Marketo Engage über freigegebene IPs senden und sich nicht für vertrauenswürdige IPs qualifizieren und monatlich mehr als 100.000 Nachrichten senden, müssen Sie sich an das Adobe Account Team (Ihren Account Manager) wenden, um eine dedizierte IP zu erwerben.

* Eine strikte SPF-Ausrichtung wird in Marketo Engage weder unterstützt noch empfohlen.

## Schritt 5: Richten Sie MX-Einträge für Ihre Domain ein {#step-set-up-mx-records-for-your-domain}

Ein MX-Eintrag ermöglicht es Ihnen, E-Mails über die Domain zu empfangen, von der aus Sie E-Mails senden, um Antworten und Abwesenheitsnachrichten zu verarbeiten. Wenn Sie von Ihrer Unternehmens-Domain aus senden, haben Sie dies wahrscheinlich bereits konfiguriert. Andernfalls können Sie ihn für gewöhnlich so einrichten, dass er dem MX-Eintrag Ihrer Unternehmens-Domain zugeordnet wird.

## Ausgehende IP-Adressen {#outbound-ip-addresses}

Eine ausgehende Verbindung wird von Marketo Engage zu einem Server im Internet in Ihrem Namen hergestellt. Einige Partner/Anbieter, mit denen Sie zusammenarbeiten, oder Ihre eigene IT-Organisation können Zulassungslisten verwenden, um den Zugriff auf Server zu beschränken. In diesem Fall müssen Sie ihnen die Blöcke ausgehender Marketo Engage-IP-Adressen bereitstellen, damit sie sie ihren Zulassungslisten hinzufügen können.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} sind ein ausgehender Integrationsmechanismus. Wenn eine [Aufruf-Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"}-Flussaktion als Teil einer Smart-Kampagne ausgeführt wird, wird eine HTTP-Anfrage an einen externen Webservice gesendet. Wenn der Herausgeber des Webservices eine Zulassungsliste in der Firewall des Netzwerks verwendet, in dem sich der externe Webservice befindet, muss der Herausgeber die unten aufgeführten IP-Adressblöcke zu seiner Zulassungsliste hinzufügen.

**CRM-Synchronisation**

Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} und [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} sind Integrationsmechanismen, die ausgehende HTTP-Anfragen an APIs senden, die von Ihrem CRM-Anbieter veröffentlicht wurden. Sie müssen sicherstellen, dass Ihre IT-Organisation keinen der unten aufgeführten IP-Adressblöcke vom Zugriff auf Ihre CRM-APIs blockiert.

**Ausgehende IP-Adressblöcke in Marketo Engage**

Die folgenden Tabellen decken alle Marketo Engage-Server ab, die ausgehende Aufrufe ausführen. Verwenden Sie die folgenden Listen, wenn Sie eine IP-Zulassungsliste, einen Server, eine Firewall, eine Zugriffssteuerungsliste, eine Sicherheitsgruppe oder einen Drittanbieterdienst konfigurieren, um ausgehende Verbindungen von Marketo Engage zu erhalten.

<table>
 <tbody>
  <tr>
   <th>IP-Block (CIDR-Notation)</th>
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
