---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter - Qualify - Marketo Docs - Produktdokumentation
title: Synchronisierungsfilter für Microsoft Dynamics - Qualify
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics Sync-Filter: Qualifizieren {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Lead in Microsoft Dynamics in einen Kontakt konvertieren möchten, stellen Sie sicher, dass Sie diesen standardmäßigen Qualifizierungsprozess verwenden. Synchronisieren Sie sie dann mit Marketo.

## Der Konvertierungsprozess {#the-conversion-process}

So funktionieren die Filter während des Konvertierungsprozesses.

| Wenn der Lead-Synchronisierungsfilter: | und der Filter für die Kontaktsynchronisierung lautet: | Dies führt zu Marketo |
|---|---|---|
| False | False | In Marketo wird nichts synchronisiert |
| True | True | Der Kontakt wird in Marketo synchronisiert. |
| False | True | Neuer Kontaktdatensatz wird in Marketo erstellt |
| True | False | MS Dynamics aktualisiert Lead-Informationen in Marketo, aber Kontaktdatensätze werden nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vordefinierten Konvertierungsprozess Qualifizieren .
