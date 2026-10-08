---
unique-page-id: 45417322
description: Erfahren Sie, wie das Löschen von Leads und Kontakten zwischen Microsoft Dynamics und Marketo funktioniert. Verwenden Sie das Flag "Microsoft wird gelöscht“ und die Flussaktion „Person löschen“ nach Bedarf.
title: Löschen eines Leads oder Kontakts
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/4BwBuLQFJ2pRehuS8EqW-UrEcg5sVeqcstu3azh0NvQ'
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
source-wordcount: '167'
ht-degree: 5%
---
# Löschen eines Leads oder Kontakts {#deleting-a-lead-or-contact}

Es gibt einige Dinge zu wissen, wenn es um das Löschen von Leads/Kontakten in [!DNL Microsoft Dynamics] geht.

* Marketo löscht Personen nicht automatisch, nur weil Leads in [!DNL Dynamics] gelöscht wurden. Stattdessen wird ein Feld-Flag &quot;Microsoft wird gelöscht“ auf „true“ gesetzt. Sie können bei Bedarf einen Trigger aus diesem Feld machen, um den Datensatz in Marketo zu löschen.

* Flussaktion „Person löschen“: Dadurch wird nur eine Person in Marketo gelöscht (eine Option, sie auch in Dynamics zu löschen, ist nicht verfügbar).

* Wenn ein Lead in Marketo gelöscht wird (aber nicht in [!DNL Dynamics]) und anschließend in [!DNL Dynamics] aktualisiert wird, wird in Marketo eine neue Person erstellt (gleiche E-Mail-Adresse, neue Personen-ID).

* Wenn ein Lead in [!DNL Dynamics] (aber nicht in Marketo) gelöscht wird und anschließend die Flussaktion „Person mit Microsoft synchronisieren“ durchläuft, wird in [!DNL Dynamics] ein neuer Lead erstellt.
