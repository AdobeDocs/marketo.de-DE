---
unique-page-id: 10092977
description: Erfahren Sie mehr über den Qualifizierungsprozess des Dynamics-Synchronisierungsfilters beim Konvertieren eines Leads in einen Kontakt. Verstehen, wie sich die Werte von Lead- und Kontaktsynchronisierungsfiltern auf die Marketo-Synchronisierung auswirken.
title: Microsoft Dynamics-Synchronisierungsfilter - Qualifizieren
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
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
