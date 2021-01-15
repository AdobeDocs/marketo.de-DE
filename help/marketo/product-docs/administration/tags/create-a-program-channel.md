---
unique-page-id: 2950682
description: Erstellen eines Programm-Kanals - Marketing Docs - Produktdokumentation
title: Erstellen eines Programm-Kanals
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---


# Erstellen eines Programm-Kanals {#create-a-program-channel}

Ein Programm ist eine spezifische Marketinginitiative. Der Kanal ist als Versand gedacht, wie Webinar oder Sponsoring oder Online-Anzeige.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Erfahren Sie mehr über [Programm](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), das wichtigste Element in Marketo.

1. Klicken Sie im Abschnitt **Admin** auf **Tags**.

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >Warum Tags? Ein Kanal ist eine Möglichkeit, ein Programm zu beschreiben, genau wie andere Tags. Der Kanal hat nur besondere Besonderheiten.

1. Klicken Sie auf das Symbol **+** neben **Kanal**, um die vorhandenen Kanal zu erweitern und anzuzeigen.

   ![](assets/image2014-9-24-12-3a58-3a33.png)

1. Klicken Sie unter **Neu** auf **Neuer Kanal**.

   ![](assets/image2014-9-24-12-3a58-3a53.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Kanal: Reklametafeln
   >
   >* Anwenden auf: Standard
   >* Progression: Mitglied, Verlobt (im Zweifelsfall funktionieren diese gut)
   >* Erfolg: Engagiert

   >
   >Kanal: Partei
   >
   >* Anwenden auf: Ereignis
   >* Progression: Eingeladen, registriert, Keine Anzeige und Teilnahme
   >* Erfolg: Angezeigt

   >
   >Sehen Sie sich die Progressionen der vorhandenen Kanal an, um eine Vorstellung davon zu erhalten, wie sie verwendet werden.

1. Gehen wir zum Parteitag-Kanal. Benennen Sie Ihren neuen **Kanal** und wählen Sie den Programm-Typ, auf den er angewendet werden soll.

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >Auf was anwenden? Es gibt mehrere Arten von Programmen. Ordnen Sie dem Kanal den richtigen Typ zu. Wählen Sie im Zweifelsfall **Default**.

   >[!NOTE]
   >
   >Bei Verwendung von &quot;Ereignis mit Webinar&quot;werden Systemzuordnungen gesperrt (wie für Webinar-Integrationen erforderlich) und können nicht bearbeitet werden.

   Geben Sie die ersten beiden Programm-Statusnamen ein und klicken Sie dann auf Hinzufügen Schritt.
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. Geben Sie ein anderes Programm **Status** und **Schritt** ein und klicken Sie dann auf **Hinzufügen Schritt**.

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >Die **Step**-Nummer wird zum Sortieren von Programm-Status verwendet. Denken Sie daran, dass die Leute in diesen Schritten nicht rückwärts gehen können. Sie können den Status nur in einen Status mit einem höheren oder gleichen Wert ändern. Verwenden Sie die gleichen Werte, wenn der Status hin- und herschalten soll, anstatt dass eine Progression durchgeführt wird.

1. Geben Sie das letzte Programm **Status** und **Schritt** ein.

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >Bei Verwendung des Typs &quot;Ereignis&quot;ist eine Systemzuordnung für den Status &quot;Registered&quot;, &quot;Warteliste&quot;und &quot;Attended&quot;erforderlich. Daher können diese Status nicht ausgeblendet werden.

1. Wählen Sie für **Registered** den Status des mobilen Check-in **.**

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. Wählen Sie **Mobile Checkin-Status** für **Anwesend**.

   ![](assets/image2014-9-24-15-3a40-3a21.png)

   >[!NOTE]
   >
   >**Mobile Check-in-Status******* Optionen sind nur verfügbar, wenn der Kanal für Ereignis-Programme verwendet wird.

   >[!NOTE]
   >
   >Nur Personen mit einem **Mobile Check-in-Status** von **Registered** und **teilgenommen** werden in [Mobile Check-in-Apps](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md) angezeigt.

   >[!TIP]
   >
   >Wenn eine neue Person in der mobilen Check-in-App erstellt wird, wird sie auf &quot;Registriert&quot;im Ereignis-Programm eingestellt. Wenn eine Person in das Ereignis der App eingecheckt ist, wird sie auf Im Ereignis-Programm teilnehmen eingestellt.

1. Wählen Sie den Programm-Status **success** und klicken Sie dann auf **Create**.

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   Gut gemacht! Wenn Sie ein neues Programm dieses Typs erstellen, wird dieser neue Kanal eine der Möglichkeiten sein.
