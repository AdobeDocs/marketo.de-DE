---
unique-page-id: 15695924
description: Ranking und Tuning bei der Kontoprofilerstellung - Marketo-Dokumente - Produktdokumentation
title: Ranking und Optimierung für Kontoprofile
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# Ranking und Optimierung für Kontoprofile {#account-profiling-ranking-and-tuning}

Das Account Profiling identifiziert Ihr Ideal Customer Profile (ICP), ordnet Unternehmen in Ihrer Datenbank basierend auf dem ICP an und fügt ICP-Indikatoren-Daten zu Konten hinzu, die als benannte Konten beworben werden.

## Modellergebnisse {#model-results}

Die Ergebnisse zeigen Ihnen alle Ihre bekannten Konten aufgeschlüsselt nach Klasse. A ist die höchste Note, D ist die niedrigste.

![](assets/results.png)

Obwohl optional, empfehlen wir, das Kontrollkästchen Automatisch hochstufen zu aktivieren, da Sie dadurch viel Zeit sparen. Wenn Sie jedoch jedes Konto durchgehen und es [manuell hinzufügen](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts) möchten, lassen Sie einfach das Kontrollkästchen deaktiviert.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Rang</strong></td> 
   <td> 
    <div>
      Konto-Rang basierend auf dem Idealkundenprofil. A ist die beste Passform, D die am wenigsten passende. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Kauflust##</strong></td> 
   <td> 
    <div>
      Geschätzte Erhöhung der Konversionsrate im Vergleich zu einer nicht auf dem ICP basierenden Auswahl von Konten. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Konten (%)</strong></td> 
   <td> 
    <div>
      Prozentsatz der Konten in der Modelleingabe, die diesen Rang haben 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% der Modellbasis</strong></td> 
   <td> 
    <div>
      Prozentsatz der Konten auf Modellbasis mit diesem Rang. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Modellabstimmung {#model-tuning}

Klicken Sie auf der Registerkarte Modell auf die Schaltfläche Modell abstimmen .

![](assets/two.png)

Es stehen mehrere Registerkarten zur Auswahl, die eine gründliche Anpassung ermöglichen.

![](assets/tuning-page.png)

**Indikatorkategorien**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Compliance</strong></td> 
   <td> 
    <div>
      Zertifizierungen, Compliance-bezogene Stellen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Funktionsweise</strong></td> 
   <td> 
    <div>
      betriebliche Tätigkeiten/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>STD</strong></td> 
   <td> 
    <div>
      Personalwesen oder Lohn- und Gehaltsabrechnungssoftware, Stellenangebote/Einstellungen im Personalbereich.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Engineering</strong></td> 
   <td> 
    <div>
      Technologien, Rahmenbedingungen, ingenieurbezogene Stellen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vertrieb</strong></td> 
   <td> 
    <div>
      Lösungen und Software für Vertrieb, verkaufsbezogene Positionen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Absicht</strong></td> 
   <td> 
    <div>
      Absichtsindikatoren. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Hardware- und Softwarelösungen, Technologien, IT-bezogene Stellen/Einstellungen.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanzwesen</strong></td> 
   <td> 
    <div>
      Finanzsoftware, finanzbezogene Positionen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Marketingtechnologien und -software, Stellen/Einstellungen im Zusammenhang mit Marketing. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Business</strong></td> 
   <td> 
    <div>
      Forbes- oder Inc-Angebote oder Geschäftspartnerschaften. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Kundenerlebnis und Kundenbeziehungen</strong></td> 
   <td> 
    <div>
      Customer Success und Customer Relations-Positionen/Einstellungen.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Eine Beschreibung jeder Spalte finden Sie, wenn Sie den Mauszeiger über die QuickInfos bewegen.

![](assets/tool-tip.png)

Klicken Sie auf die Dropdown-Liste ICP-Indikator hinzufügen , um weitere Indikatoren in Ihr Modell einzufügen.

![](assets/add-icp.png)

Wenn Sie das Kontrollkästchen „Exportieren“ aktivieren, können Sie den ICP-Indikator auf der Seite mit den benannten Kontodetails anzeigen sowie den ausgewählten ICP-Indikator als Einschränkungen in [benannten Kontofiltern“ ](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>ICP-Indikatoren sind als Einschränkungen in **Mitglied eines spezifischen Kontos** Filtern und Triggern enthalten.

Die Indikatorgewichtung steuert die Wichtigkeit, die jeder Indikator in Ihrem Modell erhält.

![](assets/weightage.png)

Klicken Sie auf Modell aktualisieren , damit diese Änderungen wirksam werden.

![](assets/refresh-button.png)

Wenn Sie mit der Optimierung Ihres Modells fertig sind (nachdem Sie es aktualisiert haben), wechseln Sie zurück zur Registerkarte Modellergebnisse und klicken Sie auf **Ränge speichern und anwenden**.

![](assets/ranks.png)
