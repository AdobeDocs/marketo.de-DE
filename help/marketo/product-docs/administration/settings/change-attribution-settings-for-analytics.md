---
unique-page-id: 2360217
description: Ändern der Attributionseinstellungen für Analytics - Marketo Docs - Produktdokumentation
title: Ändern der Attributionseinstellungen für Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Ändern der Attributionseinstellungen für Analytics {#change-attribution-settings-for-analytics}

Sie können die Art und Weise ändern, in der Marketo Kontakte mit Chancen für Erstkontakt- und Multi-Touch-Attribution, Lead-Konversionsmetriken und das Marketing-beeinflusste Opportunity-Flag verknüpft.

Diese Einstellungen wirken sich auf [!UICONTROL Umsatz-Explorer] -Berichte in den Bereichen [Analyse der Programmchancen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Opportunity Analysis](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) und Lead Analysis aus. Dies wirkt sich auch auf den Bericht [!UICONTROL Programm-Analyzer] aus.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicken Sie auf **[!UICONTROL Umsatzzyklusanalysen]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicken Sie auf den Link **[!UICONTROL Bearbeiten]** unter **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Durch Änderung dieser Einstellung werden keine Marketo-Daten geändert, sondern lediglich die Art und Weise, wie Ihre Berichte ausgeführt werden. Dies kann jederzeit rückgängig gemacht werden.

1. Wählen Sie eine Option aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Explizit]**: Nur Kontakte mit Rollen (Standard).
   >
   >**[!UICONTROL Hybrid]**: Kontaktiert die Rollen, sofern verfügbar. Wenn keine verfügbar sind, werden alle Kontakte in Konten verwendet.
   >
   >**[!UICONTROL Implizit]**: Alle Kontakte unabhängig von der Rolle.

>[!CAUTION]
>
>Bei Verwendung von **[!UICONTROL Implicit]** prüft Marketo immer alle mit dem Konto verknüpften Kontakte, unabhängig von der Rolle. **Marketo empfiehlt dringend die Verwendung von [!UICONTROL Explicit] mode**. Die Verwendung von [!UICONTROL implizit] kann zu falsch-positiven Ergebnissen führen, d. h. zu Personen, denen eine Chance zugeschrieben wird, obwohl sie keinen echten Einfluss auf die Chancen haben. Verwenden Sie [!UICONTROL Implicit] mit Vorsicht.
