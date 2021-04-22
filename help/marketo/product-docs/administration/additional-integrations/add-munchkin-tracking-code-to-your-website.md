---
unique-page-id: 2360354
description: hinzufügen Munchkin-Rückverfolgungscode auf Ihrer Website - Marketo Docs - Produktdokumentation
title: hinzufügen Munchkin-Rückverfolgungscode auf Ihrer Website
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# hinzufügen Munchkin-Trackingcode auf Ihrer Website {#add-munchkin-tracking-code-to-your-website}

Marketos benutzerspezifischer JavaScript-Rückverfolgungscode namens Munchkin verfolgt alle Personen, die Ihre Website besuchen, sodass Sie mit automatisierten Marketing-Kampagnen auf ihre Besuche reagieren können. Auch anonyme Besucher werden zusammen mit ihren IP-Adressen und anderen Informationen verfolgt. **Ohne diesen Rückverfolgungscode können Sie Besuche oder andere Aktivitäten auf Ihrer Website** nicht verfolgen!

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie Zugriff auf einen erfahrenen JavaScript-Entwickler haben. Der technische Support von Marketo ist nicht so eingerichtet, dass er bei der Fehlerbehebung für benutzerdefiniertes JavaScript unterstützt wird.

## hinzufügen Trackingcode auf Ihrer Website {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud-Kunden können auch die Integration von Marketo in Adobe Launch verwenden, um Munchkin-Skripten auf ihren Webseiten einzubinden. Rufen Sie die App [hier](https://www.adobeexchange.com/experiencecloud.details.101054.html) ab.

1. Gehen Sie zu **Admin** und klicken Sie auf **Munchkin** in der Struktur auf der linken Seite.

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   Wählen Sie Asynchron für den Rückverfolgungscode-Typ.

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >In fast allen Fällen sollten Sie den asynchronen Code verwenden. [Weitere Informationen.](#types-of-munchkin-tracking-codes)

   Klicken Sie auf und kopieren Sie den Javascript-Trackingcode, den Sie auf Ihre Website setzen möchten.

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >Verwenden Sie nicht den Code, der in diesem Screenshot gezeigt wird - Sie müssen den eindeutigen Code verwenden, der in Ihrem Konto angezeigt wird!

   >[!TIP]
   >
   >Setzen Sie Trackingcode auf die Webseiten, die Sie verfolgen möchten. Dies kann jede Seite für kleinere Sites oder nur wichtige Seiten auf Sites mit vielen dynamisch generierten Webseiten, Benutzerforen usw. sein.

   Um optimale Ergebnisse zu erzielen, verwenden Sie den asynchronen Munchkin-Code und platzieren Sie ihn in den `<head>`-Elementen Ihrer Seiten. Wenn Sie den einfachen Code verwenden (nicht empfohlen), liegt dieser direkt vor dem `</body>`-Tag.
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>Bei Sites mit hohem Traffic-Aufkommen (d. h. Hunderttausenden Besuchen pro Monat) empfehlen wir, anonyme Personen nicht zu verfolgen. [Weitere Informationen](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## hinzufügen Rückverfolgungscode bei Verwendung mehrerer Arbeitsflächen {#add-tracking-code-when-using-multiple-workspaces}

Wenn Sie Workspaces in Ihrem Marketo-Konto verwenden, haben Sie wahrscheinlich auch separate Webpräsenzen, die Ihren Arbeitsbereichen entsprechen. In diesem Fall können Sie das Munchkin-Tracking-Javascript verwenden, um Ihre anonymen Personen der richtigen Arbeitsfläche und Partition zuzuweisen.

1. Gehen Sie zu **Admin** und klicken Sie auf **Munchkin** in der Struktur auf der linken Seite.

![](assets/image2015-8-25-16-3a28-3a41.png)

1. Wählen Sie den entsprechenden Arbeitsbereich für die Webseiten aus, die Sie verfolgen möchten.

   ![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>Wenn Sie den speziellen Workspace-Munchkin-Code nicht verwenden, werden die Personen der Standardpartition zugewiesen, die beim Einrichten Ihres Kontos erstellt wurde. Es heißt zunächst &quot;Standard&quot;, aber Sie haben dies möglicherweise in Ihrem eigenen Marketo-Konto geändert.

1. Wählen Sie **Asynchron** für Rückverfolgungscode-Typ.

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. Klicken Sie auf und kopieren Sie den JavaScript-Rückverfolgungscode, der auf Ihre Website eingefügt werden soll.

   ![](assets/image2015-8-25-16-3a34-3a7.png)

   >[!CAUTION]
   >
   >Verwenden Sie nicht den Code, der in diesem Screenshot gezeigt wird - Sie müssen den eindeutigen Code verwenden, der in Ihrem Konto angezeigt wird!

1. Platzieren Sie den Rückverfolgungscode auf Ihren Webseiten im Element `<head>`. Neue Personen, die diese Seite besuchen, werden dieser Partition zugewiesen.

   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>Sie können nur ein Munchkin-Verfolgungsskript für eine einzelne Partition und einen Arbeitsbereich auf einer Seite verwenden. Schließen Sie keine Verfolgungsskripten für mehrere Partitionen/Arbeitsbereiche auf Ihrer Website ein.

>[!NOTE]
>
>In Marketo erstellte Landingpages enthalten automatisch Trackingcode, sodass Sie diesen Code nicht darauf verwenden müssen.

## Typen von Munchkin-Rückverfolgungscodes {#types-of-munchkin-tracking-codes}

Es gibt drei Arten von Munchkin-Trackingcodes, aus denen Sie wählen können. Jede Änderung wirkt sich unterschiedlich auf die Ladezeit der Webseite aus.

1. **Einfach**: hat die wenigsten Codezeilen, optimiert aber nicht für die Ladezeit der Webseite. Dieser Code lädt die jQuery-Bibliothek jedes Mal, wenn eine Webseite geladen wird.
1. **Asynchron**: verkürzt die Ladezeit der Webseite.
1. **Asynchrone jQuery**: verringert die Ladezeit von Webseiten und verbessert auch die Systemleistung. Bei diesem Code wird davon ausgegangen, dass Sie bereits über jQuery verfügen, und nicht überprüft, ob Sie ihn laden möchten.

## Testen Sie, ob Ihr Munchkin-Code {#test-if-your-munchkin-code-is-working} funktioniert.

So überprüfen Sie, ob Ihr Munchkin-Code funktioniert, nachdem Sie ihn hinzugefügt haben:

1. Besuchen Sie Ihre Webseite.

1. Gehen Sie zu **Analytics**.

   ![](assets/mainnav-analytics-hand.png)

1. Klicken Sie auf **Aktivität der Webseite**.

   ![](assets/webanalytics.png)

1. Klicken Sie auf die Registerkarte **Setup**, klicken Sie mit der Dublette auf **Aktivität Quelle** und ändern Sie sie in **Anonyme Besucher (einschließlich ISPs)**.

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. Klicken Sie auf die Registerkarte **Bericht**. Wenn keine Daten angezeigt werden, warten Sie einige Minuten und klicken Sie dann auf das Aktualisierungssymbol unten.
