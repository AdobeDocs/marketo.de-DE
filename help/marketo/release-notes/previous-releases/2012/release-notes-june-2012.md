---
unique-page-id: 2951114
description: Versionshinweise - Juni 2012 - Marketo-Dokumentation - Produktdokumentation
title: Versionshinweise - Juni 2012
exl-id: c22eda86-da7a-4c76-9cea-1ce23ff0f3e8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Versionshinweise: Juni 2012 {#release-notes-june}

## Verbesserungen bei der Marketo-Lead-Verwaltung {#marketo-lead-management-enhancements}

### Umbenennen {#rename}

Sie können Smart Lists, statische Listen und Kampagnen umbenennen. Wenn Sie diese Assets in Filtern, Triggern oder Flüssen verwenden, wird der Name auch dort automatisch aktualisiert. Sie konnten Ihre E-Mails, Formulare und Ordner immer umbenennen.

Und als Bonus haben wir die Eingabe und Anzeige von Beschreibungstexten für Assets verbessert.

![](assets/image2014-9-23-10-3a23-3a10.png)

## Feldzuordnung importieren {#import-field-mapping}

Wir haben den Import einer Liste in Marketo erheblich vereinfacht! Während des Importvorgangs können Sie den Namen des Marketo-Felds dem Namen der Spaltenüberschrift in der Importdatei zuordnen. Darüber hinaus können Sie in [!UICONTROL Admin] Aliasnamen einrichten, die dem Feldnamen in Marketo zugeordnet sind, sodass Ihre Benutzerinnen und Benutzer jedes Mal das richtige Feld auswählen.

Wenn Sie weiterhin Felder importieren und zuordnen, speichert Marketo die Zuordnungen und zeigt sie während des Imports an, um die Verwendung zu erleichtern. Und um das Leben noch einfacher zu gestalten, können Sie auf die Kopfzeile Beispielwert klicken, um die verschiedenen Werte anzuzeigen, die in das Feld eingefügt würden. Dadurch wird sichergestellt, dass Sie jedes Mal das richtige Feld zuordnen!

![](assets/image2014-9-23-10-3a23-3a27.png)

## [!UICONTROL Zusammenfassung] Seite für Smart- und statische Listen {#summary-page-for-smart-lists-and-static-lists}

Haben Sie sich schon einmal gefragt, wo Ihre Listen verwendet werden? Oder wer hat die Liste erstellt oder zuletzt geändert? Die neue Zusammenfassungsseite, die für Smart-Listen und statische Listen verfügbar ist, bietet Ihnen diese wichtigen Details.

![](assets/image2014-9-23-10-3a23-3a40.png)

Auf den bestehenden Übersichtsseiten für Programme und Kampagnen wurden das Erstellungsdatum/der Benutzer sowie das Datum/die Benutzerinformationen der letzten Änderung hinzugefügt.

![](assets/image2014-9-23-10-3a23-3a54.png)

## [!UICONTROL Von] für Assets verwendet {#used-by-for-assets}

Wir haben eine neue Registerkarte zu unseren Asset[!UICONTROL Zusammenfassungs-] namens &quot;[!UICONTROL &#x200B; von“ &#x200B;]!

![](assets/image2014-9-23-10-3a24-3a5.png)

Beispiel: [!UICONTROL Verwendet von] für statische Listen

## Gitternetzlinien für Landingpages {#landing-page-gridlines}

Das Hinzufügen von Gitternetzlinien für Einstiegsseiten erleichtert das Ausrichten von Text, Grafiken und Formularen auf der Einstiegsseite erheblich. Schalten Sie sie für jede Landingpage ein und aus und passen Sie auch die Breite zwischen den Zeilen an!

![](assets/image2014-9-23-10-3a24-3a19.png)

![](assets/image2014-9-23-10-3a24-3a33.png)

## Leads durch E-Mails blockiert {#leads-blocked-from-mailings}

Bei der Planung einer Kampagne können Sie auf den Link klicken, um die Liste der Leads anzuzeigen, die vom Versand blockiert sind.

![](assets/image2014-9-23-10-3a24-3a51.png)

## [!UICONTROL Warten] Schritt - Lead-Token und mein Token {#wait-step-lead-token-and-my-token}

In unserer Mai-Version haben wir erweiterte Optionen zum [!UICONTROL Warten]-Flussschritt hinzugefügt. Mit diesen Änderungen können Sie einen Geschäftstag, ein Datum und eine Uhrzeit angeben. In dieser Version haben wir die Möglichkeit hinzugefügt, im Warteschritt ein Token zu verwenden. Beispielsweise können Sie `{{lead.Birthday}}` verwenden, um eine E-Mail an den Geburtstag zu senden, oder `{{my.Event Date}}`, um eine endgültige Webinar-Erinnerung zu senden.

![](assets/image2014-9-23-10-3a25-3a57.png)

## [!UICONTROL Anzeigen] als [!UICONTROL Miniaturansichten] in Design Studio {#view-as-thumbnails-in-design-studio}

Wechseln Sie Ihre Ansicht von einer Bildliste zu einer Miniaturansicht!

![](assets/image2014-9-23-10-3a26-3a13.png)

Hinweis: Ab dieser Version gilt die vorherige Sortierung in Smart-Listen-Rastern nicht mehr für die nächste Smart-Liste, die Sie anzeigen. Wenn Sie beispielsweise eine Smart-Liste nach Firmenname sortieren, wird die nächste Smart-Liste, die in demselben Feld angezeigt wird, nicht automatisch sortiert.

Erinnerung: Aktualisierung des E-Mail-Leistungsberichts läuft!

## Verbesserungen bei der Marketo-Umsatzzyklusanalyse {#marketo-revenue-cycle-analytics-enhancements}

### Neue Metriken in der Programm-Opportunity-Analyse  {#new-metrics-in-program-opportunity-analysis}

Sie können jetzt Einblicke in die durchschnittliche Anzahl der Marketing-Kontakte erhalten, bevor Opportunitys erstellt oder geschlossen werden, sowie in den durchschnittlichen Wert einer Marketing-Berührung.

![](assets/image2014-9-23-10-3a26-3a30.png)

![](assets/image2014-9-23-10-3a26-3a41.png)

## Anzeigen von mehreren Diagrammen {#displaying-multi-charts}

Mit der Funktion für mehrere Diagramme können Sie mehrere Diagramme in einem einzigen Bericht des Umsatzzyklus-Explorers anzeigen. Sie können diese Funktion beispielsweise verwenden, wenn Sie dieselben Daten über verschiedene Monate hinweg anzeigen möchten. Diese Funktion verhindert auch, dass Sie separate Filter und Berichte erstellen müssen.

![](assets/image2014-9-23-10-3a27-3a41.png)

## Diagrammtyp des Wärmenetzes  {#heat-grid-chart-type}

Mit Wärmerastern können Sie Daten visualisieren, um Muster der Marketing-Leistung zu identifizieren. Dieser Visualisierungstyp farbcodiert Ihre Ergebnisse, damit Sie komplexe Geschäftsanalysen in einer leicht verständlichen Visualisierung anzeigen können.

![](assets/image2014-9-23-10-3a28-3a21.png)

## Streudiagrammtyp  {#scatter-chart-type}

Mit Streudiagrammen können Sie Daten für mehrere Dimensionen in einem Diagramm visualisieren. Bei diesem Visualisierungstyp wird basierend auf den verwendeten Attributen eine Sprechblase in einem Diagramm dargestellt. Anschließend können Sie eine Kennzahl verwenden, um die Blase farblich zu kennzeichnen, und/oder eine Kennzahl verwenden, um die Größe der Blase anzugeben.

![](assets/image2014-9-23-10-3a29-3a7.png)
