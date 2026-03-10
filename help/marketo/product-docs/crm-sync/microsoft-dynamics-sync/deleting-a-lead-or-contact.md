---
unique-page-id: 45417322
description: Erfahren Sie, wie das Löschen von Leads und Kontakten zwischen Microsoft Dynamics und Marketo funktioniert. Verwenden Sie das Flag "Microsoft wird gelöscht“ und die Flussaktion „Person löschen“ nach Bedarf.
title: Löschen eines Leads oder Kontakts
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 6%

---

# Löschen eines Leads oder Kontakts {#deleting-a-lead-or-contact}

Es gibt einige Dinge zu wissen, wenn es um das Löschen von Leads/Kontakten in [!DNL Microsoft Dynamics] geht.

* Marketo löscht Personen nicht automatisch, nur weil Leads in [!DNL Dynamics] gelöscht wurden. Stattdessen wird ein Feld-Flag &quot;Microsoft wird gelöscht“ auf „true“ gesetzt. Sie können bei Bedarf einen Trigger aus diesem Feld machen, um den Datensatz in Marketo zu löschen.

* Flussaktion „Person löschen“: Dadurch wird nur eine Person in Marketo gelöscht (eine Option, sie auch in Dynamics zu löschen, ist nicht verfügbar).

* Wenn ein Lead in Marketo gelöscht wird (aber nicht in [!DNL Dynamics]) und anschließend in [!DNL Dynamics] aktualisiert wird, wird in Marketo eine neue Person erstellt (gleiche E-Mail-Adresse, neue Personen-ID).

* Wenn ein Lead in [!DNL Dynamics] (aber nicht in Marketo) gelöscht wird und anschließend die Flussaktion „Person mit Microsoft synchronisieren“ durchläuft, wird in [!DNL Dynamics] ein neuer Lead erstellt.
