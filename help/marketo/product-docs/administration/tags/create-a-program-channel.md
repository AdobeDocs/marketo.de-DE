---
unique-page-id: 2950682
description: Erstellen eines Programmkanals - Marketo Docs - Produktdokumentation
title: Erstellen eines Programmkanals
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Erstellen eines Programmkanals {#create-a-program-channel}

Ein Programm ist eine spezifische Marketinginitiative. Der Kanal ist als Bereitstellungsmechanismus gedacht, z. B. Webinar, Sponsoring oder Online-Anzeige.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Weitere Informationen [Programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), das wichtigste Element in Marketo.

1. Unter dem **Admin** Abschnitt, klicken Sie auf **Tags**.

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >Warum Tags? Ein Kanal ist eine Möglichkeit, ein Programm wie andere Tags zu beschreiben. Der Kanal verfügt nur über spezielle zusätzliche Funktionen.

1. Klicken Sie auf **+** neben **Kanal** um vorhandene Kanäle zu erweitern und anzuzeigen.

   ![](assets/image2014-9-24-12-3a58-3a33.png)

1. under **Neu** klicken **Neuer Kanal**.

   ![](assets/image2014-9-24-12-3a58-3a53.png)

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

1. Gehen wir zum Parteitakanal-Beispiel. Benennen Sie Ihre neue **Kanal** und wählen Sie den Programmtyp aus, auf den sie angewendet werden soll.

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >Auf was anwenden? Es gibt mehrere Arten von Programmen. Ordnen Sie den Kanal dem richtigen Typ zu. Wählen Sie im Zweifelsfall **Standard**.

   >[!NOTE]
   >
   >Bei Verwendung von &quot;Ereignis mit Webinar&quot;werden Systemzuordnungen gesperrt (wie für Webinar-Integrationen erforderlich) und können nicht bearbeitet werden.

   Geben Sie die ersten beiden Programmstatusnamen ein und klicken Sie dann auf Schritt hinzufügen .
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. Andere Programme eingeben **Status** und **Schritt** number und klicken Sie auf **Schritt hinzufügen**.

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >Die **Schritt** -Zahl wird zum Sortieren des Programmstatus verwendet. Denken Sie daran, dass die Menschen in diesen Fortschrittsschritten nicht rückwärts gehen können. Sie können nur den Status in einen höheren oder gleichen Wert ändern. Verwenden Sie die gleichen Werte, wenn Status anstelle eines Fortschritts hin- und herwechseln sollen.

1. Letztes Programm eingeben **Status** und **Schritt** Zahl.

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >Bei Verwendung des Typs &quot;Ereignis&quot;ist eine Systemzuordnung für den Status Registered, Waitlisted und Attended erforderlich. Daher können diese Status nicht ausgeblendet werden.

1. Wählen Sie die **Mobile-Check-in-Status** für **Angemeldet**.

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. Wählen Sie die **Mobile-Check-in-Status** für **Angemeldet**.

   ![](assets/image2014-9-24-15-3a40-3a21.png)

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

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   Gut gemacht! Wenn Sie ein neues Programm dieses Typs erstellen, ist dieser neue Kanal eine der Möglichkeiten.
