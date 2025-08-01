---
description: Dynamic Chat-Integration - Marketo-Dokumente - Produktdokumentation
title: Integration von Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# Integration von Dynamic Chat {#dynamic-chat-integration}

Erfahren Sie mehr über die Integration von Dynamic Chat mit Sales Insight.

>[!PREREQUISITES]
>
>* Ihr Sales Insight SFDC-Paket muss Version [2.4.0 oder höher sein](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Die [Dynamic Chat-Integration muss ](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} sein
>
>* Stellen Sie sicher, dass in Ihrer Sales [Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"}Betriebseinstellungen) das Feld „API-Geheimschlüssel“ ausgefüllt ist. Wenn nicht, erfahren Sie hier, wie Sie [ abrufen ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Registerkarte &quot;[!DNL Marketo Sales Insight]&quot; {#marketo-sales-insight-configuration-tab}

Gehen Sie wie folgt vor, um die [!DNL Dynamic Chat]-Integration zu aktivieren.

1. Melden Sie sich bei Ihrem [!DNL Salesforce] Konto an, klicken Sie auf das + -Symbol am Ende der Registerkartenleiste und klicken Sie auf **[!DNL Marketo Sales Insight Config]**.

1. Klicken Sie, um das &quot;[!UICONTROL VisualForce-Bedienfeld“ &#x200B;].

   ![](assets/dynamic-chat-integration-1.png)

1. Aktivieren Sie das **[!UICONTROL Dynamic Chat-Daten aktivieren]**.

   ![](assets/dynamic-chat-integration-2.png)

## Funktionsübersicht {#feature-overview}

Die folgenden [!DNL Dynamic Chat] können von [!DNL Sales Insight] Benutzern genutzt werden…

Dialogfeld „Interagiert“: In Marketo angemeldet und in [!DNL Sales Insight] aufgefüllt, wenn ein Besucher auf einen Chatbot klickt und mit dem Dialogfeld interagiert.

* Dialogname
* „Seiten-URL“
* Status (initiiert/gelöscht/abgeschlossen)

Geplanter Termin: Anmelden bei Marketo und Ausfüllen in [!DNL Sales Insight], wenn ein Besucher einen Termin über den Chatbot erfolgreich plant.

* Dialogname
* Agent
* „Seiten-URL“
* Geplant am (Datum und Zeitstempel einfügen)
* Status (geplant, neu geplant, abgebrochen)

Marketo Ziel erreicht: Angemeldet und in [!DNL Sales Insight] aufgefüllt, wenn ein Besucher ein Ziel in einem beliebigen Dialogfluss erreicht.

* Dialogname
* Zielname
* „Seiten-URL“

Interagiert mit Dokument: Wurde in Marketo angemeldet und in [!DNL Sales Insight] aufgefüllt, wenn ein Besucher mit einem Dokument interagiert, das über den Chatbot freigegeben wurde.

* Dialogname
* Dokument
* Status

Chat-Aktivitäten sind im Insights-Dashboard verfügbar.

![](assets/dynamic-chat-integration-3.png)

Eine Chat-Registerkarte ist in den Bedienfeldern Lead und Kontakt verfügbar. Sie enthält [!UICONTROL Aktivitätstyp], [!UICONTROL Dialogfeldname] und [!UICONTROL Datum].

![](assets/dynamic-chat-integration-4.png)

Sie können weitere Informationen zu einem Aktivitätstyp erhalten, indem Sie darauf klicken.

![](assets/dynamic-chat-integration-5.png)

Gleichermaßen enthalten die Konto- und Opportunity-Bedienfelder [!UICONTROL Name], [!UICONTROL Aktivitätstyp], [!UICONTROL Dialogfeldname] und [!UICONTROL Datum] Spalten.

![](assets/dynamic-chat-integration-6.png)

Die Registerkarte Chat ist auch in Ihrer Registerkarte Global Marketo enthalten. Es umfasst drei Aktivitätstypen ([!UICONTROL Interaktives &#x200B;], [!UICONTROL Geplanter Termin], [!UICONTROL Ziel erreicht]) sowie die folgenden Spalten:

* [!UICONTROL Person]
* [!UICONTROL Konto]
* [!UICONTROL Aktivitätstyp] ([!UICONTROL Dialog aktiviert], [!UICONTROL Geplanter Termin], [!UICONTROL Ziel erreicht])
* [!UICONTROL Dialogfeldname]
* [!UICONTROL Datum]

Auch hier erfahren Sie mehr über einen Aktivitätstyp, indem Sie darauf klicken.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Wenn das Kontrollkästchen [!UICONTROL Dynamic Chat-Daten aktivieren] deaktiviert ist, werden die folgenden Funktionen deaktiviert:
>
>* Zeile mit Chat-Aktivitäten im Insights-Dashboard (intelligentes Raster und wöchentliche Listenansicht)
>* Registerkarte „Chat“ in den Bedienfeldern „Lead“, „Kontakt“, „Konto“ und „Opportunity“
>* Registerkarte „Chat“ auf der Registerkarte „Globale Marketo&quot;
>
>Es ist nicht möglich, nur eine dieser Funktionen zu deaktivieren.
