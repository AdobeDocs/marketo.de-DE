---
description: Richten Sie den Analytics-Abschnitt für Ihre neue Marketo Engage-Instanz ein.
title: Best Practices für neue Instanzen - Checkliste für Analytics
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 1%

---

# Best Practices für neue Instanzen: Analytics-Checkliste {#new-instance-best-practices-analytics-checklist}

Der Abschnitt Analytics bietet globale Berichte, die die Leistung Ihrer Marketing-Maßnahmen analysieren. Erfahren Sie mehr über die erforderlichen Schritte zur Navigation.

Denken Sie daran, [die Checklisten herunterzuladen](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) und Ihren Fortschritt zu verfolgen.

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
    <td><li>Unterscheiden Sie Berichte auf der Registerkarte Globale Berichte anhand einer Namenskonvention für Berichte.
    <ul><li>Ein Beispiel für eine gute Namensgebungskonvention ist [Berichtstyp] [Global vs. BU-spezifisches Tag] [Berichtsbeschreibung] wie [E-Mail-Leistung]-[Global]-[180 Tage E-Mail-Interaktion].</li></ul><br>
    <li>Identifizieren Sie Berichte, die für verschiedene Benutzergruppen in Ihrer Organisation freigegeben werden sollen (z. B. Verkaufsteam, Marketingleitung), und organisieren Sie die Berichte nach Ordner im Ordner Gruppenberichte in Analytics für globale Berichte.</li> 
    <li>Die Archivierung sollte auf den Ordner Globale Berichte beschränkt werden, da es sich hierbei immer um Berichte handelt.   <ul><li>Beschränken Sie die Archivierung auf organisatorische Änderungen, z. B. die Reduzierung oder das Hinzufügen relevanter Geschäftseinheiten, wenn Sie Berichte auf der Grundlage einer Geschäftsbereichsstruktur erstellen.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Arbeitsbereiche (falls zutreffend)</td>
    <td><li>Replizieren Sie die globalen Berichte und die Ordnerstruktur über Arbeitsbereiche hinweg, um eine konsistente Berichterstellung für Ihre Teams zu gewährleisten. Diese Berichte befinden sich im Ordner Gruppenberichte .</li></td>
  </tr>
  <tr>
    <td>Meine Berichte</td>
    <td><li>Identifizieren und erstellen Sie die Berichte, die zur Verwendung im Abschnitt <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Meine Berichte</a> erforderlich sind. Verwenden Sie diesen privaten Berichtsabschnitt als Ihre Sandbox für globale Berichte. Sie stehen nur dem Benutzer zur Verfügung, der den Bericht erstellt.</li>
    <li>Verwenden Sie die Namenskonvention Ihres Unternehmens, um den Bericht und die Verwendung zu identifizieren, damit Sie Berichte in Meine Berichte mit Berichten in Gruppenberichten abstimmen können.</li></td>
  </tr>
  <tr>
    <td>Berichte gruppieren</td>
    <td><li>Gruppenberichte sind die globalen Berichte Ihres Unternehmens und sollten einen Bericht über die Gesamtaktivität für Ihr Unternehmen erstellen.</li>
    <li>Erwägen Sie die Erstellung von <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">klonbaren Core-Berichten</a>, da Sie davon ausgehen, dass jede Geschäftseinheit die meiste Zeit verwendet, um die zum Abrufen des Berichts erforderliche Zeit zu verkürzen und die Datenkorrektur sicherzustellen. Siehe Details in der Tabelle <a href="#global-reports">Globale Berichte unter </a>.
    <ul><li>Personen-Leistungsbericht (alle- und zeitbasiert) nach Quelle, Monat</li>
    <li>Bericht zur Programmleistung (nach Kostenmonat, zeitbasiert)</li>
    <li>E-Mail-Leistungsbericht (zeitbasiert)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Aktivieren Sie "Globale Berichterstellung"</a> auf der Registerkarte "Einrichtung"des Berichts, um die Daten aus allen Ihren Arbeitsbereichen in die Berichte "E-Mail-Leistung"und "E-Mail-Link-Leistung"aufzunehmen. Wenn Sie mehr als einen Arbeitsbereich haben, müssen Sie ihn nur im Standardarbeitsbereich aktivieren.</li>
    <p><img src="assets/tip-icon.png" alt="Notizsymbol"> TIPP: Erstellen Sie die <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Smart-Liste</a> mit den Filtern, die Sie in die meisten Ihrer Berichte im Abschnitt Datenbank aufnehmen möchten. Wenn Sie die Kriterien der intelligenten Liste aktualisieren müssen, können Sie sie an einem Ort aktualisieren, anstatt sie in allen globalen Berichten zu aktualisieren.</td>
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
    <td><li>Fragen Sie bei Ihrem Marketing-Verantwortlichen nach Personen, die die Berichtsergebnisse und deren Kadenz während der Implementierung überprüfen sollten.</li> <li>Verwenden Sie Abonnements, um Daten an Personen zu verteilen, die in Ihrem Unternehmen Kenntnisse benötigen, ohne eine spezifische Benutzerlizenz zu erschöpfen.</li>
    <p><img src="assets/tip-icon.png" alt="Notizsymbol"> TIPP: Wenn Sie möchten, dass Benutzer auf die Echtzeitberichtsdaten zugreifen können, müssen Sie sie als Benutzer hinzufügen, damit sie den Bericht anzeigen können.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Richten Sie Abonnements ein</a> in der gewünschten Kadenz (täglich/wöchentlich/monatlich) für die laufende Überwachung durch jedes Team. Sie können auch <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">all Ihre Abonnements</a> an einer Stelle auf der Registerkarte "Abonnements"in Analytics anzeigen.</li></td>
  </tr>
