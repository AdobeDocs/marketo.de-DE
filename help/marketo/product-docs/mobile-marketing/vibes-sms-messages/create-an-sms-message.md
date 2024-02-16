---
description: SMS erstellen - Marketo Docs - Produktdokumentation
title: SMS erstellen
feature: Mobile Marketing
source-git-commit: c0e2c460559860a22a649e67624db0ad717ae327
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 2%

---

# SMS erstellen {#create-an-sms-message}

So erstellen Sie eine SMS-Nachricht:

>[!AVAILABILITY]
>
>Diese Funktion ist als Add-on für Ihr Adobe Marketo Engage-Konto verfügbar. Damit sie ordnungsgemäß bereitgestellt werden kann, muss sie über Adobe erworben werden. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer). Die native Integration von Marketo Vibes SMS ist in den USA und Kanada verfügbar. Für andere Länder kann eine Verbindung über Marketo Webhooks von [direkten Kontakt mit Besuchern](https://www.vibes.com/talk-to-sales){target="_blank"}.

>[!PREREQUISITES]
>
>[Hinzufügen von Assets als LaunchPoint-Dienst](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}

1. Navigieren Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/create-an-sms-message-1.png)

1. Klicken Sie mit der rechten Maustaste auf das gewünschte Programm und wählen Sie **[!UICONTROL Neues lokales Asset]**.

   ![](assets/create-an-sms-message-2.png)

1. Auswählen **SMS-Nachricht**.

   ![](assets/create-an-sms-message-3.png)

1. Geben Sie einen Namen und eine optionale Beschreibung für die neue SMS-Nachricht ein und klicken Sie auf **Erstellen**.

   ![](assets/create-an-sms-message-4.png)

1. Klicken Sie im Editor in die blaue Blase und beginnen Sie mit der Texteingabe.

   ![](assets/create-an-sms-message-5.png)

   >[!NOTE]
   >
   >Die Zeichenbeschränkung für eine SMS-Nachricht beträgt 160 Zeichen, die dem standardmäßigen ASCII-Zeichensatz entsprechen. Bei mehr als 160 Zeichen wird die Nachricht auf der Grundlage der Gesamtzahl der Zeichen aufgeteilt.

1. Um Ihrer Nachricht ein Token hinzuzufügen, schreiben Sie eine schnelle Begrüßung und klicken Sie auf **Token**.

   ![](assets/create-an-sms-message-6.png)

   >[!NOTE]
   >
   >Durch das Hinzufügen eines Tokens kann die Nachricht u. U. die erlaubte Zeichenanzahl überschreiten. Die Nachricht wurde dann aufgeteilt und eine zusätzliche Nachricht erstellt.

   >[!IMPORTANT]
   >
   >SMS-Kompatibilität: Alle ausgehenden SMS-Nachrichten müssen den Namen der Marke oder die Beschreibung des Programms enthalten. HILFE- und STOP-Anweisungen sollten mindestens einmal monatlich pro Abonnent für wiederkehrende Nachrichtenprogramme bereitgestellt werden.

1. Wählen Sie die gewünschte **Token**, geben Sie einen optionalen **Standardwert** und klicken Sie auf **Erstellen**.

   ![](assets/create-an-sms-message-7.png)

1. Um einen Link hinzuzufügen, wählen Sie aus, wo in der Nachricht der Link angezeigt werden soll, und klicken Sie auf **Link**.

   ![](assets/create-an-sms-message-8.png)

1. Wählen Sie einen Link-Typ aus. Marketo-Landingpage ist die Standardeinstellung. Wenn Sie damit fertig sind, klicken Sie auf das Dropdown-Menü Landingpage und wählen Sie die gewünschte Seite aus. Klicks **Einfügen** wann geschehen.

   ![](assets/create-an-sms-message-9.png)

   >[!NOTE]
   >
   >Die beiden Tracking-Links sind standardmäßig ausgewählt. Wenn Sie die Option Nur mkt_tok einschließen deaktivieren, kann der Link weiterhin verfolgt werden. Nach der Umleitung enthält die Ziel-URL jedoch nicht den Abfragezeichenfolgenparameter mkt_tok. Dieser Parameter wird von Marketo-Einstiegsseiten und Munchkin verwendet, um eine ordnungsgemäße Verfolgung der Personenaktivitäten sicherzustellen (z. B. wenn sich eine Person abmeldet).

1. Wenn Sie stattdessen eine externe URL verwenden möchten, wählen Sie **Externe URL**, geben Sie die URL ein/fügen Sie sie ein und klicken Sie auf **Einfügen**.

   ![](assets/create-an-sms-message-10.png)

   >[!NOTE]
   >
   >Wenn Sie die Option &quot;Link verfolgen&quot;beibehalten, ändert Marketo die URL automatisch zu Tracking-Zwecken. Wenn Sie die Verfolgung deaktivieren, wird die URL unverändert in der Nachricht angezeigt (z. B. `www.adobe.com`).

   >[!CAUTION]
   >
   >Es wird empfohlen, _not_ Verwenden Sie URL-Shorteners (z. B. Bitly), da die Provider Ihre Nachricht als Spam kennzeichnen können.

1. Der Link wird in der Nachricht angezeigt.

   ![](assets/create-an-sms-message-11.png)

   >[!NOTE]
   >
   >Marketo zeigt eine Link-Vorschau der Marken-Tracking-Domäne an. Wenn Sie das Kontrollkästchen &quot;mkt_tok&quot;-Link deaktivieren, wird der Link geändert.

Wenn Sie mehr als 160 Zeichen einfügen, unterteilt der Editor Ihre SMS in Abschnitte. Es gibt eine Gesamtbeschränkung von 900 Zeichen pro Nachricht. Wenn Sie diese Anzahl überschreiten, wird die Nachricht beim Versand abgeschnitten.
