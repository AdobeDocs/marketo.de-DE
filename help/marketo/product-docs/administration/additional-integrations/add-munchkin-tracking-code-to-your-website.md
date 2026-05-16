---
unique-page-id: 2360354
description: Fügen Sie Marketo [!DNL Munchkin] JavaScript zu Ihrer Site hinzu, um Besuche zu verfolgen und Web-basierte Kampagnen zu aktivieren.
title: Hinzufügen  [!DNL Munchkin]  Trackingcodes zu Ihrer Website
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
TQID: https://experienceleague.adobe.com/3L0oDc3Xx3IaOy8t8Ut2W9c4YkRTdS5Ryd4r-Yuuhts
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 685
ht-degree: 3%

---

# Hinzufügen [!DNL Munchkin] Trackingcodes zu Ihrer Website {#add-munchkin-tracking-code-to-your-website}

Der benutzerdefinierte JavaScript-Trackingcode von Marketo namens [!DNL Munchkin] verfolgt alle Personen, die Ihre Website besuchen, sodass Sie mit automatisierten Marketing-Kampagnen auf ihre Besuche reagieren können. Sogar anonyme Besucher werden zusammen mit ihren IP-Adressen und anderen Informationen verfolgt. **Ohne diesen Trackingcode können Sie Besuche oder andere Aktivitäten auf Ihrer Website nicht verfolgen**!

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie Zugriff auf einen erfahrenen JavaScript-Entwickler haben. Der technische Support von Marketo unterstützt nicht bei der Fehlerbehebung bei benutzerdefiniertem JavaScript.

## Hinzufügen von Trackingcode zu Ihrer Website {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud-Benutzer können auch die [Marketo-Integration in Adobe Launch](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} verwenden, um [!DNL Munchkin] Skript auf ihren Web-Seiten einzufügen. Wenn Sie Adobe Launch verwenden _(das [!DNL Munchkin] wird automatisch hinzugefügt_ sodass Sie es nicht selbst hinzufügen müssen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Auf **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Wählen Sie **[!UICONTROL asynchron]** für **[!UICONTROL Trackingcode-Typ]** aus.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >In fast allen Fällen sollten Sie den asynchronen Code verwenden. [Weitere Informationen](#types-of-munchkin-tracking-codes).

1. Kopieren Sie den JavaScript-Trackingcode, der Ihrer Website hinzugefügt werden soll.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >Verwenden Sie nicht den in diesem Screenshot gezeigten Code - Sie müssen den eindeutigen Code verwenden, der in Ihrem Konto angezeigt wird.

   >[!TIP]
   >
   >Fügen Sie den Trackingcode auf die Webseiten ein, die Sie verfolgen möchten. Dabei kann es sich um jede Seite für kleinere Websites handeln oder nur um wichtige Seiten auf Websites mit vielen dynamisch generierten Web-Seiten, Benutzerforen usw.

   Um die bestmöglichen Ergebnisse zu erzielen, verwenden Sie den asynchronen [!DNL Munchkin]-Code und platzieren Sie ihn in den `<head>` Elementen Ihrer Seiten. Wenn Sie den einfachen Code verwenden (nicht empfohlen), befindet sich dieser direkt vor dem `</body>`-Tag.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Bei Sites mit hohem Traffic-Volumen (d. h. Hunderttausende von Besuchen pro Monat) wird empfohlen, keine anonymen Personen zu verfolgen. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking){target="_blank"}.

## Hinzufügen von Trackingcode bei Verwendung mehrerer Arbeitsbereiche {#add-tracking-code-when-using-multiple-workspaces}

Wenn Sie Arbeitsbereiche in Ihrem Marketo-Konto verwenden, verfügen Sie wahrscheinlich auch über separate Web-Präsenzen, die Ihren Arbeitsbereichen entsprechen. In diesem Fall können Sie das JavaScript zum Tracking von [!DNL Munchkin] verwenden, um Ihre anonymen Personen dem richtigen Arbeitsbereich und der richtigen Partition zuzuweisen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Auf **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Wählen Sie den entsprechenden Arbeitsbereich für die Web-Seiten aus, die Sie verfolgen möchten.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Wenn Sie den speziellen Workspace-[!DNL Munchkin]-Code nicht verwenden, werden die Personen der Standardpartition zugewiesen, die bei der Einrichtung Ihres Kontos erstellt wurde. Standardmäßig heißt sie [!UICONTROL Standard], aber dieser Name wurde möglicherweise geändert.

1. Wählen Sie **[!UICONTROL asynchron]** für **[!UICONTROL Trackingcode-Typ]** aus.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Kopieren Sie den JavaScript-Trackingcode, der Ihrer Website hinzugefügt werden soll.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >Verwenden Sie nicht den in diesem Screenshot gezeigten Code - Sie müssen den eindeutigen Code verwenden, der in Ihrem Konto angezeigt wird.

1. Platzieren Sie den Trackingcode auf Ihren Web-Seiten im `<head>`. Neue Personen, die diese Seite besuchen, werden dieser Partition zugewiesen.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Sie können nur ein [!DNL Munchkin]-Tracking-Skript für eine einzelne Partition und einen einzigen Arbeitsbereich auf einer Seite verwenden. Schließen Sie keine Tracking-Skripte für mehrere Partitionen/Arbeitsbereiche auf Ihrer Website ein.

   >[!NOTE]
   >
   >In Marketo erstellte Landingpages enthalten automatisch Trackingcode. Sie müssen diesen Code nicht zu ihnen hinzufügen.

## Typen von [!DNL Munchkin]-Trackingcodes {#types-of-munchkin-tracking-codes}

Es gibt drei Arten von [!DNL Munchkin]-Trackingcodes, aus denen Sie wählen können. Jede wirkt sich auf die Ladezeiten der Web-Seite unterschiedlich aus.

1. **[!UICONTROL Einfach]**: verfügt über die wenigsten Codezeilen, wird aber nicht für die Ladezeit der Web-Seite optimiert. Dieser Code lädt die jQuery-Bibliothek jedes Mal, wenn eine Web-Seite geladen wird.
1. **[!UICONTROL asynchron]**: Verringert die Ladezeit von Web-Seiten.
1. **[!UICONTROL Asynchrone jQuery]**: Verringert die Ladezeit der Web-Seite und verbessert auch die Systemleistung. In diesem Code wird davon ausgegangen, dass Sie bereits über jQuery verfügen, und es wird nicht geprüft, ob es geladen wird.

## Testen, ob der [!DNL Munchkin]-Code funktioniert {#test-if-your-munchkin-code-is-working}

So überprüfen Sie, ob Ihr [!DNL Munchkin]-Code nach dem Hinzufügen funktioniert:

1. Besuchen Sie Ihre Webseite.

1. Klicken Sie in Ihrem [!DNL My Marketo] auf die Kachel **[!UICONTROL Analytics]** .

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Klicken Sie **[!UICONTROL Webseitenaktivität]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Setup“ und doppelklicken Sie auf **[!UICONTROL Activity Source]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Ändern Sie die [!UICONTROL Activity Source] in **[!UICONTROL Anonyme Besucher (einschließlich ISPs)]** und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Bericht“.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Wenn keine Daten angezeigt werden, warten Sie einige Minuten und klicken Sie dann unten auf [!UICONTROL Aktualisieren]-Symbol.
