---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter - Qualify - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync Filter - Qualifizieren
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Microsoft Dynamics Sync-Filter: Qualifizieren Sie {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Interessenten in Microsoft Dynamics in einen Kontakt konvertieren möchten, sollten Sie diesen Standardqualifizierungsprozess verwenden. Synchronisieren Sie es dann mit Marketo.

## Der Konvertierungsprozess {#the-conversion-process}

So funktionieren die Filter während des Konvertierungsprozesses.

| Wenn der Interessentensynchronisierungsfilter: | und der Filter für die Kontaktsynchronisierung lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| False | False | Nichts wird in Marketo synchronisiert |
| true | true | Der Kontakt wird in Marketo synchronisiert |
| False | true | Neuer Kontaktdatensatz wird in Marketo erstellt |
| true | False | MS Dynamics aktualisiert Interessenteninformationen in Marketo, aber Kontaktdatensätze werden nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vordefinierten Konvertierungsprozess Qualifizieren.
