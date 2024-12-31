---
description: Richten Sie den Analytics-Abschnitt für Ihre neue Marketo Engage-Instanz ein.
title: Best Practices für neue Instanzen - Analytics-Checkliste
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 1%

---

# Best Practices für neue Instanzen: Analytics-Checkliste {#new-instance-best-practices-analytics-checklist}

Der Abschnitt „Analytics“ bietet globale Berichte, die die Leistung Ihrer Marketing-Maßnahmen analysieren. Erfahren Sie mehr über die erforderlichen Schritte, um darin zu navigieren.

Denken Sie daran[ die Checklisten herunterzuladen ](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) Ihren Fortschritt zu verfolgen.

## Baumstruktur {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organisation: Benennung, Ordner und Archivierung</td>
    <td><li>Verwenden Sie eine Berichtsnamenskonvention, um Berichte auf der Registerkarte Globale Berichte zu unterscheiden.
    <ul><li>Ein Beispiel für eine bewährte Benennungskonvention ist [Berichtstyp] [Global vs. BU-spezifisches Tag] [Berichtsbeschreibung] wie [E-Mail-Leistung]-[Global]-[E-Mail-Interaktion mit 180 Tagen].</li></ul><br>
    <li>Identifizieren Sie Berichte, die für verschiedene Benutzergruppen in Ihrer Organisation (z. B. Vertriebsteam, Marketing-Leiter) freigegeben werden sollten, und organisieren Sie die Berichte nach Ordner im Ordner „Gruppenberichte“ in Analytics for Global Reports.</li> 
    <li>Die Archivierung sollte auf den Ordner „Globale Berichte“ beschränkt sein, da es sich um ständig aktivierte Berichte handelt.   <ul><li>Beschränken Sie die Archivierung auf organisatorische Änderungen, z. B. das Reduzieren oder Hinzufügen relevanter Geschäftseinheiten, wenn Sie Berichte basierend auf einer Geschäftseinheitenstruktur erstellen.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Arbeitsbereiche (falls zutreffend)</td>
    <td><li>Replizieren Sie die globalen Berichte und die Ordnerstruktur in allen Arbeitsbereichen, um ein konsistentes Reporting für Ihre Teams beizubehalten. Diese Berichte befinden sich dann im Ordner Gruppenberichte .</li></td>
  </tr>
  <tr>
    <td>Meine Berichte</td>
    <td><li>Identifizieren und erstellen Sie die Berichte, die zur Verwendung im Abschnitt <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Meine Berichte</a> erforderlich sind. Verwenden Sie diesen Abschnitt zum privaten Bericht als Sandbox für globale Berichte. Sie stehen nur dem Benutzer zur Verfügung, der den Bericht erstellt.</li>
    <li>Verwenden Sie die Namenskonvention Ihres Unternehmens, um den Bericht und die Verwendung zu identifizieren, damit Sie Berichte in „Meine Berichte“ mit Berichten in „Gruppenberichte“ abstimmen können.</li></td>
  </tr>
  <tr>
    <td>Berichte gruppieren</td>
    <td><li>Gruppenberichte sind die globalen Berichte Ihres Unternehmens und sollten einen Bericht über die Gesamtaktivität für Ihr Unternehmen enthalten.</li>
    <li>Erwägen Sie die Erstellung <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank"> (klonfähigen </a>), da Sie erwarten, dass jede Geschäftseinheit am häufigsten verwendet, um den Zeitaufwand für das Abrufen des Berichts zu reduzieren und die Datenkorrektur sicherzustellen. Weitere Informationen finden Sie in der <a href="#global-reports">Tabelle Globale Berichte </a>.
    <ul><li>Personenleistungsbericht (jederzeit und zeitbasiert) nach Quelle, Monat</li>
    <li>Performance-Bericht des Programms (nach Kostenmonat, zeitbasiert)</li>
    <li>E-Mail-Leistungsbericht (zeitbasiert)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Aktivieren Sie „Globale Berichterstellung“</a> auf der Registerkarte „Einrichtung“ des Berichts, um die Daten aus allen Ihren Arbeitsbereichen in die Berichte E-Mail-Leistung und E-Mail-Link-Leistung aufzunehmen. Wenn Sie über mehr als einen Arbeitsbereich verfügen, müssen Sie ihn nur im Standardarbeitsbereich aktivieren.</li>
    <p><img src="assets/tip-icon.png" alt="Notizensymbol"> TIPP: Erstellen Sie die <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Smart List</a> mit den Filtern, die Sie in die meisten Ihrer Berichte in den Datenbankabschnitt aufnehmen möchten. Wenn Sie die Smart-List-Kriterien aktualisieren müssen, können Sie sie an einer Stelle aktualisieren, anstatt sie in allen globalen Berichten zu aktualisieren.</td>
  </tr>
</tbody>
</table>

