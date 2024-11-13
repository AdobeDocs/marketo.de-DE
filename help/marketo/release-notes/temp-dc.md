---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Versionshinweise zu Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 7fbfdc6d34d2f1174e921464d64689b0c5687914
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 3%

---

# TEMP Dynamic Chat - Versionshinweise {#dynamic-chat-release}

## Version September/Oktober 2024 {#august-release}

### Verbesserte Live-Chat-Analyse {#enhanced-live-chat-analytics}

Am Analytics-Dashboard wurden verschiedene Verbesserungen vorgenommen, darunter:

* Gesamtzahl der angeforderten Live-Chat-Anzahl: Anzahl der Besucher, die für einen &quot;Chat mit Agenten&quot;angefordert wurden

* Gesamter vernetzter Live-Chat: Anzahl der verbundenen Besucher im Vergleich zur Gesamtanzahl der angeforderten Besucher für einen &quot;Chat mit Agenten&quot;

* Gesamtzahl der fehlenden Live-Chat-Anfragen: Anzahl der Besucher, die unbeaufsichtigt sind, im Vergleich zur Gesamtanzahl der angeforderten Kontakte für einen &quot;Chat mit Agent&quot;

* Durchschnittliche Chat-Länge in Minuten: Analyse der &quot;durchschnittlichen Chat-Länge&quot;zwischen Besuchern und Ihren Agenten

* Durchschnittliche Agent-Reaktionszeit in Sekunden: Analysieren Sie die &quot;durchschnittliche Zeit, die von den Agenten benötigt wird, um auf ihre Live-Chat-Fragen und Antworten zu antworten.

* Tägliches Dashboard: erfolgreich verbundene Live-Chat-Anfragen, fehlende Live-Chat-Anfragen, Sortierung und Filterung der aktuellen Live-Chat-Aktivitäten

SCREENSHOT

### Unterhaltsscoring {#conversation-scoring}

Quantifizieren Sie Ihre Leads anhand der Qualität ihrer Chat-Interaktion und verwenden Sie diese Metrik als Trigger/Filter in Marketo Engage-Smart-Kampagnen. Verwenden Sie das neue Attribut _Konversationsbewertung_ für die folgenden Aktivitäten:

* Hat einen Dialog geführt
* Gesprächsfluss
* Interagiert mit einem Agenten

**Zu beachtende Dinge:**

* Der Punktwert liegt zwischen 0, 1, 2, 3 (der Standardwert ist null).

* Nachdem die Konversation abgeschlossen oder abgelegt wurde, speichern Sie in der Aktivität den Scoring-Wert und posten Sie, dass sie nicht bearbeitet werden kann???? (Was bedeutet dieser Satz?)

* Festlegen einer Punktzahl:

   * Im Posteingang des Agenten - während eines Live-Chat kann der Agent eine Punktzahl für die Konversation aktualisieren oder festlegen, die in der Konversationsaktivität gespeichert wird

   * Im Stream-Designer - auf der Zielkarte kann der Benutzer eine Konversationsbewertung aktualisieren oder festlegen

SCREENSHOT

SCREENSHOT

SCREENSHOT

### Neue Lead-Erstellungslogik {#new-lead-creation-logic}

Wenn ein Lead ein Formular mit der E-Mail &quot;`abc@test.com`&quot;ausfüllt und als xyz Cookies ist, dann später dasselbe Formular mit der E-Mail &quot;`def@test.com`&quot;ausfüllt, wird ein neuer Lead erstellt, aber Cookie xyz wird mit dem neuen Lead verknüpft und aus Lead `abc@test.com` entfernt.

Ab diesem Zeitpunkt ist `abc@test.com` ein Lead ohne Cookie. KANN MAN LEIDER GEHEN?

Wenn also ein Besucher mit Cookie abc auf eine Seite gelangt und eine E-Mail-ID als `abc@p.com` angibt:

TABELLE

### Optimierte Ladezeit des Konversationsflusses {#optimized-conversation-flow-load-time}

Um das Benutzererlebnis zu verbessern, wird jetzt anstelle eines Leerraums beim Laden des Konversationsflusses ein Shimmer-Ladeprogramm angezeigt. KONVERSATION ODER KONVERSATIONAL?

**before**

GIF

**Nach**

GIF

### Option zum Vererben der Schriftart {#option-to-inherit-font}

Sie können jetzt den Chat-Bot aktivieren, um die Schriftart direkt von der Webseite zu übernehmen, auf der sie gehostet wird, anstatt die Markenschriftart im Dynamic Chat zu verwalten. Wenn Sie diese Option aktivieren, nimmt der Chatbot die Schriftart an, die im Tag `<body>` der Seite definiert ist.

SCREENSHOT

### Demandbase-Integration mit Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Demandbase-Benutzer können ihre eigene Demandbase-Lizenz mitbringen und die Integration aktivieren. Verwenden Sie Demandbase-Personenattribute für Dialog-Targeting, bedingtes Branding und benutzerdefiniertes Routing.

Die Auflösung dieser Attributwerte gegenüber einem Lead erfolgt in Echtzeit und wird im entsprechenden Lead-Profil gespeichert.