</tbody>
</table>

## Globale Berichte {#global-reports}

Ermitteln Sie Berichte, die für verschiedene Benutzergruppen in Ihrer Organisation freigegeben werden sollen (z. B. Verkaufsteam, Marketingleitung). Erstellen Sie für jedes Team/jede Benutzergruppe/jeden Geschäftsbereich eine geeignete Ordnerstruktur, um die geklonten Berichte in Gruppenberichten zu organisieren. Ziehen Sie die Einrichtung globaler Berichte in Erwägung, z. B.:

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
    <td><li>Erstellen Sie globale Berichte für Workspace/Geschäftseinheiten mit den richtigen E-Mails.</li>
    <li>Erstellen Sie einen lokalen E-Mail-Leistungsbericht in allen Ihren klonierbaren Programmvorlagen.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Verwenden Sie einen relevanten Zeitrahmen</a> (z. B. YTD, letzte 90 Tage usw.) für den Bericht, um eine genaue Ansicht der standardmäßigen E-Mail-Interaktions- und Zustellbarkeitsmetriken bereitzustellen.</li>
    <p><img src="assets/tip-icon.png" alt="Notizsymbol"> TIPP: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Schalten Sie die Filterung "Bot Activity"in <strong>Admin &gt; E-Mail</strong></a> ein, um die Protokollierung zu vermeiden oder festzustellen, ob die Protokollierung für Bot-Aktivitäten aktiviert ist. Schließen Sie den Filter so ein, dass nur geöffnete/angeklickte Aktivitäten mit der Beschränkung "Is Bot Activity"auf "False"</a> in der Smart-Liste Ihrer klonbaren globalen Berichte zugelassen werden.<a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860"></td>
  </tr>
  <tr>
    <td>Personenleistungsbericht</td>
    <td><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Es wird empfohlen, für jede Marketo Engage-Implementierung über eine geeignete <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">Kanal- und Tag-Strategie</a> zu verfügen, bevor Sie die erworbenen Personen und den ROI Ihrer Marketinginvestitionen nach Kanal verfolgen können.
    <p>
    <li>Legen Sie die Kriterien fest, anhand derer Sie die Leistung Ihrer Lead-Akquiseprogramme messen, und erstellen Sie anhand dieser Metriken zeitbasierte (aktuelle, letzte rollierende 12-Monats-Ansicht oder 180-Tage-Berichte) Standardberichte: <ul><li>Akquise-Programm: Marketo Engage-Programm, das für die Akquise der Person gutgeschrieben wird.</li>
    <li>Person Source: Die Quellkategorie, aus der hervorgeht, wie der Datensatz Ihrer Datenbank bekannt wurde (basierend auf der Werteliste in Ihrem CRM-System)
    </li></ul>
    <li>Messen Sie nach Woche oder Monat erstellte Personen. Dieser Bericht liefert Ihnen einen Messwert zur Wachstumsrate Ihrer Datenbank und darüber, ob Sie sich Ihrer Datenbankgrößenbegrenzung nähern.</li>
    <li>Filtern Sie die Metriken in "People Performance Reports"nach <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">unter Verwendung Ihrer Smart-Listen als benutzerdefinierte Spalten.</a></li>
    <p><img src="assets/tip-icon.png" alt="Notizsymbol"> TIPP: Erstellen Sie Smart-Listen für die benutzerdefinierten Spalten, die Sie zum Bericht zur Leistung von Personen in der Datenbank hinzufügen möchten, anstelle von Marketing-Aktivitäten, damit Sie den Namen der Smart-Liste richtig und deutlich sehen können, wenn er im Bericht ausgewählt wird.</td>
  </tr>
  <tr>
    <td>Bericht zur Programmleistung</td>
    <td><p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Für diesen Bericht müssen Sie über Ihre Kanäle, Statusangaben und Erfolgsschritte verfügen, die unter <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Admin</strong> &gt; <strong>Tags</strong></a> definiert sind.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Messen Sie die Effektivität Ihrer Marketing-Taktiken</a> in ausgewählten Programmen.</li>
    <li>Verwalten Sie die Programmmitgliedschaft (mithilfe von Smart-Kampagnen, um das Akquiseprogramm, den Status, den Erfolgsstatus zu aktualisieren) gemäß den Best Practices in Marketing-Aktivitäten.</li>
    <li>Maßnahme auf der Grundlage der Kosten für das laufende Jahr und für die laufenden 12 Monate.
    <ul><li>Beachten Sie, dass die Aufrechterhaltung der <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Period Costs</a> für die Nutzung des Programmleistungsberichts von entscheidender Bedeutung ist.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="Notizsymbol"> TIPP: Um alle <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">importierten Listen</a> in den Programmleistungsberichten zu aggregieren und anzuzeigen, stellen Sie sicher, dass Ihre Teams das entsprechende Akquiseprogramm für das Tagging auswählen. Erwägen Sie die <a href="https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs"> Erstellung eines Standardprogramms</a> , das als Akquiseprogramm ausgewählt werden soll, wenn die importierten Listen für keinen Kanal gelten. Dadurch wird sichergestellt, dass jede importierte Person über ein gültiges Akquiseprogramm, das sich auf Quelle, Geschäftseinheit, Kanal usw. bezieht, anstatt über einen leeren Wert verfügt.</td>
  </tr>
  <tr>
    <td>Landingpage-Leistungsbericht</td>
    <td><li>Erstellen Sie den <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Leistungsbericht für Einstiegsseiten</a> als globalen Bericht, damit Sie die Zahlen <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report"> aller Einstiegsseiten von Design Studio-/Marketingaktivitäten filtern und überprüfen können.</a></li>
    <li>Bei Programmen mit Landingpage(s) sollten Sie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">einen dedizierten lokalen Bericht in der Programmvorlage erstellen</a>, damit Sie die Leistung auf Programmebene überprüfen können.</li></td>
  </tr>
  <tr>
    <td>Webseitenaktivitätsbericht</td>
    <td><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: In diesem Bericht werden nur Webseiten (externe und Marketo-Landingpages) verfolgt, für die <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">die Munchkin JavaScript</a> aktiviert ist. Erwägen Sie die Platzierung des JavaScript-Codes in der Tag Management-Plattform, z. B. <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, um eine Hartkodierung des Codes auf jeder Webseite zu vermeiden.
    <p>
    <li>Erstellen Sie den Bericht <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Web-Seitenaktivität</a> als globalen Bericht, damit Sie die Anzahl aller Webseiten an einem Ort überprüfen können. Beachten Sie, dass Ihre externen Webseiten-Aktivitäten nur in den Berichten zur Web-Seitenaktivität angezeigt werden.</li></td>
  </tr>
