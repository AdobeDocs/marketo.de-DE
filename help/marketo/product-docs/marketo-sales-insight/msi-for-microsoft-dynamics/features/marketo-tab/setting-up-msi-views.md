---
description: Erfahren Sie, wie Sie MSI-Ansichten in Microsoft Dynamics einrichten. Konfigurieren Sie, welche Marketo Sales Insight-Registerkarten und -Daten den Benutzenden angezeigt werden.
title: Einrichten von MSI-Ansichten
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/PylFEW3pRnOwoIVF8hG2pKcFix5DO7ynWomXOfvy1e0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 264
ht-degree: 4%

---

# Einrichten von MSI-Ansichten {#setting-up-msi-views}

Durch die Installation des [!DNL Sales Insight]-Plug-ins in Dynamics werden die [!DNL Best Bets] und zugehörigen Dashboards automatisch zur Siteübersicht hinzugefügt. Wenn die Dashboards aus irgendeinem Grund nicht hinzugefügt werden, erfahren Sie hier, wie Sie sie manuell hinzufügen.

1. Klicken Sie in Dynamics auf das Zahnradsymbol und wählen Sie **[!UICONTROL Erweiterte Einstellungen]** aus der Dropdown-Liste aus.

1. Klicken Sie oben links im Bildschirm auf **[!UICONTROL Einstellungen]**. Wählen Sie unter Anpassung **[!UICONTROL Anpassungen]** aus.

1. Klicken Sie **[!UICONTROL System anpassen]**.

1. Klicken Sie in der Baumstruktur links auf **[!UICONTROL Client-Erweiterungen]** und doppelklicken Sie auf **[!UICONTROL Siteübersicht]**.

1. Klicken Sie auf den Pfeil nach rechts, um zur nächsten Seite zu gelangen. Unter „Vertrieb“ sollte Marketo angezeigt werden. Andernfalls müssen Sie sicherstellen, dass Sie das Paket ordnungsgemäß importiert haben.

   >[!NOTE]
   >
   >Unter Marketo sollten Sie Folgendes besitzen: Best Bets, Meine E-Mail, Web-Aktivität und Anonyme Web-Aktivität. Wenn eines dieser Dashboards fehlt, klicken Sie auf das Pluszeichen (+) über „Verkauf“ und fügen Sie es als Unterbereich hinzu.

1. Klicken Sie auf ein Dashboard, um es auszuwählen. Geben Sie in der Spalte rechts für jede Komponente die entsprechenden Informationen ein. Sie können alle nicht aufgelisteten Kategorien ignorieren.

   **Best Bets**</br>
URL: mainviewBestBets.html</br>
Symbol: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Titel: Best Bets

   **Meine E-Mail**</br>
URL: mkt_/MainViewMyEmail.html</br>
Symbol: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
Titel: Meine E-Mail

   **Web-Aktivität**</br>
URL: mkt_/MainViewWebActivity.html</br>
Symbol: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Titel: Web-Aktivität

   **Anonyme Web-Aktivität**</br>
URL: mkt_/MainViewWebActivity.html</br>
Symbol: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Titel: Anonyme Web-Aktivität

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.
