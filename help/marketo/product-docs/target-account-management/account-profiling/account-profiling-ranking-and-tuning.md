---
unique-page-id: 15695924
description: Ranking und Optimierung von Kontoprofilen - Marketo-Dokumente - Produktdokumentation
title: Ranking und Optimierung von Kontoprofilen
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# Ranking und Optimierung von Kontoprofilen {#account-profiling-ranking-and-tuning}

Mit der Kontoprofilerstellung wird Ihr ideales Kundenprofil (ICP) identifiziert, Unternehmen in Ihrer Datenbank werden auf der Grundlage des ICP in eine Rangfolge versetzt und ICP-Indikatordaten zu Konten hinzugefügt, die als benannte Konten beworben werden.

## Modellergebnisse {#model-results}

Die Ergebnisse zeigen Ihnen alle bekannten Konten aufgeschlüsselt nach Klassen. A ist die höchste Klasse, D die niedrigste.

![](assets/results.png)

Obwohl optional, empfehlen wir, das Kontrollkästchen Automatisch bewerben zu aktivieren, da dadurch eine Tonne Zeit eingespart wird. Wenn Sie jedoch jedes Konto durchgehen und [manuell hinzufügen](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts) möchten, lassen Sie das Kästchen einfach deaktiviert.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Rang</strong></td> 
   <td> 
    <div>
      Kontorang basierend auf dem Idealen Kundenprofil. A ist am besten geeignet, D am wenigsten geeignet. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Kauflust##</strong></td> 
   <td> 
    <div>
      Geschätzter Anstieg der Konversionsrate im Vergleich zu einer nicht auf dem VPI basierenden Kontoauswahl. 
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
      Prozentsatz der Konten auf Modellbasis mit diesem Rang. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Modellabstimmung {#model-tuning}

Klicken Sie auf der Registerkarte Modell auf die Schaltfläche Modell anpassen .

![](assets/two.png)

Es gibt mehrere Registerkarten, aus denen Sie eine detaillierte Anpassung durchführen können.

![](assets/tuning-page.png)

**Indikatorkategorien**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Konformität</strong></td> 
   <td> 
    <div>
      Zertifizierungen, Compliance-bezogene Positionen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Aktivitäten</strong></td> 
   <td> 
    <div>
      Betriebsbezogene Positionen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      HR- oder Payroll-Software, HR-bezogene Positionen/Vermietung.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ingenieurwesen</strong></td> 
   <td> 
    <div>
      Technologien, Frameworks, ingenieurbezogene Positionen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vertrieb</strong></td> 
   <td> 
    <div>
      Lösungen und Software für Vertrieb, Verkaufsstellen/Anmietung. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Absicht</strong></td> 
   <td> 
    <div>
      Intent-Indikatoren. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Hardware- und Software-Lösungen, Technologien, IT-bezogene Positionen/Einstellungen.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanzwesen</strong></td> 
   <td> 
    <div>
      Finanzsoftware, finanzbezogene Positionen/Anmietung. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Marketing-Technologien und -Software, Marketing-bezogene Positionen/Einstellungen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Unternehmen</strong></td> 
   <td> 
    <div>
      Forbes- oder Inc-Listen oder Geschäftspartnerschaften. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Kundenerlebnis und Kundenbeziehungen</strong></td> 
   <td> 
    <div>
      Kundenerfolg und Positionen/Einstellung für Kundenbeziehungen.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Bewegen Sie den Mauszeiger über die QuickInfos, um eine Beschreibung der einzelnen Spalten zu erhalten.

![](assets/tool-tip.png)

Klicken Sie auf die Dropdown-Liste ICP-Indikator hinzufügen , um weitere Indikatoren in Ihr Modell einzufügen.

![](assets/add-icp.png)

Wenn Sie das Feld &quot;Export&quot;aktivieren, wird der ICP-Indikator auf der Detailseite &quot;Named Account&quot;(Spezifisches Konto) angezeigt. Außerdem können Sie den ausgewählten ICP-Indikator als Begrenzungen in [benannten Kontofiltern](/help/marketo/product-docs/target-account-management/engage/account-filters.md) verwenden.

![](assets/export.png)

>[!NOTE]
>
>ICP-Indikatoren werden als Begrenzungen in Filtern und Triggern des Typs **Mitglied des benannten Kontos** einbezogen.

Die Indikatorgewichtung steuert die Wichtigkeitsstufe, die jeder Indikator in Ihrem Modell erhält.

![](assets/weightage.png)

Klicken Sie auf Modell aktualisieren , damit diese Änderungen wirksam werden.

![](assets/refresh-button.png)

Wenn Sie das Anpassen Ihres Modells abgeschlossen haben (nachdem Sie es aktualisiert haben), kehren Sie zur Registerkarte &quot;Modellergebnisse&quot;zurück und klicken Sie auf **Ränge speichern und anwenden**.

![](assets/ranks.png)
