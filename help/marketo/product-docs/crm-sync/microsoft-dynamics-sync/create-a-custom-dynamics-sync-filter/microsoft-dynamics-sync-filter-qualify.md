---
unique-page-id: 10092977
description: Microsoft Dynamics-Synchronisierungsfilter - Qualifizieren - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierungsfilter - Qualifizieren
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]-Synchronisierungsfilter: Qualifizieren {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Lead in einen Kontakt in [!DNL Microsoft Dynamics] konvertieren möchten, verwenden Sie unbedingt diesen standardmäßigen Qualifizierungsprozess. Synchronisieren Sie sie dann mit Marketo.

## Der Konvertierungsprozess {#the-conversion-process}

So funktionieren die Filter während des Konvertierungsprozesses.

| Wenn der Lead-Synchronisierungsfilter ist: | Der Filter für die Kontaktsynchronisierung lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| [!UICONTROL false] | [!UICONTROL false] | In Marketo wird nichts synchronisiert |
| [!UICONTROL true] | [!UICONTROL true] | Der Kontakt wird in Marketo synchronisiert |
| [!UICONTROL false] | [!UICONTROL true] | Neuer Kontakteintrag wird in Marketo erstellt |
| [!UICONTROL true] | [!UICONTROL false] | [!DNL MS Dynamics] aktualisiert Lead-Informationen in Marketo, der Kontaktdatensatz wird jedoch nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vorkonfigurierten Konvertierungsprozess von Qualifikationen.
