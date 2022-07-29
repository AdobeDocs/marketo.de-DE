---
description: Dynamic Chat-Integration - Marketo-Dokumente - Produktdokumentation
title: Dynamic Chat-Integration
hide: true
hidefromtoc: true
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: b8f2308d3b1a252a8fe10ba0a26d4c5aa07c4756
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 5%

---

# Dynamic Chat-Integration {#dynamic-chat-integration}

Erfahren Sie mehr über die Integration von Dynamic Chat mit Sales Insight.

>[!PREREQUISITES]
>
>* Ihr Sales Insight SFDC-Paket muss version sein [1.9 oder höher](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* Sie müssen über die [Dynamic Chat-Integration](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} einrichten


## Registerkarte &quot;Marketo Sales Insight-Konfiguration&quot; {#marketo-sales-insight-configuration-tab}

Gehen Sie wie folgt vor, um die Dynamic Chat-Integration zu aktivieren.

1. Melden Sie sich bei Ihrem Salesforce-Konto an, klicken Sie auf das Pluszeichen am Ende der Registerkartenleiste und klicken Sie auf **Marketo Sales Insight-Konfiguration**.

1. Klicken Sie auf , um den Bereich &quot;Visualforce&quot;zu entfernen.

   ![](assets/dynamic-chat-integration-1.png)

1. Wählen Sie die **Dynamische Chat-Daten aktivieren** aktivieren.

   ![](assets/dynamic-chat-integration-2.png)

## Funktionsübersicht {#feature-overview}

Die folgenden dynamischen Chat-Aktivitäten können von Sales Insight-Benutzern genutzt werden.

Interagiertes Dialogfeld: Angemeldet in Marketo und in Sales Insight ausgefüllt, wenn ein Besucher auf einen Chat klickt und mit dem Dialogfeld interagiert.

* Dialogname
* Seiten-URL
* Status (Initiiert/Dropped/Abgeschlossen)

Geplante Ernennung: Angemeldet in Marketo und in Sales Insight ausgefüllt, wenn ein Besucher einen Termin erfolgreich über den Chat-Bot plant.

* Dialogname
* Agent
* Seiten-URL
* Geplant am (Datum und Zeitstempel einfügen)
* Status (Geplant, Neu geplant, Abgebrochen)

Erreichtes Ziel: Wird in Marketo angemeldet und in Sales Insight ausgefüllt, wenn ein Besucher in einem beliebigen Dialogfluss ein Ziel erreicht.

* Dialogname
* Zielname
* Seiten-URL

In den Bedienfeldern &quot;Lead&quot;und &quot;Kontakt&quot;ist eine Registerkarte &quot;Chat&quot;verfügbar. Sie enthält die Spalten Aktivitätstyp, Dialogfeldname und Datum .

![](assets/dynamic-chat-integration-3.png)

Sie können mehr über einen Aktivitätstyp erfahren, indem Sie darauf klicken.

![](assets/dynamic-chat-integration-4.png)

Die Bedienfelder &quot;Konto&quot;und &quot;Chancen&quot;umfassen ebenfalls die Spalten &quot;Name&quot;, &quot;Aktivitätstyp&quot;, &quot;Dialogfeldname&quot;und &quot;Datum&quot;.

![](assets/dynamic-chat-integration-5.png)

Der Tab Chat ist auch in Ihrer Registerkarte Global Marketo enthalten. Es umfasst drei Aktivitätstypen (Dialog interagieren, Terminplanung, Ziel erreicht) sowie die folgenden Spalten:

* Person
* Konto
* Aktivitätstyp (Dialogfeld &quot;Interagiert&quot;, Terminplanung, Ziel erreicht)
* Dialogname
* Datums- und Uhrzeitstempel

Erfahren Sie mehr über einen Aktivitätstyp, indem Sie darauf klicken.

![](assets/dynamic-chat-integration-6.png)

>[!NOTE]
>
>Die Aktivität &quot;Interagiert mit Dokument&quot;wird in einer kommenden Version in MSI verfügbar sein.
