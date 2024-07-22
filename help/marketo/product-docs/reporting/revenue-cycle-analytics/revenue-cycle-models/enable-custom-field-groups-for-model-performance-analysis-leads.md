---
unique-page-id: 3571890
description: Benutzerdefinierte Feldergruppen für Modellleistungsanalyse (Leads) aktivieren - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Feldergruppen für Modellleistungsanalyse aktivieren (Leads)
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Benutzerdefinierte Feldergruppen für Modellleistungsanalyse aktivieren (Leads) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Kategorisieren Sie Standard- oder benutzerdefinierte Felder in Gruppen für die Berichterstellung über den Field Organizer in Marketo. Weitere Informationen finden Sie unter [Erstellen benutzerdefinierter Feldergruppen über den Feld-Organizer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>Wie wirkt sich die Aktivierung einer benutzerdefinierten Feldergruppe auf mehrere Analysebereiche in Umsatz-Cycle-Explorer aus?</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn...?</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Wie wirkt sich dies auf den Bereich "Modell Performance Analysis"(Leads) aus?</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Auswirkungen auf die Bereiche Lead Analysis, Kampagnenanalyse und Opportunity Analysis</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn Sie eine benutzerdefinierte Feldergruppe aktivieren, die mit einem standardmäßigen Lead- oder Firmenfeld verknüpft ist?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Die benutzerdefinierte Feldergruppe ist für die Berichterstellung im Bereich Modellleistungsanalyse (Leads) aktiviert.</p></td> 
   <td colspan="1" rowspan="1"><p>Keine Auswirkung</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn Sie eine benutzerdefinierte Feldergruppe aktivieren, die mit einem benutzerdefinierten Personen- oder Firmenfeld verknüpft ist?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Die benutzerdefinierte Feldergruppe ist für die Berichterstellung im Bereich Modellleistungsanalyse (Leads) aktiviert.</p></td> 
   <td colspan="1" rowspan="1"><p>Das benutzerdefinierte Feld selbst ist für die Berichterstellung in den Bereichen Lead-Analyse, Kampagnenanalyse und Opportunity Analysis aktiviert.</p><p><strong>HINWEIS:</strong> Benutzerdefinierte Feldergruppen werden in diesen Analysebereichen NICHT unterstützt, sodass die Gruppenzuordnungen nicht im Umsatz-Zyklus-Explorer angezeigt werden.—<em>Nur</em> im benutzerdefinierten Feld.</p></td> 
  </tr> 
 </tbody> 
</table>

Führen Sie diese Schritte aus, um eine benutzerdefinierte Feldergruppe für die Berichterstellung im Bereich Modell-Leistungsanalyse (Leads) zu aktivieren.

1. Klicken Sie auf **Admin**.

   ![](assets/one-1.png)

1. Klicken Sie auf **Umsatzzyklusanalysen**.

   ![](assets/two-1.png)

1. Klicken Sie neben einer leeren Feldergruppe auf **None** . Wenn Sie bereits drei Feldergruppen aktiviert haben und eine Bearbeitung vornehmen möchten, klicken Sie auf den Namen der Feldergruppe, die Sie ändern möchten.

   ![](assets/three.png)

1. Klicken Sie auf die Dropdownliste **Feld** und wählen Sie das gewünschte Feld aus.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >In diesem Beispiel wurde eine benutzerdefinierte Feldergruppe für ein Standardfeld (Status) aktiviert. Daher wurde nur der Bereich &quot;Modell Performance Analysis (Leads)&quot;betroffen. Wenn eine benutzerdefinierte Feldergruppe für ein benutzerdefiniertes Personen- oder Firmenfeld aktiviert wurde, würde die aktivierte Gruppe im Abschnitt &quot;Modell-Leistungsanalyse (Leads)&quot;der Registerkarte &quot;Zusammenfassung synchronisieren&quot;angezeigt und die Anzahl der benutzerdefinierten Felder für Lead, Kampagne und Opportunity Analysis würde um 1 erhöht.

1. Klicken Sie auf **Speichern**.

   ![](assets/five-1.png)
