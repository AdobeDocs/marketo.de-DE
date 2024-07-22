---
unique-page-id: 2950682
description: Erstellen eines Programmkanals - Marketo Docs - Produktdokumentation
title: Erstellen eines Programmkanals
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Erstellen eines Programmkanals {#create-a-program-channel}

Ein Programm ist eine spezifische Marketinginitiative. Der Kanal ist als Bereitstellungsmechanismus gedacht, z. B. Webinar, Sponsoring oder Online-Anzeige.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Erfahren Sie mehr über [programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), das wichtigste Element in Marketo.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-a-program-channel-1.png)

1. Klicken Sie auf **[!UICONTROL Tags]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Warum Tags? Ein Kanal ist eine Möglichkeit, ein Programm wie andere Tags zu beschreiben. Der Kanal verfügt nur über spezielle zusätzliche Funktionen.

1. Klicken Sie auf das Symbol **+** neben [!UICONTROL Kanal] , um die vorhandenen Kanäle zu erweitern und anzuzeigen.

   ![](assets/create-a-program-channel-3.png)

1. Klicken Sie unter **[!UICONTROL Neu]** auf **[!UICONTROL Neuer Kanal]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Kanal: Reklametafeln
   >
   >* Anwenden auf: Standard
   >* Progression: Mitglied, engagiert (im Zweifelsfall funktionieren diese gut)
   >* Erfolg: Interagiert
   >
   >Kanal: Party
   >
   >* Anwenden auf: Ereignis
   >* Progression: Eingeladen, Registriert, Keine Anzeige und Teilnahme
   >* Erfolg: Teilnehmer
   >
   >Sehen Sie sich die Progressionen vorhandener Kanäle an, um eine Vorstellung davon zu erhalten, wie sie verwendet werden.

1. Gehen wir zum Beispiel zum Parteitakanal. Benennen Sie den neuen Kanal **Kanal** und wählen Sie den Programmtyp aus, auf den er angewendet werden soll.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Auf was anwenden? Es gibt mehrere Arten von Programmen. Ordnen Sie den Kanal dem richtigen Typ zu. Wählen Sie im Zweifelsfall **[!UICONTROL Standard]**.

   >[!NOTE]
   >
   >Bei Verwendung von &quot;[!UICONTROL Ereignis mit Webinar]&quot; werden Systemzuordnungen gesperrt (wie für Webinar-Integrationen erforderlich) und können nicht bearbeitet werden.

1. Geben Sie die ersten beiden Programmstatusnamen ein und klicken Sie dann auf **[!UICONTROL Schritt hinzufügen]**.

   ![](assets/create-a-program-channel-6.png)

1. Geben Sie ein weiteres Programm ein, **[!UICONTROL Status]** und **[!UICONTROL Schritt]**, und klicken Sie dann auf **[!UICONTROL Schritt hinzufügen]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >Die Nummer **[!UICONTROL Schritt]** wird zum Sortieren der Programmstatus verwendet. Denken Sie daran, dass die Menschen in diesen Fortschrittsschritten nicht rückwärts gehen können. Sie können nur den Status in einen höheren oder gleichen Wert ändern. Verwenden Sie die gleichen Werte, wenn Status anstelle eines Fortschritts hin- und herwechseln sollen.

1. Geben Sie das letzte Programm **[!UICONTROL Status]** und die Nummer **[!UICONTROL Schritt]** ein.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Bei Verwendung des Typs &quot;[!UICONTROL Ereignis]&quot; ist eine Systemzuordnung für den Status &quot;Registered&quot;, &quot;Waitlisted&quot;und &quot;Attended&quot;erforderlich. Daher können diese Status nicht ausgeblendet werden.

1. Wählen Sie den **[!UICONTROL Mobile Check-in Status]** für **[!UICONTROL Registered]** aus.

   ![](assets/create-a-program-channel-9.png)

1. Wählen Sie den **[!UICONTROL Mobile Check-in Status]** für **[!UICONTROL Teilnehmer]** aus.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL Mobile Check-in Status]** -Optionen sind nur verfügbar, wenn der Kanal für Ereignisprogramme verwendet wird.

   >[!NOTE]
   >
   >In den [Mobile Check-in Apps](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md) werden nur Personen mit dem Status **[!UICONTROL Mobile Check-in]** von **[!UICONTROL Registered]** und **[!UICONTROL teilgenommen]** angezeigt.

   >[!TIP]
   >
   >Wenn eine neue Person in der Mobile Check-in-App erstellt wird, wird sie im Ereignisprogramm auf Registered gesetzt. Wenn eine Person in das Ereignis in der App eingecheckt wird, wird sie im Ereignisprogramm auf &quot;Teilnehmer&quot;gesetzt.

1. Wählen Sie den Programmstatus **[!UICONTROL Erfolg]** aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-program-channel-11.png)

   Schön gemacht! Wenn Sie ein neues Programm dieses Typs erstellen, ist dieser neue Kanal eine der Möglichkeiten.
