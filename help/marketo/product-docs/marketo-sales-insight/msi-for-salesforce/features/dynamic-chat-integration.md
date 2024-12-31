---
description: Dynamic Chat-Integration - Marketo-Dokumente - Produktdokumentation
title: Integration von Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 6e81a8891f7d6e5916549d453a694b42e08cd496
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 6%

---

# Integration von Dynamic Chat {#dynamic-chat-integration}

Erfahren Sie mehr über die Integration von Dynamic Chat mit Sales Insight.

>[!PREREQUISITES]
>
>* Ihr Sales Insight SFDC-Paket muss Version [2.4.0 oder höher sein](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Die [Dynamic Chat-Integration muss eingerichtet ](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}.
>
>* Stellen Sie sicher, dass in Ihrem Sales [Betriebseinstellungen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} das Feld „API-Geheimschlüssel“ ausgefüllt ist. Wenn nicht, erfahren Sie hier, wie Sie [ abrufen ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Registerkarte „Konfiguration von Marketo Sales Insight“ {#marketo-sales-insight-configuration-tab}

Gehen Sie wie folgt vor, um die Dynamic Chat-Integration zu aktivieren.

1. Melden Sie sich bei Ihrem Salesforce-Konto an, klicken Sie auf das + am Ende der Registerkartenleiste und klicken Sie auf **Marketo Sales Insight Config**.

1. Klicken Sie, um das Bedienfeld „VisualForce“ zu entfalten.

   ![](assets/dynamic-chat-integration-1.png)

1. Aktivieren Sie das **Dynamic Chat-Daten aktivieren**.

   ![](assets/dynamic-chat-integration-2.png)

## Funktionsübersicht {#feature-overview}

Die folgenden Dynamic Chat-Aktivitäten können von Sales Insight-Benutzern genutzt werden…

Dialog „Interagiert“: In Marketo angemeldet und in Sales Insight ausgefüllt, wenn ein Besucher auf einen Chatbot klickt und mit dem Dialogfeld interagiert.

* Dialogname
* „Seiten-URL“
* Status (initiiert/gelöscht/abgeschlossen)

Geplanter Termin: In Marketo angemeldet und in Sales Insight ausgefüllt, wenn ein Besucher einen Termin über den Chatbot erfolgreich plant.

* Dialogname
* Agent
* „Seiten-URL“
* Geplant am (Datum und Zeitstempel einfügen)
* Status (geplant, neu geplant, abgebrochen)

Marketo Erreichtes Ziel: Angemeldet und in Sales Insight eingetragen, wenn ein Besucher ein Ziel in einem beliebigen Dialogfluss erreicht.

* Dialogname
* Zielname
* „Seiten-URL“

Interagiert mit Dokument: Wurde in Marketo angemeldet und in Sales Insight eingefügt, wenn ein Besucher mit einem Dokument interagiert, das über den Chatbot freigegeben wurde.

* Dialogname
* Dokument
* Status

Chat-Aktivitäten sind im Insights-Dashboard verfügbar.

![](assets/dynamic-chat-integration-3.png)

Eine Chat-Registerkarte ist in den Bedienfeldern Lead und Kontakt verfügbar. Sie enthält die Spalten Aktivitätstyp, Dialogfeldname und Datum.

![](assets/dynamic-chat-integration-4.png)

Sie können weitere Informationen zu einem Aktivitätstyp erhalten, indem Sie darauf klicken.

![](assets/dynamic-chat-integration-5.png)

Gleichermaßen enthalten die Bedienfelder Konto und Opportunity die Spalten Name, Aktivitätstyp, Dialogfeldname und Datum.

![](assets/dynamic-chat-integration-6.png)

Die Registerkarte Chat ist auch in Ihrer Registerkarte Global Marketo enthalten. Es umfasst drei Aktivitätstypen (Dialogfeld „Interagiert“, Geplanter Termin, Ziel erreicht) sowie die folgenden Spalten:

* Person
* Konto
* Aktivitätstyp (Dialog „Interagiert“, Terminplanung, Ziel erreicht)
* Dialogname
* Datums- und Zeitstempel

Auch hier erfahren Sie mehr über einen Aktivitätstyp, indem Sie darauf klicken.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Wenn das Kontrollkästchen &quot;Dynamic Chat-Daten aktivieren“ deaktiviert ist, werden die folgenden Funktionen deaktiviert:
>
>* Zeile mit Chat-Aktivitäten im Insights-Dashboard (intelligentes Raster und wöchentliche Listenansicht)
>* Registerkarte „Chat“ in den Bedienfeldern „Lead“, „Kontakt“, „Konto“ und „Opportunity“
>* Registerkarte „Chat“ auf der Registerkarte „Globale Marketo&quot;
>
>Es ist nicht möglich, nur eine dieser Funktionen zu deaktivieren.

