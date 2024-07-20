---
unique-page-id: 2953188
description: Abgeleitete Filter - Marketo Docs - Produktdokumentation
title: Abgeleitete Filter
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Abgeleitete Filter {#inferred-filters}

Wenn ein Besucher Ihre Website besucht, werden diese von [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} Cookies gesetzt und in das System eingefügt. Wir suchen ihre IP-Adresse in einer speziellen Datenbank und schließen alle möglichen Informationen ab.

>[!NOTE]
>
>Um sicherzustellen, dass die abgeleiteten Feldwerte aktuell bleiben, aktualisieren wir regelmäßig die Datenbank, die für die IP-Adressen-Suche verwendet wird. Datenbankaktualisierungen können neue abgeleitete Feldwerte einführen, die Sie möglicherweise zu Filterdefinitionen für Smart-Listen hinzufügen müssen.
>
>Datenbankaktualisierungen können während einer [Marketo Engage-Produktversion](/help/marketo/release-notes/release-schedule.md){target="_blank"} auftreten. Wenn eine Aktualisierung durchgeführt wird, enthalten die [Marketo Engage-Versionshinweise](/help/marketo/release-notes/current.md){target="_blank"} eine Erläuterung aller Änderungen an den zurückgewiesenen Feldwerten.

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

Wenn Sie einen dieser Filter in einer Smart-Liste verwenden, liefern die Ergebnisse Personen mit diesen daraus resultierenden Informationen.

>[!TIP]
>
>Verwenden Sie diese Filter in einem Webaktivitätsbericht. Verwenden Sie die Territorien der Vertriebsmitarbeiter und melden Sie sie in den letzten 24 Stunden für einen benutzerspezifischen täglichen Bericht mit Website-Besuchern an. Sie werden es lieben!
>
>* Besuchte Webseite - Letzte 24 Stunden
>* Der Status &quot;Abgegrenzt&quot;ist [Auswählen ihres Hoheitsgebiets]

Diese anonymen Besucher werden automatisch in Personen umgewandelt, wenn sie auf einen E-Mail-Link klicken oder ein Formular ausfüllen. Sie bewahren jedoch alle enthaltenen Informationen auf.

>[!NOTE]
>
>Erfahren Sie mehr über [anonyme Aktivitäten und Leads](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}.
