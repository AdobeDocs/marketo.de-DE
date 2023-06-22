---
description: Registerkarte "Name"- Marketo Docs - Produktdokumentation
title: Registerkarte "Name"
hide: true
hidefromtoc: true
exl-id: f54b9258-451b-4607-b5a9-f8627c6f420a
source-git-commit: 983f47ded61198b015f92a770be1004a13547296
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# Registerkarte &quot;Name&quot; {#name-tab}

Journey werden durch eine Reihe von Trigger-, Filter- und Flusskarten dargestellt. Wenn Sie auf jede dieser Karten klicken, wird der entsprechende Slide-out-Bereich geöffnet.

Übersicht über Trigger: Auf der Karte wird die Anzahl der Trigger in der jeweiligen Kampagne angezeigt. Wenn Sie auf diese Karte klicken, werden auch die Detailkarten der Trigger angezeigt und gleichzeitig das Bedienfeld &quot;Slide out&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Trigger gehört

Schaltfläche &quot;Trigger bearbeiten&quot;, um auf die Registerkarte &quot;Smart-Liste&quot;zuzugreifen

Liste der Trigger-Namen

SCREENSHOT

Trigger-Detail: Auf der Karte wird der Name des Triggers angezeigt. Wenn Sie auf diese Karte klicken, wird das Bedienfeld &quot;Slide out&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Trigger gehört

Schaltfläche &quot;Trigger bearbeiten&quot;, um auf die Registerkarte &quot;Smart-Liste&quot;zuzugreifen

Liste der dem Trigger zugeordneten Begrenzungen

SCREENSHOT

Filter: Wenn Sie auf diese Karte klicken, wird das Bedienfeld &quot;Slide out&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Trigger gehört

Schaltfläche Filter bearbeiten für den Zugriff auf die Registerkarte &quot;Smart-Liste&quot;

Geschätzte Anzahl von Personen, die sich für den Filter qualifizieren

Liste der Filter und der jeweiligen Einschränkungen

SCREENSHOT

Flussschritte: Wenn ein Flussschritt keine Optionen enthält, zeigt die Karte Attribute an, die mit dem Flussschritt verknüpft sind. Wenn Sie auf die Karte klicken, wird das Bedienfeld &quot;Folie aus&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Schritt &quot;Fluss&quot;gehört

Schaltfläche &quot;Fluss bearbeiten&quot;zum Aufrufen der Registerkarte &quot;Fluss&quot;

Liste der mit dem Flussschritt verknüpften Attribute

SCREENSHOT

Flussschritte: Wenn ein Flussschritt Optionen enthält, zeigt die Karte den Namen des Flussschritts an. Wenn Sie auf die Karte klicken, wird das Bedienfeld &quot;Folie aus&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Schritt &quot;Fluss&quot;gehört

Schaltfläche &quot;Fluss bearbeiten&quot;zum Aufrufen der Registerkarte &quot;Fluss&quot;

Liste der Auswahlbedingungen, die dem Flussschritt zugeordnet sind

SCREENSHOT

Flussschritt für Ausführen und Anfordern von Kampagnen:

Wenn der Schritt Kampagnenfluss ausführen oder anfordern keine Optionen enthält, zeigt die Karte den Namen der Kampagne an. Wenn Sie auf die Karte klicken, wird das Bedienfeld &quot;Folie aus&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Flussschritt gehört

Schaltfläche &quot;Fluss bearbeiten&quot;zum Aufrufen der Registerkarte &quot;Fluss&quot;

Liste der mit dem Flussschritt verknüpften Attribute

Schaltfläche Liste anzeigen , mit der eine Liste von Kampagnen geöffnet wird, die die jeweilige Anforderung verwenden oder eine Kampagne ausführen

Hinweis: Sie können den Flussschritt von einer primären Kampagne aus bearbeiten. Um verschachtelte Kampagnen zu bearbeiten, müssen Sie über den Hyperlink im Bereich &quot;Folie aus&quot;zur Kampagne navigieren.

SCREENSHOT

SCREENSHOT

Wenn der Schritt Kampagnenfluss ausführen oder anfordern eine Auswahl enthält, zeigt die Karte den Namen der Kampagne an. Wenn Sie auf die Karte klicken, wird das Bedienfeld &quot;Folie aus&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der der Flussschritt gehört

Schaltfläche &quot;Fluss bearbeiten&quot;zum Aufrufen der Registerkarte &quot;Fluss&quot;

Liste der Auswahlbedingungen, die dem Flussschritt zugeordnet sind

SCREENSHOT

SCREENSHOT

Wenn eine Ausführungs- oder Anforderungskampagne Optionen enthält, wird durch Klicken auf die Flusskarte die Auswahl in einzelnen Karten angezeigt.

Wenn Sie auf die Auswahlkarte klicken, wird die mit der jeweiligen Auswahl verknüpfte Kampagne erweitert und gleichzeitig das Bedienfeld &quot;Folie aus&quot;mit den folgenden Informationen geöffnet:

Kampagne, zu der die Auswahl gehört

