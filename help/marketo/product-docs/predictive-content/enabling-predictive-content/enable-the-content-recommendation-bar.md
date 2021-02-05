---
unique-page-id: 4720108
description: Symbolleiste zur Inhaltsempfehlung - Marketing-Dokumente - Produktdokumentation
title: Symbolleiste für die Inhaltsempfehlung aktivieren
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---


# Inhaltsempfehlung-Leiste {#enable-the-content-recommendation-bar} aktivieren

Die Content Recommendation Engine verwendet Algorithmen für Prognoseanalyse und maschinelles Lernen, um relevante Inhalte für jeden Web-Besucher bereitzustellen. Die Recommendations-Engine prognostiziert, welche Inhalte pro Besucher am besten funktionieren. Die Inhalte für die Engine werden unter der Recommendations-Seite überwacht und gesteuert, was Ihnen bei der Optimierung Ihrer Content-ROI hilft.

>[!PREREQUISITES]
>
>Bevor Sie Prognostizierende Inhalte aktivieren, müssen Sie Folgendes tun:
>
>* [Vorbereitung von prädiktiven Inhalten](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [Genehmigen eines Titels für prädiktive Inhalte](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Aktivieren und Anpassen der Inhaltsempfehlung-Leiste {#enable-and-customize-the-content-recommendation-bar}

1. Gehen Sie zu **Inhaltseinstellungen**.

   ![](assets/settings-dropdown-hand.png)

1. Klicken Sie auf **Leiste**.

   ![](assets/content-settings-bar-hand.png)

1. Um die Empfehlungsleiste für eine URL zu aktivieren, klicken Sie einfach auf **Ein** und dann auf **Speichern**.

   ![](assets/bar-enable.png)

1. Um eine URL anzupassen, wählen Sie Farben, Stil, Format, Pfeile für die Empfehlungsleiste und Seiten aus, die die Leiste ein- oder ausschließen sollen. Passen Sie die Markendarstellung Ihrer Website an. Klicken Sie auf **Speichern**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Anzeigen-URL einschließen/ausschließen**
   >
   >    * Die Anzeigen-URL sollte der Pfad der Domäne sein.
   >    * http:// oder https:// nicht einschließen
   >    * * für Platzhalter verwenden
   * Semikolon als Trennzeichen verwenden
   * Beispiel: /contact_us*; *action=logout*
   * Bei diesem Feld ist die Groß-/Kleinschreibung zu beachten


## Überlegungen zur Empfehlungsleiste {#recommendation-bar-considerations}

* Sie benötigen mindestens ein Inhaltselement, damit die Recommendations-Engine auf der Recommendations-Seite auf **Ein** eingestellt ist. Wenn kein Inhalt aktiviert ist und die Leiste auf **Ein** eingestellt ist, wird der Pfeil-Effekt unten rechts auf der Webseite angezeigt, es werden jedoch keine empfohlenen Inhalte angezeigt.

* Je mehr Inhalte in der Recommendations-Engine ausgeführt werden, desto besser kann der Algorithmus testen und lernen, welche Inhalte am besten funktionieren. Es wird empfohlen, mit 10 bis 20 Inhaltselementen zu beginnen, die aktiv und aktiv sind, und immer neue hinzufügen.
* Das Inhaltselement, das Sie für eine Empfehlung aktivieren, sollte das RTP-Javascript-Tag enthalten. Dies hilft dem Algorithmus, empfohlene Inhalte zu verfolgen und zu optimieren.

>[!MORELIKETHIS]
* [Predictive Content für Web Rich Media aktivieren](enable-predictive-content-for-web-rich-media.md)

