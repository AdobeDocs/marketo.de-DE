---
unique-page-id: 2360217
description: Ändern der Attributionseinstellungen für Analytics - Marketo Docs - Produktdokumentation
title: Ändern der Attributionseinstellungen für Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Ändern der Attributionseinstellungen für Analytics {#change-attribution-settings-for-analytics}

Sie können die Art und Weise ändern, in der Marketo Kontakte mit Chancen für Erstkontakt- und Multi-Touch-Attribution, Lead-Konversionsmetriken und das Marketing-beeinflusste Opportunity-Flag verknüpft.

Diese Einstellungen wirken sich auf den Umsatz-Explorer unter der [Analyse der Programmchancen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Opportunity Analysis](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)und Bereiche der Interessentenanalyse. Dies wirkt sich auch auf den Bericht Programm Analyzer aus.

1. Unter dem **Admin** Abschnitt, klicken Sie auf **Umsatzzyklusanalysen**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Klicken Sie auf **Bearbeiten** Link unter **Attribution**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >Durch Ändern dieser Einstellung werden keine Marketo-Daten geändert. Sie ändert lediglich die Ausführung Ihrer Berichte. Dies kann jederzeit rückgängig gemacht werden.

1. Wählen Sie eine Option aus und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

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
