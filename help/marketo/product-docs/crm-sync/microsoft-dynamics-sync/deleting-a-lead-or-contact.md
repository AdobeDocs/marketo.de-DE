---
unique-page-id: 45417322
description: Löschen eines Interessenten oder Kontakts - Marketo Docs - Produktdokumentation
title: Löschen eines Interessenten oder Kontakts
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Löschen eines Interessenten oder Kontakts {#deleting-a-lead-or-contact}

Es gibt einige Dinge zu wissen, wenn es darum geht, Leads/Kontakte in Microsoft Dynamics zu löschen.

* Marketo löscht nicht automatisch Personen, nur weil Leads in Dynamics gelöscht wurden. Stattdessen ist das Flag &quot;Microsoft is Deleted&quot;auf &quot;true&quot;gesetzt. Sie können diesen Trigger bei Bedarf löschen, um den Datensatz in Marketo zu löschen.

* Aktion &quot;Person löschen&quot;: Dadurch wird nur eine Person in Marketo gelöscht (eine Option zum Löschen in Dynamics ist nicht verfügbar).

* Wenn ein Interessent in Marketo (aber nicht in Dynamics) gelöscht und danach in Dynamics aktualisiert wird, würde es eine neue Person in Marketo (gleiche E-Mail-Adresse, neue Personen-ID) erstellen.

* Wenn ein Interessent in Dynamics (aber nicht in Marketo) gelöscht wird und anschließend durch die Flusshandlung &quot;Synchronisierter Benutzer mit Microsoft&quot; läuft, würde dies einen neuen Vorsprung in Dynamics schaffen.
