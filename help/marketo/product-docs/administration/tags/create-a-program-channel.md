---
unique-page-id: 2950682
description: Erstellen eines Programmkanals - Marketo Docs - Produktdokumentation
title: Erstellen eines Programmkanals
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
source-git-commit: 48c2d1deea84ee747ecc2453e770ad33dd49f578
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---

# Erstellen eines Programmkanals {#create-a-program-channel}

Ein Programm ist eine spezifische Marketinginitiative. Der Kanal ist als Bereitstellungsmechanismus gedacht, z. B. Webinar, Sponsoring oder Online-Anzeige.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Weitere Informationen [Programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), das wichtigste Element in Marketo.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/create-a-program-channel-1.png)

1. Klicken **Tags**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Warum Tags? Ein Kanal ist eine Möglichkeit, ein Programm wie andere Tags zu beschreiben. Der Kanal verfügt nur über spezielle zusätzliche Funktionen.

1. Klicken Sie auf **+** neben **Kanal** um vorhandene Kanäle zu erweitern und anzuzeigen.

   ![](assets/create-a-program-channel-3.png)

1. under **Neu** klicken **Neuer Kanal**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Kanal: Reklametafeln
   >
   >* Anwenden auf: Standard
   >* Progression: Mitglied, Verlobt (im Zweifelsfall funktionieren diese gut)
   >* Erfolg: Interagiert

   >
   >Kanal: Partei
   >
   >* Anwenden auf: Ereignis
   >* Progression: Eingeladen, registriert, Keine Sendung und Teilnahme
   >* Erfolg: Angemeldet

   >
   >Sehen Sie sich die Progressionen vorhandener Kanäle an, um eine Vorstellung davon zu erhalten, wie sie verwendet werden.

1. Gehen wir zum Beispiel zum Parteitakanal. Benennen Sie Ihre neue **Kanal** und wählen Sie den Programmtyp aus, auf den sie angewendet werden soll.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Auf was anwenden? Es gibt mehrere Arten von Programmen. Ordnen Sie den Kanal dem richtigen Typ zu. Wählen Sie im Zweifelsfall **Standard**.

   >[!NOTE]
   >
   >Bei Verwendung von &quot;Ereignis mit Webinar&quot;werden Systemzuordnungen gesperrt (wie für Webinar-Integrationen erforderlich) und können nicht bearbeitet werden.

1. Geben Sie die ersten beiden Programmstatusnamen ein und klicken Sie auf **Schritt hinzufügen**.

   ![](assets/create-a-program-channel-6.png)

1. Andere Programme eingeben **Status** und **Schritt** number und klicken Sie auf **Schritt hinzufügen**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >Die **Schritt** -Zahl wird zum Sortieren des Programmstatus verwendet. Denken Sie daran, dass die Menschen in diesen Fortschrittsschritten nicht rückwärts gehen können. Sie können nur den Status in einen höheren oder gleichen Wert ändern. Verwenden Sie die gleichen Werte, wenn Status anstelle eines Fortschritts hin- und herwechseln sollen.

1. Letztes Programm eingeben **Status** und **Schritt** Zahl.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Bei Verwendung des Typs &quot;Ereignis&quot;ist eine Systemzuordnung für den Status Registered, Waitlisted und Attended erforderlich. Daher können diese Status nicht ausgeblendet werden.

1. Wählen Sie die **Mobile-Check-in-Status** für **Angemeldet**.

   ![](assets/create-a-program-channel-9.png)

1. Wählen Sie die **Mobile-Check-in-Status** für **Angemeldet**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**Mobile-Check-in-Status**** **Optionen sind nur verfügbar, wenn der Kanal für Veranstaltungsprogramme vorgesehen ist.

   >[!NOTE]
   >
   >Nur Personen mit **Mobile-Check-in-Status** von **Angemeldet** und **Angemeldet** wird im [Mobile Check-in-Apps](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Wenn eine neue Person in der Mobile Check-in-App erstellt wird, wird sie im Ereignisprogramm auf Registered gesetzt. Wenn eine Person in das Ereignis in der App eingecheckt wird, wird sie im Ereignisprogramm auf &quot;Teilnehmer&quot;gesetzt.

1. Wählen Sie die **Erfolg** Programmstatus, und klicken Sie auf **Erstellen**.

   ![](assets/create-a-program-channel-11.png)

   Gut gemacht! Wenn Sie ein neues Programm dieses Typs erstellen, ist dieser neue Kanal eine der Möglichkeiten.
