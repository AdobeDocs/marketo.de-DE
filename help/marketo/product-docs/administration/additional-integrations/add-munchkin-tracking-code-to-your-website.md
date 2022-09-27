---
unique-page-id: 2360354
description: Hinzufügen des Munchkin-Trackingcodes zu Ihrer Website - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen des Munchkin-Trackingcodes zu Ihrer Website
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
source-git-commit: dbb7478ac7b7e811bb9dfeb7c5e4a80ae400ab9b
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 2%

---

# Hinzufügen des Munchkin-Trackingcodes zu Ihrer Website {#add-munchkin-tracking-code-to-your-website}

Der benutzerdefinierte JavaScript-Trackingcode von Marketo namens Munchkin verfolgt alle Personen, die Ihre Website besuchen, sodass Sie mit automatisierten Marketingkampagnen auf ihre Besuche reagieren können. Auch anonyme Besucher werden zusammen mit ihren IP-Adressen und anderen Informationen verfolgt. **Ohne diesen Trackingcode können Sie keine Besuche oder anderen Aktivitäten auf Ihrer Website verfolgen**!

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie Zugriff auf einen erfahrenen JavaScript-Entwickler haben. Der technische Support von Marketo ist nicht für die Fehlerbehebung bei benutzerdefiniertem JavaScript eingerichtet.

## Hinzufügen von Trackingcode zu Ihrer Website {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud-Kunden können auch die Marketo-Integration in Adobe Launch verwenden, um Munchkin-Skript auf ihren Webseiten einzubinden. App abrufen [here](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Klicken **Munchkin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Wählen Sie Asynchron für den Trackingcode-Typ aus.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >In fast allen Fällen sollten Sie den asynchronen Code verwenden. [Weitere Informationen](#types-of-munchkin-tracking-codes).

1. Klicken Sie auf den Javascript-Trackingcode und kopieren Sie ihn in Ihre Website.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >Verwenden Sie nicht den in diesem Screenshot angezeigten Code - Sie müssen den eindeutigen Code verwenden, der in Ihrem Konto angezeigt wird!

   >[!TIP]
   >
   >Fügen Sie den Trackingcode auf die Webseiten ein, die Sie verfolgen möchten. Dabei kann es sich um jede Seite für kleinere Sites oder nur um wichtige Seiten auf Sites mit vielen dynamisch generierten Webseiten, Benutzerforen usw. handeln.

   Die besten Ergebnisse erzielen Sie, wenn Sie den asynchronen Munchkin-Code verwenden und ihn im `<head>` Elemente Ihrer Seiten. Wenn Sie den einfachen Code verwenden (nicht empfohlen), liegt dies direkt vor dem `</body>` -Tag.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Bei Sites mit hohem Traffic-Aufkommen (d. h. Hunderttausende Besuche pro Monat) empfehlen wir, keine anonymen Personen zu verfolgen. [Weitere Informationen](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Hinzufügen von Trackingcode bei Verwendung mehrerer Arbeitsbereiche {#add-tracking-code-when-using-multiple-workspaces}

Wenn Sie Workspace in Ihrem Marketo-Konto verwenden, verfügen Sie wahrscheinlich auch über separate Webpräsenzen, die Ihren Arbeitsbereichen entsprechen. In diesem Fall können Sie das Javascript für das Munchkin-Tracking verwenden, um Ihre anonymen Personen dem richtigen Arbeitsbereich und der richtigen Partition zuzuweisen.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Klicken **Munchkin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Wählen Sie den entsprechenden Arbeitsbereich für die Webseiten aus, die Sie verfolgen möchten.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Wenn Sie den speziellen Workspace Munchkin-Code nicht verwenden, werden die Personen der Standardpartition zugewiesen, die beim Einrichten Ihres Kontos erstellt wurde. Er heißt anfangs &quot;Standard&quot;, aber Sie haben dies möglicherweise in Ihrem eigenen Marketo-Konto geändert.

1. Auswählen **Asynchron** für den Trackingcode-Typ.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Klicken Sie auf den JavaScript-Trackingcode und kopieren Sie ihn in Ihre Website.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >Verwenden Sie nicht den in diesem Screenshot angezeigten Code - Sie müssen den eindeutigen Code verwenden, der in Ihrem Konto angezeigt wird!

1. Platzieren Sie den Trackingcode auf Ihren Webseiten im `<head>` -Element. Neue Personen, die diese Seite besuchen, werden dieser Partition zugewiesen.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Sie können nur ein Munchkin-Tracking-Skript für eine Partition und einen Arbeitsbereich auf einer Seite verwenden. Schließen Sie keine Tracking-Skripte für mehrere Partitionen/Arbeitsbereiche auf Ihrer Website ein.

   >[!NOTE]
   >
   >In Marketo erstellte Landingpages enthalten automatisch Trackingcode, sodass Sie diesen Code nicht darauf ablegen müssen.

## Typen von Munchkin-Trackingcodes {#types-of-munchkin-tracking-codes}

Es gibt drei Typen von Munchkin-Trackingcodes, aus denen Sie wählen können. Jede Änderung wirkt sich unterschiedlich auf die Ladezeiten der Webseite aus.

1. **Einfach**: hat die wenigsten Codezeilen, optimiert jedoch nicht für die Ladezeit von Webseiten. Dieser Code lädt die jQuery-Bibliothek jedes Mal, wenn eine Webseite geladen wird.
1. **Asynchron**: verkürzt die Ladezeit von Webseiten.
1. **Asynchrone jQuery**: reduziert die Ladezeit von Webseiten und verbessert auch die Systemleistung. In diesem Code wird davon ausgegangen, dass Sie bereits über jQuery verfügen und nicht überprüfen, ob Sie ihn laden.

## Testen, ob Ihr Munchkin-Code funktioniert {#test-if-your-munchkin-code-is-working}

So überprüfen Sie, ob Ihr Munchkin-Code funktioniert, nachdem Sie ihn hinzugefügt haben:

1. Besuchen Sie Ihre Webseite.

1. Klicken Sie in Ihrer Marketo auf die **Analytics** Kachel.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Klicken **Webseiten-Aktivität**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Klicken Sie auf **Einrichtung** Registerkarte, doppelklicken **Aktivitätsquelle**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Ändern Sie die Aktivitätsquelle in **Anonyme Besucher (einschließlich ISPs)** und klicken Sie auf **Anwenden**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Klicken Sie auf **Bericht** Registerkarte.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Wenn keine Daten angezeigt werden, warten Sie einige Minuten und klicken Sie auf das Aktualisierungssymbol unten.
