---
description: Übersicht über das E-Mail-Tracking - Marketo-Dokumente - Produktdokumentation
title: Übersicht über das E-Mail-Tracking
hide: true
hidefromtoc: true
source-git-commit: 8789ed464f532bbe76c2cb456374d9c0f505ece0
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Übersicht über das E-Mail-Tracking {#email-tracking-overview}

## Funktionsweise des Antworten-Trackings {#how-reply-tracking-works}

Das Tracking der Antworten erfolgt durch Überprüfen einer Nachrichten-ID, die in jeder gesendeten E-Mail enthalten ist. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir die beste Antwort-Tracking-Funktion nutzen können.

>[!PREREQUISITES]
>
>Verbindung mit E-Mail-Server: Sales Connect muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eintrifft. Sie müssen Ihr Sales Connect-Konto mit Gmail verbinden. Wenn Sie Outlook verwenden, müssen wir in Ihren Exchange-Server integrieren.

Wenn Sales Connect die Antwort Ihres potenziellen Kunden auf Ihre E-Mail nicht verfolgen kann, kann eine Kampagne nicht aufgrund der Antworterkennung angehalten oder die Antwort an Salesforce protokolliert werden. Was bedeutet, dass jede E-Mail-Adresse antworten kann?

Wenn Sie also flynn@flynnsarcade.com per E-Mail senden und er mit kevinf@flynnsarcade.com antwortet, können wir die Antwort verfolgen. Wenn Sie außerdem eine E-Mail an flynn@flynnsarcade.com und CC alan@encom.com senden und Alan Sie zurückschreibt, wird auch die Antwort erkannt und die Kampagne beendet.

## Funktionsweise des Antworten-Trackings {#how-reply-tracking-works}

Text

## Verfolgen Ihrer E-Mail-Anhänge {#how-to-track-your-email-attachments}

