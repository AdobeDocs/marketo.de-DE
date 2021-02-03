---
unique-page-id: 10096683
description: ON24 Ereignis Registration Updates - Marketing Docs - Produktdokumentation
title: ON24-Ereignis-Registrierungsaktualisierungen
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# ON24 Ereignis Registrierungs-Updates {#on-event-registration-updates}

## Manuelles Genehmigen von Registranten {#manually-approving-registrants}

Sie können Ihre Registrierungspflichtigen manuell genehmigen, bevor Sie ihnen eine Bestätigungs-E-Mail senden. Dazu müssen Sie Ihre Kampagnen so konfigurieren, dass sie diesen zusätzlichen Schritt handhaben:

1. Für die Kampagne zum Trigger registrieren:

   * Legen Sie in der Smart-Liste den Trigger auf **Ausfüllbares Formular** fest.
   * Stellen Sie im Fluss den Status in Progression auf **Ausstehende Genehmigung** ein.

1. Gehen Sie zum Ereignis und klicken Sie auf die Registerkarte **Members**. Auf dieser Registerkarte werden alle Personen angezeigt, die das Formular ausgefüllt haben. Ihr Status sollte auf **Ausstehende Genehmigung** eingestellt werden.
1. Verwenden Sie den Filter oben im Raster, um nur die Personen mit dem Status **Ausstehende Genehmigung** Ansicht.
1. Wählen Sie die Personen aus, die Sie registrieren möchten (Umschalt-Klick, Strg-Klick oder Alle auswählen).
1. Klicken Sie im Menü auf **Status ändern**. Wählen Sie **Registered**, **Abgelehnt** oder einen anderen anwendbaren Status.

## Umgang mit Personen mit einem Registrierungsfehler {#handling-people-with-a-registration-error}

Wenn eine Person nicht registriert, sondern stattdessen auf den Status Registrierungsfehler gesetzt wird, ist es nicht zu spät, um sich zu erholen.

1. Filtern Sie auf der Registerkarte Mitglieder die Liste der Personen mit dem Status **Registrierungsfehler**.
1. Bevor Sie fortfahren, stellen Sie sicher, dass Sie das Integrationsproblem festgestellt und behoben haben (überprüfen Sie, ob unter **Ereignis-Partner** in Admin keine Fehler auftreten).
1. Nachdem das Problem behoben wurde, wählen Sie alle Personen mit dem Status &quot;Registrierungsfehler&quot;aus und ändern Sie ihren Status in **Registered**. Dadurch wird versucht, sie erneut bei ON24 zu registrieren.

## Mitgliederstatus von ON24 {#updating-member-status-from-on} aktualisieren

Marketo holt die Anwesenheitsinformationen automatisch um ca. 23.00 Uhr Pazifik pro Nacht ein. Um die Anwesenheitsinformationen manuell zu aktualisieren, klicken Sie unter **Ereignis-Aktionen** auf **Von Webinar-Anbieter aktualisieren**.

>[!MORELIKETHIS]
>
>[Ereignisse des Marketo ON24-Adapters](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
