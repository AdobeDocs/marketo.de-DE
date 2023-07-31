---
description: Registerkarte "Interaktionszuordnung"- Marketo-Dokumente - Produktdokumentation
title: Registerkarte "Interaktionskarte"
hide: true
hidefromtoc: true
exl-id: f54b9258-451b-4607-b5a9-f8627c6f420a
source-git-commit: 3c7eb2fc2e64898e12f08743225c0b802bf97474
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Registerkarte &quot;Interaktionskarte&quot; {#engagement-map-tab}

Interaktionszuordnung wird durch eine Reihe von Trigger-, Filter- und Flusskarten dargestellt. Wenn Sie auf jede Karte klicken, werden zusätzliche Informationen angezeigt.

Übersicht über Trigger: Auf dieser Karte wird die Anzahl der Trigger in Ihrer Kampagne angezeigt. Wenn Sie darauf klicken, werden eine Karte für jeden Trigger sowie ein Slide-out-Bedienfeld mit den folgenden Informationen angezeigt:

* Kampagne, zu der der Trigger gehört
* Liste der Trigger-Namen
* Schaltfläche &quot;Trigger bearbeiten&quot;

  ![](assets/engagement-map-tab-1.png)

Trigger Detail: Auf dieser Karte wird der Name des Triggers angezeigt. Wenn Sie darauf klicken, wird ein Slide-out-Bedienfeld mit den folgenden Informationen angezeigt:

* Kampagne, zu der der Trigger gehört
* Liste der dem Trigger zugeordneten Begrenzungen
* Schaltfläche &quot;Trigger bearbeiten&quot;

  ![](assets/engagement-map-tab-2.png)

Filter: Wenn Sie auf diese Karte klicken, wird ein Slide-out-Bedienfeld mit den folgenden Informationen angezeigt:

* Kampagne, zu der der Trigger gehört
* Geschätzte Anzahl von Personen, die sich für den Filter qualifizieren
* Liste der Filter und der jeweiligen Einschränkungen
* Schaltfläche &quot;Filter bearbeiten&quot;

  ![](assets/engagement-map-tab-3.png)

Flussschritte: Wenn ein Flussschritt Optionen enthält, zeigt diese Karte den Namen des Flussschritts an. Wenn Sie darauf klicken, wird ein Slide-out-Bedienfeld mit den folgenden Informationen angezeigt:

* Campaign Der Fluss -Schritt gehört zu
* Liste der Auswahlbedingungen, die mit dem Flussschritt verknüpft sind
* Schaltfläche &quot;Fluss bearbeiten&quot;

  ![](assets/engagement-map-tab-4.png)

Flussschritte: Wenn ein Flussschritt _not_ alle Optionen einschließen, zeigt diese Karte Attribute an, die mit dem Flussschritt verknüpft sind. Wenn Sie darauf klicken, wird ein Slide-out-Bedienfeld mit den folgenden Informationen angezeigt:

* Campaign Der Fluss -Schritt gehört zu
* Liste der dem Flussschritt zugeordneten Attribute
* Schaltfläche &quot;Fluss bearbeiten&quot;

  ![](assets/engagement-map-tab-5.png)

## Flussschritt für Ausführen und Anfordern von Kampagnen {#flow-step-for-execute-and-request-campaigns}

* Wenn der Schritt Kampagnenfluss ausführen oder anfordern keine Optionen enthält, zeigt die Karte den Namen der Kampagne an. Wenn Sie auf die Karte klicken, wird ein Bedienfeld mit der folgenden Information angezeigt:

   * Kampagne, zu der der Flussschritt gehört
   * Schaltfläche &quot;Fluss bearbeiten&quot;
   * Liste der dem Flussschritt zugeordneten Attribute
   * Schaltfläche &quot;Liste anzeigen&quot;, über die eine Liste von Kampagnen geöffnet wird, die die jeweilige Kampagne &quot;Anfrage/Ausführung&quot; verwenden

>[!NOTE]
>
>Sie können die Flussschritte von einer primären Kampagne aus bearbeiten. Um verschachtelte Kampagnen zu bearbeiten, müssen Sie über den Link im Dia-out-Bedienfeld zur Kampagne navigieren.

![](assets/engagement-map-tab-6.png)

![](assets/engagement-map-tab-7.png)

* Wenn der Schritt Kampagnenfluss ausführen oder anfordern eine Auswahl enthält, zeigt die Karte den Namen der Kampagne an. Wenn Sie auf die Karte klicken, wird ein Bedienfeld mit der folgenden Information angezeigt:

   * Kampagne, zu der der Flussschritt gehört
   * Liste der Auswahlbedingungen, die mit dem Flussschritt verknüpft sind
   * Schaltfläche &quot;Fluss bearbeiten&quot;

  ![](assets/engagement-map-tab-8.png)

  ![](assets/engagement-map-tab-9.png)

* Wenn eine Ausführen- oder Anforderungskampagne Optionen enthält, wird das Klicken auf die Flusskarte erweitert, um alle Optionen in einzelnen Karten anzuzeigen. Wenn Sie auf die Auswahlkarte klicken, wird die mit der jeweiligen Auswahl verknüpfte Kampagne erweitert und ein Slide-out-Bedienfeld mit den folgenden Informationen angezeigt:

   * Kampagne, zu der die Auswahl gehört
   * Schaltfläche &quot;Auswahl bearbeiten&quot;
   * Liste der Auswahlbedingungen, die mit dem Flussschritt verknüpft sind
   * Schaltfläche &quot;Liste anzeigen&quot;, über die eine Liste von Kampagnen geöffnet wird, die die jeweilige Kampagne &quot;Anfrage/Ausführung&quot; verwenden

  ![](assets/engagement-map-tab-10.png)

## Visualisieren einer verschachtelten Execute-Kampagne {#visualizing-a-nested-execute-campaign}

Führen Sie Kampagnen mit der übergeordneten Kampagne nacheinander aus. Personen, die sich für eine ausführbare Kampagne qualifizieren, führen alle Flussschritte aus der Kampagne aus und kehren zur primären Kampagne zurück, um die Durchsatzschritte dieser Kampagne zu verfolgen.

Nachstehend finden Sie ein Beispiel für eine Smart-Kampagne, &quot;Kampagne A&quot;, die einen Workflow-Schritt zum Ausführen einer Kampagne enthält. Stellen Sie sich &quot;Kampagne A&quot;als Ihre primäre Kampagne vor.

![](assets/engagement-map-tab-11.png)

1. Wenn Sie auf die Karte Kampagnenfluss ausführen klicken, werden Details zu &quot;Kampagne B&quot;angezeigt.
1. &quot;Kampagne B&quot;enthält einen Filter, der die Zielgruppe in zwei Gruppen unterteilt: qualifiziert und nicht qualifiziert.
1. Die qualifizierte Zielgruppe durchläuft die mit &quot;Kampagne B&quot;verknüpften Flussschritte.
1. Alle Zielgruppen (qualifiziert und nicht qualifiziert) kehren zu &quot;Kampagne A&quot;zurück und fahren mit dem nächsten Flussschritt fort.

   ![](assets/engagement-map-tab-12.png)

Sie können in &quot;Kampagne B&quot;auf den Schritt Kampagnenfluss ausführen klicken. Daraufhin werden die Auswahlkarten und die mit jeder Auswahl verknüpfte Kampagne angezeigt.

![](assets/engagement-map-tab-13.png)

## Visualisieren von Anforderungskampagnen {#visualizing-request-campaign}

Anfragekampagnen werden parallel zur übergeordneten Kampagne ausgeführt. Personen, die sich für eine Anfragekampagne qualifizieren, führen alle Flussschritte der Kampagne aus und beenden dann die Kampagne. Gleichzeitig durchlaufen dieselben Personen die Durchsatzschritte der primären Kampagne.

Im Folgenden finden Sie ein Beispiel für eine Smart-Kampagne, &quot;Kampagne A&quot;, die einen Schritt zum Anforderungskampagnenfluss enthält. Stellen Sie sich &quot;Kampagne A&quot;als Ihre primäre Kampagne vor.

![](assets/engagement-map-tab-14.png)

1. Wenn Sie auf die Flusskarte der Anfragekampagne klicken, werden die Details von &quot;Kampagne B&quot;angezeigt.
1. &quot;Kampagne B&quot;enthält einen Filter, der die Zielgruppe in zwei Gruppen unterteilt: qualifiziert und nicht qualifiziert.
1. Die qualifizierte Zielgruppe durchläuft die mit &quot;Kampagne B&quot;verknüpften Flussschritte.
1. Gleichzeitig wechseln alle Zielgruppen zu den nächsten Flussprogrammen in &quot;Kampagne A&quot;.

   ![](assets/engagement-map-tab-15.png)

Sie können Ihre verschachtelten Kampagnen genauer untersuchen, wenn einer der Durchsatzschritte eine andere Anfragekampagne enthält, indem Sie auf die Flusskarte klicken, um die Details der Kampagne anzuzeigen.

![](assets/engagement-map-tab-16.png)

Im Folgenden finden Sie ein Beispiel für eine Anforderungskampagne mit Auswahlmöglichkeiten.

![](assets/engagement-map-tab-17.png)

## Umgang mit Fehlern {#error-handling}

Fehler in Smart-Listen und Fluss-Schritten werden über ein Fehlersymbol auf der Karte hervorgehoben. Darüber hinaus wird eine entsprechende Fehlermeldung im Dia-out-Bedienfeld angezeigt.

Unten finden Sie ein Beispiel für einen Fehler in einem Trigger, der auf der Übersichtskarte &quot;Trigger&quot;, im Slide-out-Bedienfeld und auf der Detailkarte des Triggers angezeigt wird.

![](assets/engagement-map-tab-18.png)

![](assets/engagement-map-tab-19.png)

**Fehler in Filterkarten können Folgendes enthalten:**

* Fehler in der Smart-Liste, der dazu führt, dass die qualifizierte Zielgruppe nicht angezeigt wird

* Fehler in der Filterlogik

* Fehler bei Begrenzungen (oder fehlende Beschränkungen) in einem oder mehreren Filtern

  ![](assets/engagement-map-tab-20.png)

>[!NOTE]
>
>Fehler innerhalb einer verschachtelten Kampagne werden erst sichtbar, wenn Sie zum Erweitern der verschachtelten Kampagne auf klicken.
