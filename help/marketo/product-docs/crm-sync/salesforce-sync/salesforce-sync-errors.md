---
description: Salesforce-Synchronisierungsfehler - Marketo Docs - Produktdokumentation
title: Salesforce-Synchronisierungsfehler
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 3%

---

# Salesforce-Synchronisierungsfehler {#salesforce-sync-errors}

Ansicht einer Zusammenfassung der Fehler, die während des Synchronisierungsprozesses aufgetreten sind. Dies schließt Fehler ein, die durch Fehler bei der Synchronisierung inkompatibler Daten verursacht wurden.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Ansicht-Synchronisierungsfehler {#view-sync-errors}

1. Klicken Sie auf **Admin**.

   ![](assets/salesforce-sync-errors-1.png)

1. Klicken Sie unter Integration auf **Salesforce** und dann auf die Registerkarte **Fehler synchronisieren**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Die aufgelisteten Fehler reichen von der aktuellen Zeit bis zu fünf Tagen vor der aktuellen Synchronisierung.

| Feld | Beschreibung |
|---|---|
| Fehlgeschlagen an | Datensatzebene _oder_ |
| Datum/Uhrzeit des Fehlers | Fehlerdetails |
| Fehlertyp | SFDC-Rückkehrmeldung |

>[!TIP]
>
>Wenn Sie auf den Datensatz auf Datensatzebene klicken, werden die Marketo- und Salesforce-IDs des zugehörigen Objekts angezeigt. In einigen Fällen stammt die Meldung auf der Datensatzebene und auf der Auftragsebene direkt von Salesforce. Die Online-Suche kann weitere Details liefern.

## Filter-Synchronisierungsfehler {#filter-sync-errors}

1. Klicken Sie zum Filtern der Daten auf das Filtersymbol ganz rechts auf der Seite.

   ![](assets/salesforce-sync-errors-3.png)

1. Wählen Sie Datum und Zeitraum aus und filtern Sie dann nach Fehlertyp (Auftragsebene oder Datensatzstufe). Klicken Sie nach Abschluss des Vorgangs auf **Apply**.

   ![](assets/salesforce-sync-errors-4.png)

**Optionaler Schritt**: Um Synchronisierungsfehler zu exportieren, klicken Sie auf  **Exportieren**. Die Daten werden als CSV exportiert.

![](assets/salesforce-sync-errors-5.png)
