---
unique-page-id: 10092977
description: Microsoft Dynamics-Synchronisierungsfilter - Qualifizieren - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierungsfilter - Qualifizieren
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 6%

---

# Microsoft Dynamics-Synchronisierungsfilter: Qualifizieren {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Lead in einen Kontakt in Microsoft Dynamics konvertieren möchten, verwenden Sie unbedingt diesen standardmäßigen Qualifizierungsprozess. Synchronisieren Sie sie dann mit Marketo Engage.

## Der Konvertierungsprozess {#the-conversion-process}

So funktionieren die Filter während des Konvertierungsprozesses.

| Wenn der Lead-Synchronisierungsfilter ist: | Der Filter für die Kontaktsynchronisierung lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| Falsch | Falsch | In Marketo wird nichts synchronisiert |
| True | True | Der Kontakt wird in Marketo synchronisiert |
| Falsch | True | Neuer Kontakteintrag wird in Marketo erstellt |
| True | Falsch | MS Dynamics aktualisiert die Lead-Informationen in Marketo, der Kontaktdatensatz wird jedoch nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vorkonfigurierten Konvertierungsprozess von Qualifikationen.
