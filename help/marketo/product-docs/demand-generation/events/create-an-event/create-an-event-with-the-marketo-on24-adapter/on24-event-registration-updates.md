---
unique-page-id: 10096683
description: Aktualisierungen bei der ON24-Ereignisregistrierung - Marketo-Dokumente - Produktdokumentation
title: Aktualisierungen zur ON24-Ereignisregistrierung
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Aktualisierungen zur ON24-Ereignisregistrierung {#on-event-registration-updates}

## Registranten manuell genehmigen {#manually-approving-registrants}

Sie können die Registrierenden manuell genehmigen, bevor Sie ihnen eine Bestätigungs-E-Mail senden. Dazu müssen Sie Ihre Kampagnen so konfigurieren, dass sie mit diesem zusätzlichen Schritt umgehen:

1. Für die Kampagne „Registrierungs-Trigger&quot;:

   * Legen Sie in der Smart-Liste den Trigger auf **Formular ausfüllen** fest.
   * Legen Sie im Fluss den Status In Bearbeitung auf **Ausstehende Genehmigung** fest.

1. Gehen Sie zur Veranstaltung und klicken Sie auf die **Mitglieder** Registerkarte. Auf dieser Registerkarte werden alle Personen angezeigt, die das Formular ausgefüllt haben. Ihr Status sollte auf „Ausstehende **&quot; gesetzt**.
1. Verwenden Sie den Filter oben im Raster, um nur die Personen mit dem Status **Genehmigung ausstehend** anzuzeigen.
1. Wählen Sie die Personen aus, die Sie registrieren möchten (Umschalt-Klick, Strg-Klick oder Alle auswählen).
1. Klicken Sie im Menü auf **Status**. Wählen Sie **Registriert**, **Abgelehnt** oder einen anderen anwendbaren Status aus.

## Umgang mit Personen mit einem Registrierungsfehler {#handling-people-with-a-registration-error}

Wenn eine Person am Ende nicht registriert wird, sondern auf den Status „Registrierungsfehler“ gesetzt wird, ist es noch nicht zu spät, um ihn wiederherzustellen.

1. Filtern Sie auf der Registerkarte Mitglieder die Liste der Personen mit dem Status **Registrierungsfehler**.
1. Bevor Sie fortfahren, stellen Sie sicher, dass Sie das Problem mit der -Integration ermittelt und behoben haben (stellen Sie sicher, dass unter **Ereignispartner** in Admin keine Fehler auftreten).
1. Nachdem das Problem behoben wurde, wählen Sie alle Personen mit dem Status Registrierungsfehler aus und ändern Sie ihren Status in **Registriert**. Dadurch wird versucht, sie erneut bei ON24 zu registrieren.

## Mitgliedsstatus von ON24 aktualisieren {#updating-member-status-from-on}

Marketo ruft die Anwesenheitsdaten automatisch jeden Abend um ca. 23.00 Uhr Pacific ab. Um die Informationen zur Teilnahme manuell zu aktualisieren, klicken Sie **Vom Webinar-Anbieter aktualisieren** unter &quot;**&quot;**.

>[!MORELIKETHIS]
>
>[Informationen zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
