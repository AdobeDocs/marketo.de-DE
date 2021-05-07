---
unique-page-id: 11378869
description: Erstellen einer SMS-Nachricht für Vibes - Marketo Docs - Produktdokumentation
title: Erstellen einer Vibes-SMS-Nachricht
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
translation-type: tm+mt
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 3%

---

# Erstellen einer Vibes-SMS-Nachricht {#create-a-vibes-sms-message}

So erstellen Sie eine SMS-Nachricht für Vibes:

>[!AVAILABILITY]
>
>Diese Funktion ist als Add-On für Ihr Adobe Marketo Engage-Konto verfügbar. Damit sie ordnungsgemäß bereitgestellt werden kann, muss sie über Adobe erworben werden. Weitere Informationen erhalten Sie von Ihrem Adobe Customer Success Manager.

>[!NOTE]
>
>SMS-Textnachrichten sind nicht HIPAA-konform.

1. Gehen Sie zu **Marketing-Aktivitäten** und klicken Sie mit der rechten Maustaste auf ein Programm.

   ![](assets/mobile-right-click-hand.jpg)

1. Klicken Sie auf **Neues lokales Element**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >Alternativ können Sie auf die Dropdownliste **Neu** klicken.

1. Klicken Sie auf **SMS-Nachricht**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. Geben Sie einen Namen und eine optionale Beschreibung für die neue SMS-Nachricht ein und klicken Sie auf **Erstellen**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. Klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/edit-draft-hand.jpg)

1. Klicken Sie im Meldungseditor in die blaue Blase und beginnen Sie mit der Texteingabe.

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >Die Beschränkungen für die USA und Kanada unterscheiden sich bei 160 bzw. 130 Zeichen. Wenn Sie diese Zeichenbeschränkungen überschreiten, kann Ihre Nachricht geteilt werden. Während wir zeigen, wenn Sie die Grenze von Kanada überschreiten, ist der Editor für US optimiert und teilt die Nachricht auf der Grundlage der US-Grenze.

1. Klicken Sie im Menü &quot;Einfügen&quot;auf **Token**, um Ihrer Nachricht ein Token hinzuzufügen.

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >Durch das Hinzufügen eines Tokens kann die Nachricht u. U. die erlaubte Zeichenanzahl überschreiten. Die Nachricht wird dann aufgeteilt, was zu zusätzlichen Kosten führt.

1. Klicken Sie im Menü &quot;Einfügen&quot;auf **Link**, um Ihrer Nachricht einen Link hinzuzufügen.

   ![](assets/full-message-link-hand.jpg)

1. Wählen Sie einen Linktyp aus. Die Marketo-Landingpage ist die Standardeinstellung. Wenn Sie damit beginnen, müssen Sie die Landingpage aus der Dropdown-Liste auswählen und auf **Einfügen** klicken.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >Die beiden Tracking-Links sind standardmäßig ausgewählt.

1. Wenn Sie stattdessen eine externe URL verwenden möchten, klicken Sie auf die Schaltfläche **Externe URL** und geben Sie die URL in das Feld URL ein. Klicken Sie auf **Einfügen**.

   ![](assets/insert-link-url-hands.jpg)

1. Der Link wird in der Nachricht angezeigt.

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo zeigt eine Link-Vorschau der Markenverfolgungsdomäne an. Wenn Sie das Kontrollkästchen für den Link &quot;mkt_tok&quot;deaktivieren, wird der Link geändert. Deaktivieren Sie auch das Kontrollkästchen &quot;Link verfolgen&quot;, und die URL wird auf die Standardlänge gekürzt (z. B. www.mygooglepage.com).

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >Die Zeichenanzahl bezieht sich nur auf die Zeichen in der niedrigsten Meldung.

Wenn Sie mehr als die US-Grenze einfügen, unterteilt der Editor Ihre Nachricht in Abschnitte. Die Gesamtsumme ist auf 900 Zeichen begrenzt. Nach Erreichen dieser Grenze wird die Nachricht automatisch abgeschnitten, wenn sie an ihre Audience gesendet wird.
