---
unique-page-id: 10096683
description: Aktualisierungen zur Ereignisregistrierung auf ON24 - Marketo-Dokumente - Produktdokumentation
title: Aktualisierungen der Ereignisregistrierung in ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Aktualisierungen der Ereignisregistrierung in ON24 {#on-event-registration-updates}

>[!IMPORTANT]
>
>Ab August 2022 unterstützt ON24 keine neuen Marketo-Integrationen mehr. Die Informationen in diesem Artikel gelten nur für bestehende Benutzer.

## Manuelles Genehmigen von Registranten {#manually-approving-registrants}

Sie können Ihre Registrierungspflichtigen manuell validieren, bevor Sie ihnen eine Bestätigungs-E-Mail schicken. Dazu müssen Sie Ihre Kampagnen so konfigurieren, dass sie diesen zusätzlichen Schritt handhaben:

1. Für die Registrierungs-Trigger-Kampagne:

   * Setzen Sie in der Smart-Liste den Trigger auf **Formular ausfüllen**.
   * Legen Sie im Fluss den Status in Progression auf **Ausstehende Genehmigung**.

1. Gehen Sie zum Ereignis und klicken Sie auf die Schaltfläche **Mitglieder** Registerkarte. Auf dieser Registerkarte werden alle Personen angezeigt, die das Formular ausgefüllt haben. Ihr Status sollte auf **Ausstehende Genehmigung**.
1. Verwenden Sie den Filter oben im Raster, um nur die Personen mit dem Status **Ausstehende Genehmigung**.
1. Wählen Sie die Personen aus, die Sie registrieren möchten (Umschalt-Klick, Strg-Klick oder Alle auswählen).
1. Klicken Sie im Menü auf **Status ändern**. Auswählen **Angemeldet**, **Zurückgewiesen** oder einen anderen anwendbaren Status.

## Umgang mit Personen mit einem Registrierungsfehler {#handling-people-with-a-registration-error}

Wenn eine Person nicht registriert, sondern auf den Status Registrierfehler gesetzt wird, ist es nicht zu spät, um sich zu erholen.

1. Filtern Sie im Tab Mitglieder die Liste der Personen mit dem Status . **Registrierungsfehler**.
1. Bevor Sie fortfahren, stellen Sie sicher, dass Sie das Problem mit der Integration ermittelt und behoben haben (überprüfen Sie, ob es unter keine Fehler gibt). **Veranstaltungspartner** in Admin).
1. Nachdem das Problem behoben wurde, wählen Sie alle Personen mit dem Status Registrierungsfehler aus und ändern Sie ihren Status in **Angemeldet**. Dadurch wird versucht, sie erneut bei ON24 zu registrieren.

## Aktualisierung des Mitgliederstatus von ON24 {#updating-member-status-from-on}

Marketo ruft die Anwesenheitsinformationen automatisch jeden Abend um ca. 23 Uhr Pacific ab. Um die Teilnehmerinformationen manuell zu aktualisieren, klicken Sie auf **Von Webinar-Anbieter aktualisieren** under **Ereignisaktionen**.

>[!MORELIKETHIS]
>
>[Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
