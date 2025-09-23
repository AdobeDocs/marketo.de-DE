---
unique-page-id: 45417322
description: Löschen von Leads oder Kontakten - Marketo-Dokumente - Produktdokumentation
title: Löschen eines Leads oder Kontakts
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 6%

---

# Löschen eines Leads oder Kontakts {#deleting-a-lead-or-contact}

Es gibt einige Dinge zu wissen, wenn es um das Löschen von Leads/Kontakten in [!DNL Microsoft Dynamics] geht.

* Marketo löscht Personen nicht automatisch, nur weil Leads in [!DNL Dynamics] gelöscht wurden. Stattdessen wird ein Feld-Flag &quot;Microsoft wird gelöscht“ auf „true“ gesetzt. Sie können bei Bedarf einen Trigger aus diesem Feld machen, um den Datensatz in Marketo zu löschen.

* Flussaktion „Person löschen“: Dadurch wird nur eine Person in Marketo gelöscht (eine Option, sie auch in Dynamics zu löschen, ist nicht verfügbar).

* Wenn ein Lead in Marketo gelöscht wird (aber nicht in [!DNL Dynamics]) und anschließend in [!DNL Dynamics] aktualisiert wird, wird in Marketo eine neue Person erstellt (gleiche E-Mail-Adresse, neue Personen-ID).

* Wenn ein Lead in [!DNL Dynamics] (aber nicht in Marketo) gelöscht wird und anschließend die Flussaktion „Person mit Microsoft synchronisieren“ durchläuft, wird in [!DNL Dynamics] ein neuer Lead erstellt.
