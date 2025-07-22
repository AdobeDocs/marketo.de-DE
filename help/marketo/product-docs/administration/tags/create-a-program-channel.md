---
unique-page-id: 2950682
description: Erstellen eines Programmkanals - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines Programmkanals
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Erstellen eines Programmkanals {#create-a-program-channel}

Ein Programm ist eine spezifische Marketing-Initiative. Der Kanal ist als Bereitstellungsmechanismus gedacht, z. B. Webinar, Sponsoring oder Online-Anzeige.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Erfahren Sie mehr über [Programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), das wichtigste Element in Marketo.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-a-program-channel-1.png)

1. Klicken Sie auf **[!UICONTROL Tags]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Warum Tags? Ein Kanal ist eine Möglichkeit, ein Programm zu beschreiben, genau wie andere Tags. Der Kanal hat nur besondere Extras.

1. Klicken Sie auf das Pluszeichen **+** neben [!UICONTROL Kanal], um vorhandene Kanäle zu erweitern und anzuzeigen.

   ![](assets/create-a-program-channel-3.png)

1. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Neuer Kanal]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Kanal: Billboard
   >
   >* Anwenden auf: Standard
   >* Fortschritt: Mitglied, Interagiert (im Zweifel funktionieren diese einwandfrei)
   >* Erfolg: Interagiert
   >
   >Kanal: Party
   >
   >* Anwenden auf: Ereignis
   >* Fortschritt: Eingeladen, registriert, keine Sendung und Teilgenommen
   >* Erfolgreich: Teilgenommen
   >
   >Sehen Sie sich die Progressionen vorhandener Kanäle an, um eine Vorstellung davon zu erhalten, wie sie verwendet werden können.

1. Nehmen wir das Beispiel des Partykanals. Benennen Sie Ihren neuen **[!UICONTROL Kanal]** und wählen Sie den Programmtyp aus, für den er gelten soll.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Auf was anwenden? Es gibt verschiedene Arten von Programmen. Passen Sie den Kanal dem richtigen Typ an. Wählen Sie im Zweifelsfall &quot;**[!UICONTROL &quot;]**.

   >[!NOTE]
   >
   >Bei Verwendung von [!UICONTROL Ereignis mit Webinar] werden Systemzuordnungen gesperrt (wie es für Webinar-Integrationen erforderlich ist) und können nicht bearbeitet werden.

1. Geben Sie die ersten beiden Programmstatusnamen ein und klicken Sie dann auf **[!UICONTROL Schritt hinzufügen]**.

   ![](assets/create-a-program-channel-6.png)

1. Geben Sie ein anderes Programm **[!UICONTROL Status]** und **[!UICONTROL Schritt]** ein und klicken Sie dann auf **[!UICONTROL Schritt hinzufügen]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >Die **[!UICONTROL Schritt]**-Nummer wird zum Sortieren der Programmstatus verwendet. Denken Sie daran, dass Menschen bei diesen Fortschrittsschritten nicht rückwärts gehen können. Sie können nur den Status in einen höheren oder gleichwertigen Status ändern. Verwenden Sie die gleichen Werte, wenn Status hin- und herwechseln sollen, anstatt einer Progression.

1. Geben Sie das letzte Programm **[!UICONTROL Status]** und **[!UICONTROL Step]** Number ein.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Bei Verwendung des Typs &quot;[!UICONTROL Ereignis]&quot; ist eine Systemzuordnung für den Status „Registriert“, „Auf der Warteliste“ und „Teilgenommen“ erforderlich. Daher können diese Status nicht ausgeblendet werden.

1. Wählen Sie den **[!UICONTROL Mobile Check-in Status]** für **[!UICONTROL Registriert]**.

   ![](assets/create-a-program-channel-9.png)

1. Wählen Sie den **[!UICONTROL Mobile Check-in Status]** für **[!UICONTROL Attended]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL Mobile Check-in Status]** Optionen sind nur verfügbar, wenn der Kanal für Ereignisprogramme ist.

   >[!NOTE]
   >
   >Nur Personen mit dem **[!UICONTROL „Mobile Check]** in Status **[!UICONTROL von Registriert]** und **[!UICONTROL Teilgenommen]** werden in den [Mobile Check-in Apps](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md) angezeigt.

   >[!TIP]
   >
   >Wenn eine neue Person in der mobilen Check-in-App erstellt wird, wird sie im Veranstaltungsprogramm auf [!UICONTROL Registriert] gesetzt. Wenn eine Person in die Veranstaltung in der App eingecheckt wird, wird sie im Veranstaltungsprogramm auf [!UICONTROL Teilgenommen] gesetzt.

1. Wählen Sie den **[!UICONTROL Erfolg]** Programmstatus aus und klicken Sie dann auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-program-channel-11.png)

   Gut gemacht! Wenn Sie ein neues Programm dieses Typs erstellen, wird dieser neue Kanal eine der Optionen sein.
