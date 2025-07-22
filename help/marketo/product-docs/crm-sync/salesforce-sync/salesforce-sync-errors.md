---
description: Salesforce-Synchronisierungsfehler - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisierungsfehler
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 4%

---

# [!DNL Salesforce] Synchronisierungsfehler {#salesforce-sync-errors}

Zeigen Sie eine Zusammenfassung der Fehler an, auf die während des Synchronisierungsprozesses gestoßen ist. Dazu gehören Fehler, die durch Fehler beim Synchronisieren inkompatibler Daten verursacht werden.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Synchronisierungsfehler anzeigen {#view-sync-errors}

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-errors-1.png)

1. Klicken Sie unter Integration auf **Salesforce** und dann auf die Registerkarte **[!UICONTROL Synchronisierungsfehler]**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Die aufgelisteten Fehler reichen von der aktuellen Zeit bis fünf Tage vor der aktuellen Synchronisierung.

| Feld | Beschreibung |
|---|---|
| Fehlgeschlagen am | Datensatzebene _oder_ Auftragsebene |
| Datum/Uhrzeit des Fehlers | Fehlerdetails |
| Fehlertyp | SFDC-Rückmeldung |

>[!TIP]
>
>Durch Klicken auf den Datensatz auf Datensatzebene werden die Marketo- und [!DNL Salesforce]-IDs des zugehörigen Objekts angezeigt. In einigen Fällen stammen die Meldungen zu Fehlern auf Datensatz- und Auftragsebene direkt aus [!DNL Salesforce]. Die Online-Suche nach ihnen kann zusätzliche Details liefern.

## Synchronisierungsfehler filtern {#filter-sync-errors}

1. Um die Daten zu filtern, klicken Sie auf das Filtersymbol ganz rechts auf der Seite.

   ![](assets/salesforce-sync-errors-3.png)

1. Wählen Sie Ihren Datums- und Zeitbereich aus und filtern Sie dann nach Fehlertyp (Auftragsebene oder Datensatzebene). Klicken Sie **[!UICONTROL Anwenden]** wenn Sie fertig sind.

   ![](assets/salesforce-sync-errors-4.png)

**OPTIONALER SCHRITT**: Um Synchronisierungsfehler zu exportieren, klicken Sie auf **[!UICONTROL Exportieren]**. Die Daten werden als CSV exportiert.

![](assets/salesforce-sync-errors-5.png)
