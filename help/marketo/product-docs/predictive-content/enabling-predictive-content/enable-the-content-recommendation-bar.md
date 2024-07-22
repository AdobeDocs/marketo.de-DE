---
unique-page-id: 4720108
description: Aktivieren der Symbolleiste für Inhaltsempfehlungen - Marketo-Dokumente - Produktdokumentation
title: Symbolleiste für Inhaltsempfehlung aktivieren
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Symbolleiste für Inhaltsempfehlung aktivieren {#enable-the-content-recommendation-bar}

Die Content Recommendation Engine verwendet prädiktive Analyse- und maschinelle Lernalgorithmen, um jedem Webbesucher relevante Inhalte bereitzustellen. Die Recommendations-Engine sagt für jeden Besucher voraus, welcher Inhalt die beste Leistung erbringt. Der Inhalt für die Engine wird unter der Recommendations-Seite überwacht und gesteuert, sodass Sie den ROI Ihrer Inhalte optimieren können.

>[!PREREQUISITES]
>
>Vor der Aktivierung des prädiktiven Inhalts müssen Sie:
>
>* **Bereiten Sie Ihren prädiktiven Inhalt vor**
>
>   * [Prädiktiven Inhalt für E-Mails bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) oder
>   * [Prädiktiven Inhalt für Rich Media bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) oder
>   * [Prädiktiven Inhalt für die Empfehlungsleiste bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Genehmigen eines Titels für prädiktiven Inhalt](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)

## Symbolleiste für Inhaltsempfehlung aktivieren und anpassen {#enable-and-customize-the-content-recommendation-bar}

1. Navigieren Sie zu **Inhaltseinstellungen**.

   ![](assets/settings-dropdown-hand.png)

1. Klicken Sie auf **Balken**.

   ![](assets/content-settings-bar-hand.png)

1. Um die Empfehlungsleiste für eine URL zu aktivieren, klicken Sie einfach auf **Ein** und dann auf **Speichern**.

   ![](assets/bar-enable.png)

1. Um eine URL anzupassen, wählen Sie Farben, Stil, Format, Pfeile für die Empfehlungsleiste und Seiten aus, die die Leiste ein- oder ausschließen sollen. Passen Sie an das Branding Ihrer Website an. Klicken Sie auf **Speichern**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Anzeige-URL einschließen/ausschließen**
   >
   >* Die Anzeigen-URL sollte der Pfad der Domäne sein.
   >* Schließen Sie https:// oder https:// nicht ein
   >* Verwenden Sie &#42; für Platzhalter
   * Semikolon als Trennzeichen verwenden
   * Beispiel: /contact_us&#42;; &#42;action=logout&#42;
   * Bei diesem Feld wird zwischen Groß- und Kleinschreibung unterschieden

## Überlegungen zur Empfehlungsleiste {#recommendation-bar-considerations}

* Sie benötigen mindestens ein Inhaltselement für die Empfehlungsleiste, das auf der Recommendations-Seite auf **Ein** gesetzt ist, damit die Empfehlungs-Engine funktioniert. Wenn kein Inhalt aktiviert ist und der Balken auf **Ein** eingestellt ist, wird der Pfeileffekt unten rechts auf der Webseite angezeigt, es werden jedoch keine empfohlenen Inhalte angezeigt.

* Je mehr Inhalte in der Empfehlungs-Engine ausgeführt werden, desto besser kann der Algorithmus testen und lernen, welche Inhalte am besten funktionieren. Es wird empfohlen, mit 10 bis 20 Inhaltselementen zu beginnen, die aktiv und aktiv sind, und weiterhin neue hinzuzufügen.
* Das Inhaltselement, das Sie für die Empfehlung aktivieren, sollte das RTP-JavaScript-Tag enthalten. Dies hilft dem Algorithmus, empfohlene Inhalte zu verfolgen und zu optimieren.

>[!MORELIKETHIS]
>
[Aktivieren von prädiktivem Inhalt für Web-Rich-Media](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
