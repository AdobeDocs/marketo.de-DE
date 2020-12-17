---
unique-page-id: 15695924
description: Rangansicht und Abstimmung von Kontoprofilen - Marketing Docs - Produktdokumentation
title: Rangansicht und Abstimmung von Kontoprofilen
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# Rangansicht und Abstimmung von Kontoprofilen {#account-profiling-ranking-and-tuning}

Die Kontoprofilerstellung identifiziert Ihr ideales Profil (ICP), sortiert Firmen in Ihrer Datenbank nach dem ICP und fügt ICP-Indikatordaten zu Konten hinzu, die als benannte Konten beworben werden.

## Modellergebnisse {#model-results}

Die Ergebnisse zeigen Ihnen alle bekannten Konten nach Besoldungsgruppe aufgeschlüsselt. A ist die höchste Klasse, D die niedrigste.

![](assets/results.png)

Obwohl optional, empfehlen wir, das Kontrollkästchen Automatisch fördern zu aktivieren, da es Ihnen eine Tonne Zeit einspart. Wenn Sie jedoch die einzelnen Konten durchlaufen und [sie manuell hinzufügen](http://docs.marketo.com/display/DOCS/Discover+Accounts#DiscoverAccounts-DiscoverCRMAccounts) möchten, lassen Sie das Kontrollkästchen einfach deaktiviert.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Rang</strong></td> 
   <td> 
    <div>
      Kontostand basierend auf dem Ideal Customer Profil. A ist am besten geeignet, D am wenigsten geeignet. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Tendenz</strong></td> 
   <td> 
    <div>
      Geschätzte Steigerung des Konversionsraten im Vergleich zu einer nicht auf dem VPI basierenden Kontenauswahl. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Konten (%)</strong></td> 
   <td> 
    <div>
      Prozentsatz der Konten in Modelleingaben mit diesem Rang. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% der Modellgrundlage</strong></td> 
   <td> 
    <div>
      Prozentsatz der Konten auf Modellbasis, die diesen Rang haben. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Modelloptimierung {#model-tuning}

Klicken Sie auf der Registerkarte Modell auf die Schaltfläche Modell anpassen.

![](assets/two.png)

Es stehen verschiedene Registerkarten zur Auswahl, die eine detaillierte Anpassung ermöglichen.

![](assets/tuning-page.png)

Indikator-Kategorien

| **Compliance** | Zertifizierungen, Compliance-bezogene Positionen/Anmietung. |
|---|---|
| **Aktivitäten** | Geschäftsbezogene Positionen/Vermietung. |
| **HR** | HR- oder Payroll-Software, HR-bezogene Positionen/Miete. |
| **Engineering** | Technologien, Frameworks, ingenieurbezogene Positionen/Miete. |
| **Vertrieb** | Lösungen und Software für Vertrieb, Verkaufsstellen/Vermietung. |
| **Zweck** | Zielindikatoren. |
| **IT** | Hardware- und Softwarelösungen, Technologien, IT-bezogene Positionen/Miete. |
| **Finance** | Finanz-Software, finanzbezogene Positionen/Miete. |
| **Marketing** | Marketing-Technologien und Software, Marketing-bezogene Positionen/Miete. |
| **Geschäft** | Forbes oder Inc Listen oder Geschäftspartnerschaften. |
| **Kundenerlebnis und Kundenbeziehungen** | Kundenerfolg und Kundenbeziehungen Positionen/Vermietung. |

Bewegen Sie den Mauszeiger über die QuickInfos, um eine Beschreibung der einzelnen Spalten anzuzeigen.

![](assets/tool-tip.png)

Klicken Sie auf die Dropdownliste Hinzufügen ICP-Indikator, um weitere Indikatoren in Ihr Modell einzufügen.

![](assets/add-icp.png)

Wenn Sie das Kontrollkästchen &quot;Exportieren&quot;aktivieren, können Sie den ICP-Indikator auf der Seite &quot;Benanntes Konto&quot;anzeigen und den ausgewählten ICP-Indikator als Einschränkungen unter [Benannte Filter](http://docs.marketo.com/display/DOCS/Account+Filters) verwenden.

![](assets/export.png)

>[!NOTE]
>
>ICP-Indikatoren werden als Einschränkungen in den Filtern und Auslöser von **Mitglied des benannten Kontos** einbezogen.

Die Indikatorgewichtung steuert die Wichtigkeitsstufe, die jeder Indikator in Ihrem Modell erhält.

![](assets/weightage.png)

Klicken Sie auf Modell aktualisieren, damit diese Änderungen wirksam werden.

![](assets/refresh-button.png)

Wenn Sie das Anpassen des Modells abgeschlossen haben (nachdem Sie es aktualisiert haben), kehren Sie zur Registerkarte Modellergebnisse zurück und klicken Sie auf **Ränge speichern und anwenden**.

![](assets/ranks.png)

