---
unique-page-id: 4720108
description: Aktivieren der Inhaltsempfehlungsleiste - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der Inhaltsempfehlungsleiste
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Aktivieren der Inhaltsempfehlungsleiste {#enable-the-content-recommendation-bar}

Die Inhaltsempfehlungs-Engine verwendet prädiktive Analysen und Algorithmen des maschinellen Lernens, um jedem Web-Besucher relevante Inhalte bereitzustellen. Die Recommendations-Engine sagt voraus, welche Inhalte pro Besucher am besten funktionieren würden. Der Inhalt für die Engine wird unter der Recommendations-Seite überwacht und gesteuert, sodass Sie Ihren Inhalts-ROI optimieren können.

>[!PREREQUISITES]
>
>Bevor Sie prädiktive Inhalte aktivieren, müssen Sie:
>
>* **Prädiktive Inhalte vorbereiten**
>
>   * [Prädiktiven Inhalt für E-Mails bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) oder
>   * [Bearbeiten prädiktiver Inhalte für Rich Media](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) oder
>   * [Bearbeiten prädiktiver Inhalte für die Empfehlungsleiste](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Genehmigen eines Titels für Prognoseinhalte](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)

## Aktivieren und Anpassen der Inhaltsempfehlungsleiste {#enable-and-customize-the-content-recommendation-bar}

1. Navigieren Sie **Inhaltseinstellungen**.

   ![](assets/settings-dropdown-hand.png)

1. Klicken Sie auf **Leiste**.

   ![](assets/content-settings-bar-hand.png)

1. Um die Empfehlungsleiste für eine URL zu aktivieren, klicken Sie einfach auf **Ein** und dann **Speichern**.

   ![](assets/bar-enable.png)

1. Um eine URL anzupassen, wählen Sie Farben, Stil, Format, Pfeile für die Empfehlungsleiste und Seiten, auf denen die Leiste ein- oder ausgeschlossen werden soll. Passen Sie es an Ihr Website-Branding an. Klicken Sie auf **Speichern**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Anzeige-URL einschließen/ausschließen**
   >
   >* Anzeige-URL sollte der Pfad der Domain sein
   >* Schließen Sie weder https:// noch https:// ein.
   >* &#42; für Platzhalter verwenden
   >* Semikolon als Trennzeichen verwenden
   >* Beispiel: /contact_us&#42;; &#42;action=logout&#42;
   >* Bei diesem Feld wird zwischen Groß- und Kleinschreibung unterschieden

## Überlegungen zur Empfehlungsleiste {#recommendation-bar-considerations}

* Sie benötigen mindestens ein Inhaltselement, damit die Empfehlungsleiste auf der Recommendations **Seite auf „Ein** gesetzt wird, damit die Empfehlungs-Engine funktioniert. Wenn kein Inhalt aktiviert ist und die Leiste auf **Ein** eingestellt ist, wird der Pfeileffekt unten rechts auf der Web-Seite angezeigt, es werden jedoch keine empfohlenen Inhalte angezeigt.

* Je mehr Inhalte in der Recommendations-Engine ausgeführt werden, desto besser für den Algorithmus, zu testen und zu lernen, welche Inhalte am besten funktionieren. Es wird empfohlen, mit der Ausführung und Aktivierung von 10 bis 20 Inhaltsfragmenten zu beginnen und weitere neue hinzuzufügen.
* Der Inhalt, den Sie für eine Empfehlung aktivieren, sollte das RTP-JavaScript-Tag enthalten. Dies hilft dem Algorithmus, empfohlene Inhalte zu verfolgen und zu optimieren.

>[!MORELIKETHIS]
>
>[Prädiktive Inhalte für Web-Rich-Media aktivieren](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
