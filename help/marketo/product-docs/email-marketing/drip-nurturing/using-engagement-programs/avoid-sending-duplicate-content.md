---
unique-page-id: 10096409
description: Versenden doppelter Inhalte vermeiden - Marketo-Dokumente - Produktdokumentation
title: Senden doppelter Inhalte vermeiden
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Zauber innerhalb des ZEE-Programms **derselbe** ausgelöst wird | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Zauber innerhalb des ZEE-Programms **derselbe** ausgelöst wird | Kein Mitglied des Standardprogramms | Ja |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Zauber innerhalb eines **anderen** CEE-Programms ausgelöst wird | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die durch einen Zauber innerhalb eines **anderen** CEE-Programms ausgelöst wird | Kein Mitglied des Standardprogramms | Ja |
| Ein **anderes** CEE-Programm mit einem Smart-Stream | Mitglied beider CEE-Programme | Nein |
