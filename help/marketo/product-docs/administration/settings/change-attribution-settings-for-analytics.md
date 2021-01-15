---
unique-page-id: 2360217
description: Ändern der Zuordnungseinstellungen für Analytics - Marketing Docs - Produktdokumentation
title: Ändern der Zuordnungseinstellungen für Analytics
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Ändern der Zuordnungseinstellungen für Analytics {#change-attribution-settings-for-analytics}

Sie können die Art und Weise ändern, wie Marketo Kontakte mit Chancen für First- und Multi-Touch-Zuordnungen, Interessentenumrechnungsmetriken und die vom Marketing beeinflusste Opportunitätskennzeichnung verknüpft.

Diese Einstellungen wirken sich auf den Umsatz-Explorer-Bericht unter den Analysen [Programm-Chancen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Chancen-Analyse](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) und Interessentenanwerbung aus. Dies wirkt sich auch auf den Programm Analyzer-Bericht aus.

1. Klicken Sie im Abschnitt **Admin** auf **Umsatzwyklusanalyse**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Klicken Sie auf den Link **Bearbeiten** unter **Zuordnung**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >Durch Ändern dieser Einstellung werden keine Markierungsdaten geändert. Sie ändert lediglich die Ausführung Ihrer Berichte. Dies kann jederzeit rückgängig gemacht werden.

1. Wählen Sie eine Option und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**Explizit**: Nur Kontakte mit Rollen (Standard).
   >
   >**Hybrid**: Kontakte mit Rollen, sofern verfügbar. Wenn keine verfügbar sind, werden alle Kontakte in Konten verwendet.
   >
   >**Implizit**: Alle Kontakte unabhängig von der Rolle.

>[!CAUTION]
>
>Bei Verwendung von **Implizit** prüft Marketo immer alle mit dem Konto verknüpften Kontakte, unabhängig von der Rolle. **Marketo empfiehlt dringend die Verwendung des expliziten Modus**. Die Verwendung von Implizit kann zu Falsch-Positiv-Werten führen. d.h. Menschen, denen eine Chance zugeschrieben wird, obwohl sie keinen wirklichen Einfluss auf die Chancen haben. Verwenden Sie Implizit mit Vorsicht.
