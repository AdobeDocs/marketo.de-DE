---
unique-page-id: 10096409
description: Versenden doppelter Inhalte vermeiden - Marketo-Dokumente - Produktdokumentation
title: Senden doppelter Inhalte vermeiden
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
source-git-commit: daaf3dc9b4da95db743409c6e2a6c426ed00e9c7
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 3%

---

# Senden doppelter Inhalte vermeiden {#avoid-sending-duplicate-content}

Hast du schon einmal zweimal dieselbe E-Mail erhalten? Wahnsinn, nicht wahr?

Im Folgenden finden Sie sieben mögliche Szenarien und Ergebnisse, die Sie kennen sollten, um zu verhindern, dass dieselbe Nachricht mit Interaktionsprogrammen zweimal gesendet wird.

## Szenarien {#scenarios}

| Die E-Mail wird gesendet von | Die Person ist | Person erhält E-Mail |
|---|---|---|
| Eine Kampagne in einem separaten, eigenständigen Standardprogramm | Kein Mitglied des Standardprogramms | Ja |
| Eine Kampagne in einem separaten, eigenständigen Standardprogramm | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Abruf innerhalb der **same** CEE-Programm | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Abruf innerhalb der **same** CEE-Programm | Kein Mitglied des Standardprogramms | Ja |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Abruf innerhalb einer **distinct** CEE-Programm | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Abruf innerhalb einer **distinct** CEE-Programm | Kein Mitglied des Standardprogramms | Ja |
| A **distinct** CEE-Programm mit intelligentem Stream | Mitglied beider CEE-Programme | Nein |
