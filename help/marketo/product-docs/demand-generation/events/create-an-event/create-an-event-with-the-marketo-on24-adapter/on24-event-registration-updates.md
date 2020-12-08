---
unique-page-id: 10096683
description: ON24 Ereignis Registration Updates - Marketing Docs - Produktdokumentation
title: ON24-Ereignis-Registrierungsaktualisierungen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---


# ON24-Ereignis-Registrierungsaktualisierungen {#on-event-registration-updates}

## Manuelles Genehmigen von Registranten {#manually-approving-registrants}

Sie können Ihre Registrierungspflichtigen manuell genehmigen, bevor Sie ihnen eine Bestätigungs-E-Mail senden. Dazu müssen Sie Ihre Kampagnen so konfigurieren, dass sie diesen zusätzlichen Schritt handhaben:

1. Kampagne zum Registrierungsauslöser:

   * Legen Sie in der intelligenten Liste als Auslöser das **Ausfüllen des Formulars** fest.
   * Legen Sie im Fluss den Status in Progression auf **Ausstehende Genehmigung** fest.

1. Gehen Sie zum Ereignis und klicken Sie auf die Registerkarte **Mitglieder** . Auf dieser Registerkarte werden alle Personen angezeigt, die das Formular ausgefüllt haben. Ihr Status sollte auf **Ausstehende Genehmigung** eingestellt werden.
1. Verwenden Sie den Filter oben im Raster, um nur die Personen mit dem Status **Ausstehende Genehmigung** Ansicht.
1. Wählen Sie die Personen aus, die Sie registrieren möchten (Umschalt-Klick, Strg-Klick oder Alle auswählen).
1. Klicken Sie im Menü auf Status **ändern**. Wählen Sie **Registrierter**, **Abgelehnt** oder einen anderen anwendbaren Status.

## Umgang mit Personen mit einem Registrierungsfehler {#handling-people-with-a-registration-error}

Wenn eine Person nicht registriert, sondern stattdessen auf den Status Registrierungsfehler gesetzt wird, ist es nicht zu spät, um sich zu erholen.

1. Filtern Sie auf der Registerkarte Mitglieder die Liste der Personen mit dem Status **Registrierungsfehler**.
1. Bevor Sie fortfahren, stellen Sie sicher, dass Sie das Integrationsproblem festgestellt und behoben haben (überprüfen Sie, ob unter &quot; **Ereignis-Partner** in Admin&quot;keine Fehler auftreten).
1. Nachdem das Problem behoben wurde, wählen Sie alle Personen mit dem Status &quot;Registrierungsfehler&quot;aus und ändern Sie ihren Status in &quot; **Registriert**&quot;. Dadurch wird versucht, sie erneut bei ON24 zu registrieren.

## Aktualisierung des Mitgliederstatus von ON24 {#updating-member-status-from-on}

Marketo holt die Anwesenheitsinformationen automatisch um ca. 23.00 Uhr Pazifik pro Nacht ein. Um die Anwesenheitsinformationen manuell zu aktualisieren, klicken Sie unter &quot; **Ereignis-Aktionen&quot;auf &quot;Von Webinar-Anbieter** **aktualisieren&quot;**.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Ereignisse des Marketo ON24-Adapters](understanding-marketo-on24-adapter-events.md)

>