</tbody>
</table>

## Lokale Berichte {#local-reports}

Einige Marketo Engage-Berichte eignen sich am besten als lokale Assets innerhalb bestimmter Programme in Marketingaktivitäten, da ihre typische Verwendung in einer begrenzteren Anzahl von Programmen und Assets erfolgt. Erwägen Sie die Einrichtung grundlegender Berichte, z. B.:

<table>
<thead>
  <tr>
    <th style="width:20%">Berichtstyp</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Leistungsbericht von E-Mail-Links</td>
    <td><li>Erstellen Sie einen <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">E-Mail-Link-Leistungsbericht</a> in Programmen, die E-Mails senden, und Ihren Drip-Kampagnen, um Einblicke in die Links zu erhalten, auf die Benutzer in E-Mail-Sendungen klicken.</li></td>
  </tr>
  <tr>
    <td>Bericht zur Kampagnenaktivität</td>
    <td><li>Erstellen Sie den Bericht <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Kampagnenaktivität</a> und wählen Sie einen Zeitraum innerhalb Ihres Ordners für die operative Aktivität in Marketingaktivitäten aus.</li>
    <li>Richten Sie Berichte ein, um die Trigger für jeden Anwendungsfall zu überwachen und <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">Kampagnenfilter anwenden</a> (z. B. Trigger zur Verhaltensscoring, Trigger zur Lebenszyklusqualifizierung, Trigger zu interessanten Momenten).</li></td>
  </tr>
  <tr>
    <td>Interaktions-Stream-Leistungsbericht (falls zutreffend)</td>
    <td><li>Erstellen Sie einen <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Interaktions-Stream-Leistungsbericht</a> , um die Effektivität von Inhalten und Streams zu messen, die innerhalb Ihres Interaktionsprogramms bereitgestellt werden.</li>
    <li>Erwägen Sie die Verwendung des Filters "<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank"> Segmentierung"auf der Registerkarte "Einrichtung"des Berichts</a> und gruppieren Sie die Berichtsdaten nach dem in Ihrem Interaktionsprogramm verwendeten <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">Segment</a> (z. B. Personenquelle, Branche). Auf diese Weise erhalten Sie tiefere Einblicke in die Interaktionsmuster der einzelnen Segmente und können so strategische Änderungen vornehmen, um Ihr Interaktionsprogramm zu verbessern (Inhalt, Stream, Stream-Kadenz usw.).</li></td>
  </tr>
</tbody>
</table>
