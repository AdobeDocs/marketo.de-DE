---
unique-page-id: 45417322
description: Löschen eines Leads oder Kontakts - Marketo Docs - Produktdokumentation
title: Lead oder Kontakt löschen
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Lead oder Kontakt löschen {#deleting-a-lead-or-contact}

Beim Löschen von Leads/Kontakten in Microsoft Dynamics sind einige Dinge zu beachten.

* Marketo Engage löscht Personen nicht automatisch, nur weil Leads in Dynamics gelöscht wurden. Stattdessen wird die Markierung &quot;Microsoft ist gelöscht&quot;auf &quot;true&quot;gesetzt. Sie können dieses Feld bei Bedarf ausblenden, um den Datensatz in Marketo zu löschen.

* Aktion &quot;Person löschen&quot;: Dadurch wird nur eine Person in Marketo gelöscht (es ist keine Option verfügbar, diese auch in Dynamics zu löschen).

* Wenn ein Lead in Marketo (aber nicht in Dynamics) gelöscht und anschließend in Dynamics aktualisiert wird, wird in Marketo eine neue Person erstellt (dieselbe E-Mail-Adresse, neue Personen-ID).

* Wenn ein Lead in Dynamics gelöscht wird (aber nicht in Marketo) und anschließend die Durchlaufaktion &quot;Person mit Microsoft synchronisieren&quot;ausgeführt wird, würde in Dynamics ein neuer Lead erstellt.
