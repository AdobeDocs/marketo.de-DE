---
unique-page-id: 10096409
description: Erfahren Sie mehr über Szenarien, die doppelte E-Mails in Interaktionsprogrammen verhindern oder zulassen. Verwenden Sie Programmmitgliedschaft und CEE-Regeln, um Wiederholungen zu vermeiden.
title: Vermeiden des Versands von doppelten Inhalten
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
TQID: 'https://experienceleague.adobe.com/vJ0HguG6ad182v-Jkf-0DF6zAosaJG5B-me3ghxnYIM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: fc5011cf-5b46-40b1-a5de-d7f042f85633
    internal-label: Engagement programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 7%
---
# Vermeiden des Versands von doppelten Inhalten {#avoid-sending-duplicate-content}

Im Folgenden finden Sie sieben mögliche Szenarien und Ergebnisse, die zu beachten sind, um zu verhindern, dass jemand dieselbe Nachricht zweimal mit Interaktionsprogrammen sendet.

## Szenarios {#scenarios}

| Die E-Mail wird gesendet von | Die Person ist | Person erhält E-Mail |
|---|---|---|
| Eine Kampagne in einem separaten, eigenständigen Standardprogramm | Nicht Mitglied des Standardprogramms | Ja |
| Eine Kampagne in einem separaten, eigenständigen Standardprogramm | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die von einer Besetzung innerhalb des **gleichen** CEE-Programms ausgelöst wird | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die von einer Besetzung innerhalb des **gleichen** CEE-Programms ausgelöst wird | Nicht Mitglied des Standardprogramms | Ja |
| Eine Kampagne innerhalb eines Standardprogramms, die von einer Besetzung innerhalb eines **anderen** CEE-Programms ausgelöst wird | Ein Mitglied des Standardprogramms | Nein |
| Eine Kampagne innerhalb eines Standardprogramms, die von einer Besetzung innerhalb eines **anderen** CEE-Programms ausgelöst wird | Nicht Mitglied des Standardprogramms | Ja |
| Ein **anderes** CEE-Programm unter Verwendung eines Smart-Streams | Mitglied beider MOE-Programme | Nein |
