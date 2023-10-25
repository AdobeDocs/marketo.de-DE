---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter - Qualify - Marketo Docs - Produktdokumentation
title: Synchronisierungsfilter für Microsoft Dynamics - Qualify
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 6%

---

# Synchronisierungsfilter für Microsoft Dynamics: Qualifizieren {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Lead in Microsoft Dynamics in einen Kontakt konvertieren möchten, stellen Sie sicher, dass Sie diesen standardmäßigen Qualifizierungsprozess verwenden. Synchronisieren Sie sie dann mit Marketo Engage.

## Der Konvertierungsprozess {#the-conversion-process}

So funktionieren die Filter während des Konvertierungsprozesses.

| Wenn der Lead-Synchronisierungsfilter: | und der Filter für die Kontaktsynchronisierung lautet: | Dies führt zu Marketo |
|---|---|---|
| Falsch | Falsch | In Marketo wird nichts synchronisiert. |
| True | True | Der Kontakt wird in Marketo synchronisiert. |
| Falsch | True | Neuer Kontaktdatensatz wird in Marketo erstellt |
| True | Falsch | MS Dynamics aktualisiert Lead-Informationen in Marketo, aber Kontaktdatensätze werden nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vordefinierten Konvertierungsprozess Qualifizieren .
