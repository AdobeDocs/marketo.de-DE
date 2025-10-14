---
description: GenAI-Funktionen - Marketo-Dokumente - Produktdokumentation
title: GenAI-Funktionen
feature: Interactive Webinars
exl-id: 3e0a41b0-7ff3-4676-bafc-4e7a0725a737
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---

# GenAI-Funktionen {#gen-ai-features}

Automatische Generierung von Kapiteln und Zusammenfassungen für aufgezeichnete Webinare, wodurch die Zugänglichkeit verbessert und die Navigation für Ihre Zielgruppe erleichtert werden.

* **Automatische Kapitelgenerierung**: KI-gestützte Technologie erstellt Kapitel für Ihre Webinar-Inhalte.

* **KI-generierte Zusammenfassung**: Erhalten Sie eine automatisierte Textzusammenfassung Ihres Webinars.

* **Bearbeitbare Inhalte**: Ändern Sie die generierten Kapitel und Zusammenfassungen bei Bedarf mithilfe von manuellen und KI-gestützten Bearbeitungsfunktionen.

* **Einfache Integration**: Fügen Sie Ihren Landingpages mühelos Kapitel und Zusammenfassungen hinzu, indem Sie den HTML-Code in den gewünschten Web-Seiten-Editor kopieren.

## GenAI aktivieren {#enable-genai}

>[!PREREQUISITES]
>
>Bevor Sie diese Funktionen verwenden können, müssen Sie zunächst die Adobe GenAI-Nutzungsbedingungen akzeptieren. Falls Sie dies noch nicht getan haben, wenden Sie sich bitte an das Adobe Account Team (Ihren Account Manager), um weitere Informationen zu erhalten.

Nachdem Sie die Adobe GenAI-Nutzungsbedingungen akzeptiert haben, müssen Sie sie für einzelne Benutzer aktivieren. Gehen Sie dazu zu **[!UICONTROL Admin]** > **[!UICONTROL Interaktive Webinare]** und wählen Sie aus, welche Benutzer Zugriff auf GenAI haben sollen.

![](assets/gen-ai-features-1.png){width="800" zoomable="yes"}

## Zugriff {#how-to-access}

1. Navigieren Sie zur Seite „Webinar-Übersicht“ in Interaktive Webinare in Marketo Engage.

1. Warten Sie nach der Durchführung Ihres On-Demand-Webinars 30 bis 60 Minuten, bis die KI Ihre Aufzeichnung verarbeitet hat. Die Schaltfläche Generieren wird anklickbar, sobald sie verfügbar ist.

1. Klicken Sie **[!UICONTROL GenAI-Inhalt anzeigen]**.

   ![](assets/gen-ai-features-2.png){width="800" zoomable="yes"}

1. Eine neue Registerkarte wird geöffnet, auf der KI-generierte Kapitel und eine Textzusammenfassung angezeigt werden.

## Erzeugten Inhalt bearbeiten {#edit-generated-content}

1. Überprüfen der generierten Kapitel und der Zusammenfassung.

1. Wenn Änderungen erforderlich sind, klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten]**.

   Vornehmen von Änderungen:

   * Bearbeiten Sie den Text in der Zusammenfassung und/oder den Kapiteltiteln.

   * Passen Sie bei Bedarf Zeitstempel an, indem Sie die Werte in den Zeitstempelfeldern bearbeiten.

   * Löschen Sie unerwünschte Kapitel, indem Sie sie auswählen und auf **[!UICONTROL Löschen]** klicken.

   * Führen Sie zwei aufeinander folgende Kapitel zusammen, indem Sie sie auswählen und auf **[!UICONTROL Zusammenführen]** klicken.

      * AI generiert ein zusammengesetztes Kapitel, das aus den beiden ausgewählten Kapiteln besteht

      * Um mehrere Kapitel zusammenzuführen, müssen Sie zwei gleichzeitig durchführen

     ![](assets/gen-ai-features-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* Bei Bedarf können Sie die Qualität der generierten Kapitel/Zusammenfassungen mit den Symbolen __ Daumen hoch![&#x200B; &#x200B;](assets/icon-thumbs-up.png) oder _Daumen runter_![Daumen runter](assets/icon-thumbs-down.png) bewerten. Sie können auch alle problematischen Inhalte markieren, indem Sie auf das Markierungssymbol (![) &#x200B;](assets/icon-flag.png).
   >
   >* Wenn Sie mit der ursprünglichen Zusammenfassung nicht zufrieden sind, können Sie auf die Schaltfläche **[!UICONTROL Zusammenfassung neu erstellen]** klicken, und es wird eine andere Version generiert.

1. Speichern Sie Ihre Änderungen, indem Sie auf **[!UICONTROL Speichern]** oben rechts auf dem Bildschirm klicken.

## Verwenden generierter Inhalte {#use-generated-content}

Nachdem Sie den gewünschten Inhalt kopiert haben, fügen Sie ihn in den Editor Ihrer Wahl (z. B. den Marketo Engage-Landingpage-Editor) ein und nehmen Sie die gewünschten Anpassungen vor.

### Zusammenfassung {#summary}

**HTML kopieren** - Klicken Sie auf die Schaltfläche **[!UICONTROL HTML kopieren]**, um den gesamten Text abzurufen, wobei der HTML-Code ihn in einer Tabelle formatieren muss.

**Nur Text** - Wenn Sie nur den Text kopieren möchten, markieren Sie ihn einfach und klicken Sie bei gedrückter Strg-/Befehlstaste+C mit der rechten Maustaste darauf.

### Kapitel {#chapters}

**HTML kopieren** - Klicken Sie auf die Schaltfläche **[!UICONTROL HTML kopieren]**, um die Aufzeichnung und ihre Kapitel in einem Videoplayer zu formatieren.

## Zielgruppe auswählen

Nutzen Sie intelligente Kampagnen-/Listenfilter und/oder Trigger, um zu sehen, was jeder Betrachter gesehen hat, wie oft es war usw., was personalisierte Folgemaßnahmen ermöglicht.

![](assets/gen-ai-features-4.png){width="800" zoomable="yes"}

* **Trigger**: _Klicks auf Link auf Webseite_, _Besuche Webseite_

* **Filter**: _auf Link auf Webseite geklickt_, _besuchte Webseite_

Der „Link“ ist der Name des Kapitels und die „Web-Seite“ ist die Seite, auf der Ihr On-Demand-Webinar gehostet wird.

>[!TIP]
>
>Verwenden Sie [Beschränkungen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} um Ihre Zielgruppe weiter einzuengen.

## Zu beachtende Punkte {#things-to-note}

* Das Löschen oder Zusammenführen von Kapiteln wirkt sich nur auf den Kapitelstapel aus, nicht auf den Videoinhalt selbst. Diese Aktionen sind dauerhaft.

* Die GenAI-Funktionen sind flexibel und können mit verschiedenen Web-Seiten-Editoren verwendet werden, nicht nur mit denen in Marketo Engage.

* Zeigen Sie Ihre Änderungen immer in der Vorschau an, um die gewünschte Funktionalität und das gewünschte Erscheinungsbild sicherzustellen.

* Durch Löschen des Webinars werden auch die GenAI-Inhalte gelöscht.

* Wenn Sie den GenAI-Inhalt löschen möchten, ohne das Webinar zu löschen, wenden Sie sich an das Adobe Account Team (Ihren Account Manager) oder senden Sie eine Anfrage zur Datenlöschung an: `marketo-webinar-genai-alerts@adobe.com`.
