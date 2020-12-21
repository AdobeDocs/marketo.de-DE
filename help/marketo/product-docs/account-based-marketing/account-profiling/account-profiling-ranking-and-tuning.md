---
unique-page-id: 15695924
description: Rangansicht und Abstimmung von Kontoprofilen - Marketing Docs - Produktdokumentation
title: Rangansicht und Abstimmung von Kontoprofilen
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Rangansicht und Abstimmung von Kontoprofilen {#account-profiling-ranking-and-tuning}

Die Kontoprofilerstellung identifiziert Ihr ideales Profil (ICP), sortiert Firmen in Ihrer Datenbank nach dem ICP und fügt ICP-Indikatordaten zu Konten hinzu, die als benannte Konten beworben werden.

## Modellergebnisse {#model-results}

Die Ergebnisse zeigen Ihnen alle bekannten Konten nach Besoldungsgruppe aufgeschlüsselt. A ist die höchste Klasse, D die niedrigste.

![](assets/results.png)

Obwohl optional, empfehlen wir, das Kontrollkästchen Automatisch fördern zu aktivieren, da es Ihnen eine Tonne Zeit einspart. Wenn Sie jedoch die einzelnen Konten durchlaufen und [sie manuell hinzufügen](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md#discover-crm-accounts) möchten, lassen Sie das Kontrollkästchen einfach deaktiviert.

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

**Indikator-Kategorien**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Compliance</strong></td> 
   <td> 
    <div>
      Zertifizierungen, Compliance-bezogene Positionen/Anmietung. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Aktivitäten</strong></td> 
   <td> 
    <div>
      Geschäftsbezogene Positionen/Vermietung. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      HR- oder Payroll-Software, HR-bezogene Positionen/Miete.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Engineering</strong></td> 
   <td> 
    <div>
      Technologien, Frameworks, ingenieurbezogene Positionen/Miete. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vertrieb</strong></td> 
   <td> 
    <div>
      Lösungen und Software für Vertrieb, Verkaufsstellen/Vermietung. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Zweck</strong></td> 
   <td> 
    <div>
      Zielindikatoren. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Hardware- und Softwarelösungen, Technologien, IT-bezogene Positionen/Miete.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finance</strong></td> 
   <td> 
    <div>
      Finanz-Software, finanzbezogene Positionen/Miete. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Marketing-Technologien und Software, Marketing-bezogene Positionen/Miete. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Geschäft</strong></td> 
   <td> 
    <div>
      Forbes oder Inc Listen oder Geschäftspartnerschaften. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Kundenerlebnis und Kundenbeziehungen</strong></td> 
   <td> 
    <div>
      Kundenerfolg und Kundenbeziehungen Positionen/Vermietung.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Bewegen Sie den Mauszeiger über die QuickInfos, um eine Beschreibung der einzelnen Spalten anzuzeigen.

![](assets/tool-tip.png)

Klicken Sie auf die Dropdownliste Hinzufügen ICP-Indikator, um weitere Indikatoren in Ihr Modell einzufügen.

![](assets/add-icp.png)

Wenn Sie das Kontrollkästchen &quot;Exportieren&quot;aktivieren, können Sie den ICP-Indikator auf der Seite &quot;Benanntes Konto&quot;anzeigen und den ausgewählten ICP-Indikator als Einschränkungen unter [Benannte Filter](/help/marketo/product-docs/account-based-marketing/engage/account-filters.md) verwenden.

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
