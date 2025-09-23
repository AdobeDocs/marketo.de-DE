---
unique-page-id: 2360217
description: Attributionseinstellungen für Analytics ändern - Marketo-Dokumente - Produktdokumentation
title: Ändern der Attributionseinstellungen für Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 5%

---

# Ändern der Attributionseinstellungen für Analytics {#change-attribution-settings-for-analytics}

Sie können die Art und Weise ändern, wie Marketo Kontakte mit Opportunities für Erstkontakt- und Mehrfachkontakt-Attribution, Lead-Konversionsmetriken und der Marketing-beeinflussten Opportunity-Markierung verknüpft.

Diese Einstellungen wirken sich auf [!UICONTROL Umsatz-Explorer] Berichte in den [Programm-](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Opportunity-](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) und Lead-Analyse aus. Dies wirkt sich auch auf den Bericht [!UICONTROL Programm-]&quot; aus.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicken Sie **[!UICONTROL Umsatzzyklusanalyse]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicken Sie auf den **[!UICONTROL Bearbeiten]**-Link unter **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Wenn Sie diese Einstellung ändern, werden keine Marketo-Daten geändert, sondern lediglich die Ausführung Ihrer Berichte. Dies kann jederzeit rückgängig gemacht werden.

1. Wählen Sie eine Option aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Explicit]**: Nur Kontakte mit Rollen (Standard).
   >
   >**[!UICONTROL Hybrid]**: Kontakte mit Rollen, falls verfügbar. Wenn keine verfügbar sind, werden alle Kontakte in Konten verwendet.
   >
   >**[!UICONTROL Implizit]**: Alle Kontakte unabhängig von der Rolle.

>[!CAUTION]
>
>Bei Verwendung von **[!UICONTROL implizit]** prüft Marketo immer alle mit dem Konto verknüpften Kontakte, unabhängig von der Rolle. **Marketo empfiehlt dringend die Verwendung [!UICONTROL expliziten] Modus**. Die Verwendung von [!UICONTROL Implicit] kann zu falsch positiven Ergebnissen führen, d. h. zu Personen, die eine Opportunity guthaben, obwohl sie keinen echten Einfluss auf die Opportunity haben. Verwenden Sie [!UICONTROL implizit] mit Vorsicht.
