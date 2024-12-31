---
unique-page-id: 3571890
description: Aktivieren benutzerdefinierter Feldergruppen für Modellleistungsanalyse (Leads) - Marketo-Dokumente - Produktdokumentation
title: Aktivieren von benutzerdefinierten Feldergruppen für die Modellleistungsanalyse (Leads)
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Aktivieren von benutzerdefinierten Feldergruppen für die Modellleistungsanalyse (Leads) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Kategorisieren Sie standardmäßige oder benutzerdefinierte Felder in Gruppen für das Reporting über den Feld-Organisator in Marketo. Weitere Informationen finden Sie unter [Erstellen benutzerdefinierter Feldergruppen über den Feld-Organisator](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>Wie wirkt sich die Aktivierung einer benutzerdefinierten Feldergruppe auf mehrere Analysebereiche im Umsatzzyklus-Explorer aus?</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn…?</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Auswirkungen auf den Bereich Modellleistungsanalyse (Leads)</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Auswirkungen auf die Bereiche Lead-Analyse, Kampagnenanalyse und Opportunity-Analyse</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn Sie eine benutzerdefinierte Feldergruppe aktivieren, die mit einem standardmäßigen Lead- oder Firmenfeld verknüpft ist?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Die benutzerdefinierte Feldergruppe ist für das Reporting im Bereich Modellleistungsanalyse (Leads) aktiviert</p></td> 
   <td colspan="1" rowspan="1"><p>Keine Auswirkung</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Was passiert, wenn Sie eine benutzerdefinierte Feldergruppe aktivieren, die mit einem benutzerdefinierten Personen- oder Firmenfeld verknüpft ist?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Die benutzerdefinierte Feldergruppe ist für das Reporting im Bereich Modellleistungsanalyse (Leads) aktiviert</p></td> 
   <td colspan="1" rowspan="1"><p>Das benutzerdefinierte Feld selbst ist für das Reporting in den Bereichen Lead-Analyse, Kampagnenanalyse und Opportunity-Analyse aktiviert.</p><p><strong>HINWEIS</strong> Benutzerdefinierte Feldergruppen werden in diesen Analysebereichen NICHT unterstützt, sodass die Gruppenverknüpfungen im Umsatzzyklus-Explorer nicht (<em>) </em> benutzerdefinierten Feld angezeigt werden.</p></td> 
  </tr> 
 </tbody> 
</table>

Führen Sie die folgenden Schritte aus, um eine benutzerdefinierte Feldergruppe für das Reporting im Bereich Modellleistungsanalyse (Leads) zu aktivieren.

1. Klicken Sie auf **Admin**.

   ![](assets/one-1.png)

1. Klicken Sie **Umsatzzyklusanalyse**.

   ![](assets/two-1.png)

1. Klicken Sie **Keine** neben einer leeren Feldergruppe. Wenn Sie bereits drei Feldergruppen aktiviert haben und eine Bearbeitung vornehmen möchten, klicken Sie auf den Namen der Feldergruppe, die Sie ändern möchten.

   ![](assets/three.png)

1. Klicken Sie auf **Feld** und wählen Sie das gewünschte aus.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >In diesem Beispiel wurde eine benutzerdefinierte Feldergruppe für ein Standardfeld (Status) aktiviert. Daher war nur der Bereich Modellleistungsanalyse (Leads) betroffen. Wenn eine benutzerdefinierte Feldergruppe für ein benutzerdefiniertes Personen- oder Unternehmensfeld aktiviert worden wäre, würde die aktivierte Gruppe im Abschnitt „Lead-Performance-Analyse“ auf der Registerkarte „Zusammenfassung synchronisieren“ angezeigt und die benutzerdefinierte Felderanzahl für Lead-, Kampagnen- und Opportunity-Analyse würde um eins steigen.

1. Klicken Sie auf **Speichern**.

   ![](assets/five-1.png)
