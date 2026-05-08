---
unique-page-id: 10092977
description: Erfahren Sie mehr über den Qualifizierungsprozess des Dynamics-Synchronisierungsfilters beim Konvertieren eines Leads in einen Kontakt. Verstehen, wie sich die Werte von Lead- und Kontaktsynchronisierungsfiltern auf die Marketo-Synchronisierung auswirken.
title: Microsoft Dynamics-Synchronisierungsfilter - Qualifizieren
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]-Synchronisierungsfilter: Qualifizieren {#microsoft-dynamics-sync-filter-qualify}

Wenn Sie einen Lead in einen Kontakt in [!DNL Microsoft Dynamics] konvertieren möchten, verwenden Sie diesen standardmäßigen Qualifizierungsprozess. Synchronisieren Sie sie dann mit Marketo.

## Der Konvertierungsprozess {#the-conversion-process}

| Wenn der Lead-Synchronisierungsfilter ist: | Der Filter für die Kontaktsynchronisierung lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| [!UICONTROL false] | [!UICONTROL false] | In Marketo wird nichts synchronisiert |
| [!UICONTROL true] | [!UICONTROL true] | Der Kontakt wird in Marketo synchronisiert |
| [!UICONTROL false] | [!UICONTROL true] | Neuer Kontakteintrag wird in Marketo erstellt |
| [!UICONTROL true] | [!UICONTROL false] | [!DNL MS Dynamics] aktualisiert Lead-Informationen in Marketo, der Kontaktdatensatz wird jedoch nicht synchronisiert |

>[!CAUTION]
>
>Wir unterstützen nur den vorkonfigurierten Konvertierungsprozess von Qualifikationen.
