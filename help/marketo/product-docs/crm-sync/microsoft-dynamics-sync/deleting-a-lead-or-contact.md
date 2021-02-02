---
unique-page-id: 45417322
description: Löschen eines Interessenten oder Kontakts - Marketing Docs - Produktdokumentation
title: Löschen eines Interessenten oder Kontakts
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Löschen eines Interessenten oder Kontakts {#deleting-a-lead-or-contact}

Es gibt einige Dinge zu wissen, wenn es darum geht, Leads/Kontakte in Microsoft Dynamics zu löschen.

* Marketo löscht nicht automatisch Personen, nur weil Leads in Dynamics gelöscht wurden. Stattdessen ist das Flag &quot;Microsoft is Deleted&quot;auf &quot;true&quot;gesetzt. Sie können diesen Trigger bei Bedarf löschen, um den Datensatz in Marketo zu löschen.

* Aktion &quot;Person löschen&quot;: Dadurch wird nur eine Person in Marketo gelöscht (eine Option, sie auch in Dynamics zu löschen ist nicht verfügbar).

* Wenn ein Interessent in Marketo gelöscht wird (aber nicht in Dynamics) und danach in Dynamics aktualisiert wird, würde es eine neue Person in Marketo schaffen (gleiche E-Mail-Adresse, neue Personen-ID).

* Wenn ein Lead in Dynamics (aber nicht in Marketo) gelöscht wird und dann durch die Flusshandlung &quot;Synchronisierte Person mit Microsoft&quot; läuft, würde es einen neuen Lead in Dynamics schaffen.