## Abonnements {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Abonnements</td>
    <td><li>Abstimmung mit Ihrem Marketing-Leiter bezüglich Personen, die die Berichtsergebnisse und deren Kadenz während der Implementierung überprüfen sollten.</li> <li>Verwenden Sie Abonnements, um Daten an Personen in Ihrem Unternehmen zu verteilen, die sie kennen sollten, ohne eine spezifische Benutzerlizenz zu erschöpfen.</li>
    <p><img src="assets/tip-icon.png" alt="Notizensymbol"> TIPP: Wenn Sie möchten, dass Benutzer auf die Echtzeitberichtsdaten zugreifen, müssen Sie sie als Benutzer hinzufügen, damit sie den Bericht anzeigen können.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Richten Sie </a> gewünschten Intervall (täglich/wöchentlich/monatlich) Abonnements für das kontinuierliche Monitoring jedes Teams ein. Sie können <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions"> auch alle Ihre Abonnements an </a> Stelle auf der Registerkarte Abonnements in Analytics anzeigen.</li></td>
  </tr>
</tbody>
</table>

## Globale Berichte {#global-reports}

Identifizieren Sie Berichte, die für verschiedene Benutzergruppen innerhalb Ihrer Organisation (z. B. Vertriebsteam, Marketing-Leiter) freigegeben werden sollten. Erstellen Sie für jedes Team/jede Benutzergruppe/Geschäftseinheit eine geeignete Ordnerstruktur, um die geklonten Berichte in Gruppenberichten zu organisieren. Erwägen Sie die Einrichtung globaler Berichte, z. B.:

<table>
<thead>
  <tr>
    <th style="width:20%">Berichtstyp</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-Mail-Leistungsbericht</td>
    <td><li>Erstellen Sie globale, Workspace-/Geschäftsbereichsweite Berichte mit den richtigen E-Mails.</li>
    <li>Erstellen Sie in allen klonbaren Programmvorlagen einen lokalen E-Mail-Leistungsbericht.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Verwenden Sie einen relevanten Zeitrahmen (</a>. B. bis zum Geschäftsdatum, letzte 90 Tage usw.) für den Bericht, um eine genaue Ansicht der standardmäßigen E-Mail-Interaktions- und Zustellbarkeitsmetriken zu erhalten.</li>
    <p><img src="assets/tip-icon.png" alt="Notizensymbol"> TIPP: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Aktivieren Sie die Filterung der „Bot-Aktivität“ in <strong>Admin &gt; E-Mail</strong></a>, um eine Protokollierung zu vermeiden oder zu ermitteln, ob die Protokollierung für Bot-Aktivitäten aktiviert ist. Schließen Sie den Filter ein, um nur <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Geöffnete/angeklickte Aktivitäten zuzulassen, bei denen in der Smart List Ihrer klonbaren globalen Berichte die Option „Ist Bot-Aktivität“ auf „Falsch</a> beschränkt ist.</td>
  </tr>
  <tr>
    <td>People Performance Report</td>
    <td><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Es wird empfohlen, für jede Marketo Engage<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">Implementierung eine geeignete Kanal- und Tag-</a> zu verwenden, bevor Sie die erworbenen Mitarbeiter und den ROI Ihrer Marketing-Investitionen nach Kanal verfolgen können.
    <p>
    <li>Legen Sie die Kriterien fest, mit denen Sie die Leistung Ihrer Lead-Akquise-Programme messen, und erstellen Sie anhand dieser Metriken zeitbasierte Standardberichte (aktuelles Jahr, Ansicht der letzten rollierenden 12 Monate oder 180 Tage): <ul><li>Akquise-Programm: Marketo Engage-Programm, das für die Akquise der Person angerechnet wird.</li>
    <li>Personen-Source: Die Quellkategorie dafür, wie der Datensatz in Ihrer Datenbank bekannt wurde (basierend auf der Quellliste mit Werten in Ihrem CRM)
    </li></ul>
    <li>Nach Woche oder Monat erstellte Personen messen. Dieser Bericht liefert Ihnen ein Maß für Ihre Datenbankwachstumsrate und gibt an, ob Sie sich Ihrem Datenbankgrößenlimit nähern.</li>
    <li>Filtern Sie die Metriken in Personenleistungsberichten, indem <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report"> Ihre Smart-Listen als benutzerdefinierte Spalten verwenden</a></li>
    <p><img src="assets/tip-icon.png" alt="Notizensymbol"> TIPP: Erstellen Sie in der Datenbank Smart Lists für die benutzerdefinierten Spalten, die Sie anstelle von Marketing-Aktivitäten zum Bericht „Personen-Performance“ hinzufügen möchten, damit Sie den Smart List-Namen richtig und deutlich sehen können, wenn er im Bericht ausgewählt wird.</td>
  </tr>
  <tr>
    <td>Programmvollzugsbericht</td>
    <td><p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Für diesen Bericht müssen Ihre Kanäle, Fortschrittsstatus und Erfolgsschritte unter „Admin<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong> &gt; „Tags</strong> <strong> definiert </strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Messen Sie die Effektivität Ihrer Marketing-Taktiken</a> innerhalb selektiver Programme.</li>
    <li>Verwalten Sie die Programmmitgliedschaft (mithilfe von Smart Campaign, um Akquiseprogramm, Status, Erfolgsstatus zu aktualisieren) entsprechend den Best Practices innerhalb von Marketing-Aktivitäten.</li>
    <li>Maßnahme auf der Grundlage der Kosten für das laufende Jahr und rollierende 12 Monate.
    <ul><li>Denken Sie daran<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program"> dass die Beibehaltung </a>Periodenkosten“ für die Nutzung des Programmleistungsberichts von entscheidender Bedeutung ist.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="Notizensymbol"> TIPP: Um (<a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">) Listen in den Programmleistungsberichten </a> aggregieren und anzuzeigen, stellen Sie sicher, dass Ihre Teams das entsprechende Akquise-Programm für das Tagging auswählen. Erwägen Sie <a href="https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">Erstellen eines Standardprogramms</a> das als Akquise-Programm ausgewählt werden soll, wenn die importierten Listen für keinen Kanal gelten. Dadurch wird sichergestellt, dass jede importierte Person über ein gültiges Akquiseprogramm verfügt, das sich auf die Quelle, die Geschäftseinheit, den Kanal usw. bezieht, und nicht auf einen leeren Wert.</td>
  </tr>
  <tr>
    <td>Bericht zur Leistung der Landingpage</td>
    <td><li>Erstellen Sie den <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Landingpage-Leistungsbericht</a> als globalen Bericht, damit Sie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report"> Anzahl </a> Landingpages für Design Studio-/Marketing-Aktivitäten an einem Ort filtern und überprüfen können.</li>
    <li>Bei Programmen mit Landingpage(s) sollten Sie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">in der Programmvorlage einen dedizierten lokalen Bericht erstellen</a> damit Sie die Leistung auf Programmebene überprüfen können.</li></td>
  </tr>
  <tr>
    <td>Webseitenaktivitätsbericht</td>
    <td><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Nur Web-Seiten (externe und Marketo-Landingpages), auf <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website"> "Munchkin JavaScript</a> aktiviert ist, werden in diesem Bericht verfolgt. Erwägen Sie, den JavaScript-Code in der Tag Management-Plattform zu platzieren, z. B. <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, um zu vermeiden, dass der Code auf jeder Web-Seite hartcodiert wird.
    <p>
    <li>Erstellen Sie den <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Webseitenaktivitätsbericht</a> als globalen Bericht, damit Sie die Anzahl aller Web-Seiten an einem Ort überprüfen können. Beachten Sie, dass Ihre externen Webseiten-Aktivitäten nur in den Web-Seiten-Aktivitätsberichten widergespiegelt werden.</li></td>
  </tr>
