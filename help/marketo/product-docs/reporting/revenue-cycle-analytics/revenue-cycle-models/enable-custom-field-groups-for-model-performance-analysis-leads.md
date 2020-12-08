---
unique-page-id: 3571890
description: Benutzerspezifische Feldgruppen für Analyse der Modellleistung (Interessenten) aktivieren - Marketing-Dokumente - Produktdokumentation
title: Benutzerspezifische Feldgruppen für Analyse der Modellleistung aktivieren (Interessenten)
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Benutzerspezifische Feldgruppen für Analyse der Modellleistung aktivieren (Interessenten) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!NOTE]
>
>**Voraussetzungen**
>
>Kategorisieren Sie Standard- oder benutzerdefinierte Felder zum Berichte in Gruppen über den Field Organizer in Marketing. Weitere Informationen finden Sie unter [Erstellen benutzerdefinierter Feldgruppen über den Feldorganisator](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>Wie wirkt sich die Aktivierung einer benutzerspezifischen Feldgruppe auf mehrere Analysen in Umsatz-Cycle Explorer aus?</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn...?</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Auswirkungen auf den Modellleistungsbereich (Interessenten) Analyse</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Auswirkungen auf die Bereiche Analyse, Analyse der Kampagne und Analyse von Chancen</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn Sie eine benutzerspezifische Feldgruppe aktivieren, die mit einem Standardfeld für Interessenten oder Firmen verknüpft ist?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Die benutzerspezifische Feldgruppe ist für den Berichte im Bereich Modellleistung (Interessenten) der Analyse aktiviert.</p></td> 
   <td colspan="1" rowspan="1"><p>Keine Auswirkung</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn Sie eine benutzerspezifische Feldgruppe aktivieren, die mit einem Feld für eine benutzerdefinierte Firma oder Person verknüpft ist?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Die benutzerspezifische Feldgruppe ist für den Berichte im Bereich Modellleistung (Interessenten) der Analyse aktiviert.</p></td> 
   <td colspan="1" rowspan="1"><p>Das benutzerdefinierte Feld selbst ist für den Berichte in den Analysen Interessentenanwerbung, Kampagne-Analyse und Chancen aktiviert.</p><p><strong>HINWEIS:</strong> Benutzerspezifische Feldgruppen werden in diesen Analysen NICHT unterstützt. Daher werden die Gruppenzuordnungen nicht im Umsatz-Cycle-Explorer angezeigt, sondern<em>nur</em> im benutzerdefinierten Feld.</p></td> 
  </tr> 
 </tbody> 
</table>

Führen Sie die folgenden Schritte aus, um eine benutzerspezifische Feldgruppe für den Berichte im Bereich Modellleistung (Interessenten) zu aktivieren.

1. Klicken Sie auf **Admin**.

   ![](assets/one-1.png)

1. Klicken Sie auf **Umsatzzyklusanalyse**.

   ![](assets/two-1.png)

1. Klicken Sie neben einer leeren Feldgruppe auf **Keine** . Wenn Sie bereits drei Feldgruppen aktiviert haben und eine Bearbeitung vornehmen möchten, klicken Sie auf den Namen der Feldgruppe, die Sie ändern möchten.

   ![](assets/three.png)

1. Klicken Sie auf die Dropdownliste **Feld** und wählen Sie das gewünschte Feld aus.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >In diesem Beispiel wurde eine benutzerspezifische Feldgruppe für ein Standardfeld (Status) aktiviert. Daher wurde nur der Bereich Modellleistung Analyse (Interessenten) beeinträchtigt. Wenn eine benutzerspezifische Feldgruppe für ein benutzerdefiniertes Firmen- oder Personenkreis aktiviert wurde, wird die aktivierte Gruppe im Bereich &quot;Modellleistung (Interessenten)&quot;der Registerkarte &quot;Zusammenfassung&quot;angezeigt und die Anzahl der benutzerspezifischen Felder für &quot;Interessent&quot;, &quot;Kampagne&quot;und &quot;Chancen&quot;-Analyse wird um 1 erhöht.

1. Klicken Sie auf **Speichern**.

   ![](assets/five-1.png)
