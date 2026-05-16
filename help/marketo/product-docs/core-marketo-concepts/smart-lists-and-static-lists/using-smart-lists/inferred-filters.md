---
unique-page-id: 2953188
description: Erfahren Sie mehr über abgeleitete Filter in Smart Lists. Verstehen, wie Marketo Filter aus verknüpften Assets ableitet.
title: Abgeleitete Filter
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
TQID: https://experienceleague.adobe.com/-dKeAfCxfD1ErbfBzLqARUMwFY-I9RdkWGC0b-ZtNyE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 218
ht-degree: 1%

---

# Abgeleitete Filter {#inferred-filters}

Wenn jemand Ihre Website besucht, [&#128279;](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} MunchkinCookies und legt sie im System ab. Das System sucht ihre IP in einer speziellen Datenbank und leitet alle Arten von Informationen ab.

>[!NOTE]
>
>Um sicherzustellen, dass die abgeleiteten Feldwerte auf dem neuesten Stand bleiben, wird die für die Suche nach IP-Adressen verwendete Datenbank regelmäßig aktualisiert. Datenbankaktualisierungen können neue abgeleitete Feldwerte einführen, die Sie ggf. den Filterdefinitionen für die Smart-Liste hinzufügen müssen.
>
>Datenbankaktualisierungen können während einer [Marketo Engage-Produktversion erfolgen](/help/marketo/release-notes/release-schedule.md){target="_blank"}. Wenn eine Aktualisierung erfolgt, enthalten die [Marketo Engage](/help/marketo/release-notes/current.md){target="_blank"}Versionshinweise eine Erläuterung aller Änderungen an abgeleiteten Feldwerten.

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

Wenn Sie einen dieser Filter in einer Smart List verwenden, ergeben die Ergebnisse Personen mit diesen abgeleiteten Informationen.

>[!TIP]
>
>Verwenden Sie diese Filter in einem Web-Aktivitätsbericht. Verwenden Sie die Gebiete der Vertriebsmitarbeiter und abonnieren Sie sie für einen benutzerdefinierten täglichen Bericht mit Website-Besuchern in den letzten 24 Stunden. Sie werden es lieben!
>
>* Besuchte Web-Seite - Letzte 24 Stunden
>* Abgeleiteter Staat ist [wählen Sie ihr Territorium]

Diese anonymen Besucher werden automatisch in Personen umgewandelt, wenn sie auf einen E-Mail-Link klicken oder ein Formular ausfüllen. Sie behalten jedoch alle abgeleiteten Informationen bei.

>[!NOTE]
>
>Weitere Informationen über [anonyme Aktivität und Leads](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}.
