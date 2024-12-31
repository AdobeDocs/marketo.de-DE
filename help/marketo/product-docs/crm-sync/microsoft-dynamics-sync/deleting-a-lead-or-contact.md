---
unique-page-id: 45417322
description: Löschen von Leads oder Kontakten - Marketo-Dokumente - Produktdokumentation
title: Lead oder Kontakt löschen
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Lead oder Kontakt löschen {#deleting-a-lead-or-contact}

Es gibt einige Dinge zu wissen, wenn es um das Löschen von Leads/Kontakten in Microsoft Dynamics geht.

* Marketo Engage löscht Personen nicht automatisch, nur weil Leads in Dynamics gelöscht wurden. Stattdessen wird ein Feld-Flag &quot;Microsoft wird gelöscht“ auf „true“ gesetzt. Sie können bei Bedarf einen Trigger aus diesem Feld machen, um den Datensatz in Marketo zu löschen.

* Flussaktion „Person löschen“: Dadurch wird nur eine Person in Marketo gelöscht (eine Option, sie auch in Dynamics zu löschen, ist nicht verfügbar).

* Wenn ein Lead in Marketo (aber nicht in Dynamics) gelöscht und danach in Dynamics aktualisiert wird, wird eine neue Person in Marketo erstellt (gleiche E-Mail-Adresse, neue Personen-ID).

* Wenn ein Lead in Dynamics gelöscht wird (aber nicht in Marketo) und anschließend die Flussaktion „Person mit Microsoft synchronisieren“ durchläuft, wird ein neuer Lead in Dynamics erstellt.
