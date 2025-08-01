---
description: Übersicht über die Interaktionskarte - Marketo-Dokumente - Produktdokumentation
title: Interaktionskarte - Übersicht
exl-id: 01cb283d-06c2-4a99-86a9-39dea9550c08
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Interaktionskarte - Übersicht {#engagement-map-overview}

Mit der Interaktionskarte können Sie Ihre Smart-Kampagnen intuitiv visualisieren. Es bietet vollständige Abwärtskompatibilität mit allen bestehenden Marketo Engage Smart-Kampagnen, ohne dass aktuelle Funktionen verloren gehen.

>[!NOTE]
>
>Interaktionszuordnung ist derzeit in intelligenten Kampagnen verfügbar. Es ist nicht in Programmen verfügbar.

![](assets/engagement-map-overview-1.png)

## Zugriff auf Interaktionszuordnung {#accessing-engagement-map}

Navigieren Sie zu einer beliebigen vorhandenen Kampagne und klicken Sie auf **Schaltfläche** Interaktionszuordnung“.

![](assets/engagement-map-overview-2.png)

In der Interaktionskarte werden zwei Registerkarten angezeigt: [Interaktionskarte](/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-tab.md){target="_blank"} und [Einstellungen](/help/marketo/product-docs/core-marketo-concepts/engagement-map/settings-tab.md){target="_blank"}.

![](assets/engagement-map-overview-3.png)

## Kartenbeschreibungen {#card-descriptions}

**Trigger**: In Kampagnen, die Trigger enthalten, verfügt die Zuordnung über eine Karte &quot;Trigger-Übersicht“. Wenn Sie darauf klicken, wird für jeden Trigger eine Karte sowie ein ausklappbares Bedienfeld mit zusätzlichen Informationen angezeigt.

**Filter**: In Kampagnen, die Filter enthalten, enthält die Zuordnung eine Karte „Filterübersicht“. Wenn Sie darauf klicken, wird ein ausklappbares Bedienfeld mit zusätzlichen Informationen zu jedem Filter angezeigt.

**Flussschritte**: Jede Kampagne enthält eine Karte für jeden Flussschritt. Wenn Sie darauf klicken, wird ein ausklappbares Bedienfeld mit zusätzlichen Informationen angezeigt.

**Wahlen**: Wenn ein Flussschritt eine oder mehrere Auswahlmöglichkeiten enthält, wird beim Klicken auf die Flusskarte für jede Auswahl eine Karte sowie ein ausklappbares Bedienfeld mit zusätzlichen Informationen angezeigt.

## Verschachtelte Kampagnen {#nested-campaigns}

* Wenn eine Kampagne den Schritt Kampagnenfluss anfordern oder ausführen enthält, werden beim Klicken auf die Flusskarte Details zur aufgerufenen Kampagne sowie ein ausklappbares Bedienfeld mit zusätzlichen Informationen angezeigt.

* Wenn eine Kampagne den Schritt Kampagnenfluss anfordern oder ausführen mit Auswahlmöglichkeiten enthält, wird beim Klicken auf die Flusskarte für jede Auswahl eine Karte sowie ein ausklappbares Bedienfeld mit weiteren Informationen zu den Auswahlmöglichkeiten angezeigt. Wenn Sie auf eine Auswahlkarte klicken, werden Details zur aufgerufenen Kampagne sowie ein ausklappbares Bedienfeld mit weiteren Informationen angezeigt.

* Wenn eine der verschachtelten Kampagnen über den Schritt Kampagnenfluss anfordern oder ausführen verfügt, werden beim Klicken auf die Flusskarte außerdem Details zur Kampagne angezeigt. Dasselbe gilt, wenn der Flussschritt Auswahlmöglichkeiten enthält.

## Navigation oben {#top-navigation}

Die obere Navigationsleiste enthält die folgenden Funktionen:

* Kampagnenname und Zugriff auf das Modal „Kampagne bearbeiten“. Der Kampagnenname und die Beschreibung können hier bearbeitet werden.

* Der Kampagnenstatus und der Kampagnentyp werden unter dem Kampagnennamen angezeigt.

* Schaltfläche „Aktivieren/Deaktivieren“ für Trigger-Kampagnen

* Smart-Liste bearbeiten - Sie werden in einer neuen Registerkarte zur Benutzeroberfläche der Smart-Liste navigiert, wo Sie Ihre Filter und/oder Trigger hinzufügen oder bearbeiten können

* Fluss bearbeiten - Sie werden in einer neuen Registerkarte zur Fluss -Oberfläche navigiert, wo Sie Ihre Flussschritte hinzufügen oder bearbeiten können.

* Exportieren : Dadurch wird ein Bild der Kampagnenvisualisierung heruntergeladen. Die heruntergeladene Version spiegelt alle Verzweigungen wider, die Sie erweitert haben

* Kampagnenmitglieder anzeigen - Dadurch wird eine neue Registerkarte mit Details zum Kampagnenmitglied geöffnet.

>[!NOTE]
>
>Änderungen, die in einer geöffneten Smart-Liste und auf einer geöffneten Fluss-Registerkarte vorgenommen wurden, werden bei der Aktualisierung auf der Registerkarte Interaktionszuordnung angezeigt. Sie wird nicht automatisch aktualisiert. Aktualisierungen und Bearbeitungen, die automatisch gespeichert werden, werden nach der Aktualisierung der Registerkarte Interaktionszuordnung angezeigt.

## FAQs {#faq}

**Muss ich alle meine Kampagnen in der Interaktionskarte neu erstellen?**

Nein. Interaktionszuordnung ist vollständig abwärtskompatibel. Mit einem Klick auf eine Schaltfläche können Sie jede Ihrer vorhandenen Kampagnen in der visuellen Interaktionskarte anzeigen.

**Bedeutet Engagement Map in Marketo Engage, dass ich den Zugriff auf die Ordnerstruktur verliere und erneut lernen muss, wie man eine Smart Campaign erstellt?**

Nein. Das Tolle an Engagement Map ist, dass sie das Beste aus beiden Welten bietet. Sie ergänzt die derzeitige Art und Weise, wie Kampagnen erstellt werden. Alle Anwender erhalten weiterhin die leistungsstarken Funktionen von Marketo Engage, die nun durch klare visuelle Elemente ergänzt werden.

**Ist Engagement Map ein kostenpflichtiges Add-on?**

Nein. Alle bestehenden und neuen Marketo Engage-Benutzer unter allen Abonnements haben Zugriff auf diese kostenlose Funktion.

**Bin ich als Marketo Engage-Administrator dafür verantwortlich, die Interaktionskarte zu aktivieren/deaktivieren?**

Nein. Interaktionszuordnung steht allen Benutzern in ihren Instanzen zur Verfügung. Sie können sie für bestimmte Benutzer, Arbeitsbereiche usw. nicht aktivieren/deaktivieren.

**Wie unterscheidet sich dies von anderen visuellen Buildern?**

Die Interaktionskarte zeichnet sich durch drei Schlüsselelemente aus:

* Flexibilität: Einfaches Verwalten und Validieren von verbundenen oder tief verschachtelten Kampagnen mit Visualisierung.

* Funktionalität: Alle Visualisierungen sind vorkonfiguriert, was die Verwendung erleichtert. Die verschachtelte Struktur ermöglicht es Ihnen, einzutauchen und das gesamte Bild zu erhalten.

* Leistung: Sie behalten die gesamte Raffinesse von Marketo Engage, jetzt in einem visuellen Format.

>[!MORELIKETHIS]
>
>* [Registerkarte Interaktionszuordnung](/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-tab.md){target="_blank"}
>* [Registerkarte „Einstellungen](/help/marketo/product-docs/core-marketo-concepts/engagement-map/settings-tab.md){target="_blank"}
