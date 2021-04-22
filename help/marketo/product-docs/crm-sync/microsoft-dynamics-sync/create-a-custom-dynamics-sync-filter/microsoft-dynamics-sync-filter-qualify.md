---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter - Qualify - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync Filter - Qualifizieren
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics Sync-Filter: Qualifizieren Sie {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Interessenten in Microsoft Dynamics in einen Kontakt konvertieren möchten, sollten Sie diesen Standardqualifizierungsprozess verwenden. Synchronisieren Sie es dann mit Marketo.

## Der Konvertierungsprozess {#the-conversion-process}

So funktionieren die Filter während des Konvertierungsprozesses.

| Wenn der Interessentensynchronisierungsfilter: | und der Filter für die Kontaktsynchronisierung lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| Falsch | Falsch | Nichts wird in Marketo synchronisiert |
| Wahr | Wahr | Der Kontakt wird in Marketo synchronisiert |
| Falsch | Wahr | Neuer Kontaktdatensatz wird in Marketo erstellt |
| Wahr | Falsch | MS Dynamics aktualisiert Interessenteninformationen in Marketo, aber Kontaktdatensätze werden nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vordefinierten Konvertierungsprozess Qualifizieren.
