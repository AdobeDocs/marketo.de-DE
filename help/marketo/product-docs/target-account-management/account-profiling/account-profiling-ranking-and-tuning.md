---
unique-page-id: 15695924
description: Ranking und Tuning bei der Kontoprofilerstellung - Marketo-Dokumente - Produktdokumentation
title: Ranking und Optimierung für die Kontoprofilierung
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 6%

---

# Ranking und Optimierung für die Kontoprofilierung {#account-profiling-ranking-and-tuning}

Das Account Profiling identifiziert Ihr Ideal Customer Profile (ICP), ordnet Unternehmen in Ihrer Datenbank basierend auf dem ICP an und fügt ICP-Indikatordaten zu Konten hinzu, die als [!UICONTROL Named Accounts“ &#x200B;] werden.

>[!IMPORTANT]
>
>Ab 2025 ist die Kontoprofilerstellung für neue Benutzer nicht mehr verfügbar. Dies funktioniert weiterhin für bestehende Benutzer.

## Modellergebnisse {#model-results}

Die Ergebnisse zeigen Ihnen alle Ihre bekannten Konten aufgeschlüsselt nach Klasse. A ist die höchste Note, D ist die niedrigste.

![](assets/results.png)

Obwohl optional, empfehlen wir, das Kontrollkästchen Automatisch hochstufen zu aktivieren, da Sie dadurch viel Zeit sparen. Wenn Sie jedoch jedes Konto durchgehen und es [manuell hinzufügen](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts) möchten, lassen Sie einfach das Kontrollkästchen deaktiviert.

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Rang</span></strong></td>
   <td>
    <div>
      Konto-Rang basierend auf dem Idealkundenprofil. A ist die beste Passform, D die am wenigsten passende.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Kauflust##</span></strong></td>
   <td>
    <div>
      Geschätzte Erhöhung der Konversionsrate im Vergleich zu einer nicht auf dem ICP basierenden Auswahl von Konten.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Konten (%)</span></strong></td>
   <td>
    <div>
      Prozentsatz der Konten in der Modelleingabe, die diesen Rang haben
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">% der Modellbasis</span></strong></td>
   <td>
    <div>
      Prozentsatz der Konten auf Modellbasis mit diesem Rang.
    </div></td>
  </tr>
 </tbody>
</table>

## Modellabstimmung {#model-tuning}

Klicken Sie auf der Registerkarte Modell auf die Schaltfläche **[!UICONTROL Modell]**.

![](assets/two.png)

Es stehen mehrere Registerkarten zur Auswahl, die eine gründliche Anpassung ermöglichen.

![](assets/tuning-page.png)

**Indikatorkategorien**

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Compliance</span></strong></td>
   <td>
    <div>
      Zertifizierungen, Compliance-bezogene Stellen/Einstellungen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Funktionsweise</span></strong></td>
   <td>
    <div>
      betriebliche Tätigkeiten/Einstellungen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">STD</span></strong></td>
   <td>
    <div>
      Personalwesen oder Lohn- und Gehaltsabrechnungssoftware, Stellenangebote/Einstellungen im Personalbereich.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Engineering</span></strong></td>
   <td>
    <div>
      Technologien, Rahmenbedingungen, ingenieurbezogene Stellen/Einstellungen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Vertrieb</span></strong></td>
   <td>
    <div>
      Lösungen und Software für Vertrieb, verkaufsbezogene Positionen/Einstellungen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Absicht</span></strong></td>
   <td>
    <div>
      Absichtsindikatoren.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">IT</span></strong></td>
   <td>
    <div>
      Hardware- und Softwarelösungen, Technologien, IT-bezogene Stellen/Einstellungen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Finanzwesen</span></strong></td>
   <td>
    <div>
      Finanzsoftware, finanzbezogene Positionen/Einstellungen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Marketing</span></strong></td>
   <td>
    <div>
      Marketingtechnologien und -software, Stellen/Einstellungen im Zusammenhang mit Marketing.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Business</span></strong></td>
   <td>
    <div>
      Forbes- oder Inc-Angebote oder Geschäftspartnerschaften.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Kundenerlebnis und Kundenbeziehungen</span></strong></td>
   <td>
    <div>
      Customer Success und Customer Relations-Positionen/Einstellungen.
    </div></td>
  </tr>
 </tbody>
</table>

Eine Beschreibung jeder Spalte finden Sie, wenn Sie den Mauszeiger über die QuickInfos bewegen.

![](assets/tool-tip.png)

Klicken Sie auf [!UICONTROL ICP-Indikator hinzufügen], um weitere Indikatoren in Ihr Modell einzufügen.

![](assets/add-icp.png)

Wenn Sie das Kästchen [!UICONTROL Exportieren] aktivieren, können Sie den ICP-Indikator auf der Detailseite [!UICONTROL Benanntes Konto] sowie den ausgewählten ICP-Indikator als Einschränkungen in [benannten Kontofiltern“ &#x200B;](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>ICP-Indikatoren sind als Einschränkungen in **[!UICONTROL Mitglied eines spezifischen Kontos]** Filtern und Triggern enthalten.

[!UICONTROL Indikatorgewichtung] steuert die Wichtigkeit, die jeder Indikator in Ihrem Modell erhält.

![](assets/weightage.png)

Klicken Sie **[!UICONTROL Modell aktualisieren]** damit diese Änderungen wirksam werden.

![](assets/refresh-button.png)

Wenn Sie mit der Optimierung Ihres Modells fertig sind (nachdem Sie es aktualisiert haben), wechseln Sie zurück zur Registerkarte Modellergebnisse und klicken Sie auf **[!UICONTROL Ränge speichern und anwenden]**.

![](assets/ranks.png)
