---
unique-page-id: 2360217
description: Ändern der Attributionseinstellungen für Analytics - Marketo Docs - Produktdokumentation
title: Ändern der Attributionseinstellungen für Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 3%

---

# Ändern der Attributionseinstellungen für Analytics {#change-attribution-settings-for-analytics}

Sie können die Art und Weise ändern, in der Marketo Kontakte mit Chancen für Erstkontakt- und Multi-Touch-Attribution, Lead-Konversionsmetriken und das Marketing-beeinflusste Opportunity-Flag verknüpft.

Diese Einstellungen wirken sich auf den Umsatz-Explorer unter der [Analyse der Programmchancen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Opportunity Analysis](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)und Bereiche der Interessentenanalyse. Dies wirkt sich auch auf den Bericht Programm Analyzer aus.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicken **Umsatzzyklusanalysen**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicken Sie auf **Bearbeiten** Link unter **Attribution**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Durch Ändern dieser Einstellung werden keine Marketo-Daten geändert. Sie ändert lediglich die Ausführung Ihrer Berichte. Dies kann jederzeit rückgängig gemacht werden.

1. Wählen Sie eine Option aus und klicken Sie auf **Speichern**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**Explizit**: Nur Kontakte mit Rollen (Standard).
   >
   >**Hybrid**: Kontaktiert ggf. Rollen. Wenn keine verfügbar sind, werden alle Kontakte in Konten verwendet.
   >
   >**Implizit**: Alle Kontakte unabhängig von der Rolle.

>[!CAUTION]
>
>Bei Verwendung von **Implizit**, prüft Marketo immer alle mit dem Konto verknüpften Kontakte unabhängig von der Rolle. **Marketo empfiehlt dringend die Verwendung des expliziten Modus**. Die Verwendung von Implicit kann zu falsch-positiven Ergebnissen führen. d. h. Menschen, denen eine Chance zugeschrieben wird, obwohl sie keinen echten Einfluss auf die Chancen haben. Verwenden Sie Implicit mit Vorsicht.
