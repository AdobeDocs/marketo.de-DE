---
description: Wie kann ich Selbstansichten verhindern - Marketo Docs - Produktdokumentation
title: Wie kann ich Selbstansichten verhindern?
hide: true
hidefromtoc: true
source-git-commit: 3b7cc0c855221f6fd0fba6dca08ccbe361ca9758
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Wie kann ich Selbstansichten verhindern? {#how-do-i-prevent-self-views}

Falsch-Positiv-Werte für das Ansichtstracking können zu Inkonsistenzen bei der Berichterstellung führen. Dies tritt oft auf, wenn Benutzer von Marketo Sales versehentlich das Tracking-Pixel von ihrem E-Mail-Client aus aufrufen (dies wird als Selbstansicht bezeichnet). Im Folgenden finden Sie einige Tipps, wie Sie Selbstansichten deutlich reduzieren und sogar beseitigen können.

## Web (Outlook Web App und Gmail) {#web-outlook-web-app-and-gmail}

Marketo Sales speichert ein Cookie in Ihrem Browser, um zu verhindern, dass Ansichten beim Öffnen Ihrer E-Mails in Outlook Web App und Gmail verfolgt werden. Wenn Sie weiterhin Selbstansichten erhalten, empfehlen wir Folgendes:

* Stellen Sie sicher, dass Cookies auf Ihrem Computer aktiviert sind.

* Wenn Sie einen neuen Computer oder ein neues Mobilgerät verwenden, stellen Sie sicher, dass Sie sich bei der Webanwendung angemeldet haben. Dadurch können wir Ihren Computer/Ihr Gerät in Zukunft erkennen.

## Desktop (Windows) {#desktop-windows}

Ansichten werden verfolgt, indem Sie ein kleines unsichtbares Bildpixel in Ihren E-Mail-Client herunterladen. Sie können die Anzahl der Selbstansichten in Outlook erheblich verringern, indem Sie Bilder deaktivieren, die automatisch heruntergeladen werden. Im Folgenden werden die Schritte beschrieben.

1. Klicken Sie in Outlook auf **Datei** in der Menüleiste.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Klicken **Optionen**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Klicken Sie im Dialogfeld &quot;Outlook Options&quot;auf **Vertrauenscenter**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Klicken Sie unter &quot;Microsoft Outlook Trust Center&quot;auf **Einstellungen für das Sicherheitscenter**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Klicken Sie im Menü auf der linken Seite auf Automatischer Download und wählen Sie die **Herunterladen von Bildern nicht automatisch in HTML-E-Mail- oder RSS-Elementen** aktivieren.

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Klicken **OK** im Dialogfeld &quot;Sicherheitscenter&quot;angezeigt.

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Klicken **OK** im Dialogfeld &quot;Outlook Options&quot;.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Desktop (Mac) {#desktop-mac}

Ansichten werden verfolgt, indem Sie ein kleines unsichtbares Bildpixel in Ihren E-Mail-Client herunterladen. Sie können die Anzahl der Selbstansichten in Outlook erheblich verringern, indem Sie Bilder deaktivieren, die automatisch heruntergeladen werden. Im Folgenden werden die Schritte beschrieben.

1. Klicken Sie in Outlook auf **Outlook** in der Menüleiste und wählen Sie **Voreinstellungen**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Wählen Sie unter E-Mail die Option **Lesen**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Klicken Sie unter &quot;Security&quot;auf die **Nie** Optionsfeld.

   ![](assets/how-do-i-prevent-self-views-10.png)