</tbody>
</table>

## Lokale Berichte {#local-reports}

Einige Marketo Engage-Berichte werden am besten als lokale Assets innerhalb bestimmter Programme in Marketing-Aktivitäten bereitgestellt, da sie in der Regel in einer eingeschränkteren Reihe von Programmen und Assets verwendet werden. Sie sollten grundlegende Berichte einrichten, z. B.:

<table>
<thead>
  <tr>
    <th style="width:20%">Berichtstyp</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-Mail-Link-Leistungsbericht</td>
    <td><li>Erstellen Sie einen <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">E-Mail-Link-Leistungsbericht</a> innerhalb von Programmen, die E-Mails senden, und Ihrer Dropdown-Kampagnen, um Ihnen Einblicke in die Links zu geben, auf die Personen in Ihren E-Mail-Sendungen klicken.</li></td>
  </tr>
  <tr>
    <td>Bericht zu Kampagnenaktivitäten</td>
    <td><li>Erstellen Sie den <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Kampagnenaktivitätsbericht</a> und wählen Sie einen Zeitraum innerhalb Ihres Betriebsordners unter „Marketing-Aktivitäten“.</li>
    <li>Richten Sie Berichte ein, um die Trigger für jeden Anwendungsfall zu überwachen und <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">Kampagnenfilter anzuwenden</a> (z. B. Trigger bei der Verhaltens-Bewertung, Trigger bei der Lebenszyklusqualifizierung, Trigger bei interessanten Momenten).</li></td>
  </tr>
  <tr>
    <td>Interaktions-Stream-Leistungsbericht (falls zutreffend)</td>
    <td><li>Erstellen Sie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Interaktions-Stream-Leistungsbericht</a> um die Effektivität von Inhalten und Streams zu messen, die in Ihrem Interaktionsprogramm bereitgestellt werden.</li>
    <li>Erwägen Sie die Verwendung des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank"> Filters „Segmentierung“ auf der Registerkarte „Einrichtung</a> des Berichts und die Gruppierung der Berichtsdaten nach <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">Segment</a> (z. B. Personenquelle, Branche), die in Ihrem Interaktionsprogramm verwendet werden. Auf diese Weise erhalten Sie tiefere Einblicke in die Interaktionsmuster der einzelnen Segmente und können strategische Änderungen vornehmen, um Ihr Interaktionsprogramm zu verbessern (Inhalt, Stream, Stream-Kadenz usw.).</li></td>
  </tr>
</tbody>
</table>