Schaltfläche &quot;Auswahl bearbeiten&quot;, um auf die Registerkarte &quot;Fluss&quot;zuzugreifen

Liste der Auswahlbedingungen, die dem Flussschritt zugeordnet sind

Schaltfläche Liste anzeigen , mit der eine Liste von Kampagnen geöffnet wird, die die jeweilige Anforderung verwenden oder eine Kampagne ausführen

SCREENSHOT

Visualisieren von verschachtelten Execute-Campaign (neuer Abschnitt)

Führen Sie Kampagnen aus, die nacheinander mit der übergeordneten Kampagne ausgeführt werden, d. h. Leads, die für eine ausführbare Kampagne infrage kommen, führen alle Flussschritte der Kampagne aus und kehren zur primären Kampagne zurück, um durch die Durchsatzschritte dieser Kampagne fortzufahren.

Im Folgenden finden Sie ein Beispiel einer intelligenten Kampagne &quot;Kampagne A&quot;, die einen Schritt zum Ausführen des Kampagnenflusses enthält. Sie können sich vorstellen, dass &quot;Kampagne A&quot;Ihre primäre Kampagne ist.

SCREENSHOT

Wenn Sie auf die Karte Kampagnenfluss ausführen klicken, werden Details zu &quot;Kampagne B&quot;angezeigt

Kampagne B enthält Filter, welche Verzweigungen in nicht qualifizierter und qualifizierter Zielgruppe ausscheiden.

Qualifizierte Zielgruppe durchläuft die mit &quot;Kampagne B&quot;verknüpften Flussschritte.

Alle Zielgruppen (qualifiziert und nicht qualifiziert) kehren zu &quot;Kampagne A&quot;zurück und fahren mit dem nächsten Flussschritt fort

SCREENSHOT

Sie können in &quot;Kampagne B&quot;auf Kampagnenfluss ausführen klicken. Daraufhin werden Auswahlkarten und Kampagnen angezeigt, die mit jeder Auswahl verknüpft sind.

SCREENSHOT

Visualisieren der Anforderungskampagne (neuer Abschnitt)

Anfragekampagnen werden parallel zur übergeordneten Kampagne ausgeführt, d. h. Leads, die für eine Anfragekampagne qualifiziert sind, führen alle Durchsatzschritte aus der Kampagne aus und beenden die Kampagne. Parallel dazu durchlaufen dieselben Leads auch die Flussschritte der primären Kampagne.

Im Folgenden finden Sie ein Beispiel einer intelligenten Kampagne &quot;Kampagne A&quot;, die einen Schritt zum Anforderungskampagnenfluss enthält. Sie können sich vorstellen, dass &quot;Kampagne A&quot;Ihre primäre Kampagne ist.

SCREENSHOT

Wenn Sie auf die Karte für den Ablauf der Anforderungskampagne klicken, werden Details von &quot;Kampagne B&quot;angezeigt

Kampagne B enthält Filter, welche Verzweigungen in die qualifizierte Zielgruppe eingehen.

Qualifizierte Zielgruppe durchläuft die mit &quot;Kampagne B&quot;verknüpften Flussschritte.

Parallel dazu wechseln alle Zielgruppen zu den nächsten Flussschritten in &quot;Kampagne A&quot;.

SCREENSHOT

Sie können tiefer in verschachtelte Kampagnen eintauchen, wenn einer der Flussschritte eine weitere Anfragekampagne enthält, indem Sie auf die Flusskarte klicken, um Details zur Kampagne anzuzeigen.

SCREENSHOT

Hier ist ein Beispiel für eine Anforderungskampagne mit Auswahlmöglichkeiten.

SCREENSHOT

Umgang mit Fehlern:

Fehler in den Schritten &quot;Smart-Liste&quot;und &quot;Fluss&quot;werden über das Fehlersymbol auf der Karte hervorgehoben. Darüber hinaus wird die entsprechende Fehlermeldung im Bedienfeld &quot;Folie ausblenden&quot;angezeigt.

Im Folgenden finden Sie ein Beispiel für einen Fehler in Trigger, der auf der Übersichtskarte Trigger, im Bedienfeld &quot;Folie&quot;sowie auf der Trigger-Detailkarte angezeigt wird.

SCREENSHOT

SCREENSHOT

Fehler in Filterkarte kann enthalten

Fehler in der Smart-Liste, der dazu führt, dass keine qualifizierte Zielgruppe angezeigt wird

Fehler in Filterlogik

Fehler bei Beschränkungen oder Fehlen von Beschränkungen in einem oder mehreren Filtern

SCREENSHOT

Wenn Sie keine Werte (Attribute) eingeben, werden sie nicht als Fehler gekennzeichnet. Sie funktionieren weiterhin wie auf der Registerkarte &quot;Fluss&quot;. Daher werden bestehende Kampagnen nicht gestört. Wenn jedoch Flussschritte keine Attribute enthalten, werden diese als Warnungen angezeigt.

SCREENSHOT

Hinweis: Fehler innerhalb einer verschachtelten Kampagne sind erst sichtbar, wenn Sie zum Erweitern der verschachtelten Kampagne auf klicken
