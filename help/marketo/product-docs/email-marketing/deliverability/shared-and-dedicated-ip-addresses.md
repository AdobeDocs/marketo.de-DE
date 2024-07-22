---
unique-page-id: 10912085
description: Freigegebene und dedizierte IP-Adressen - Marketo-Dokumente - Produktdokumentation
title: Freigegebene und dedizierte IP-Adressen
exl-id: 3d7a78f4-531a-4ad7-a20b-1385bd62d1d9
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Freigegebene und dedizierte IP-Adressen {#shared-and-dedicated-ip-addresses}

## Was ist eine IP-Adresse? {#what-is-an-ip-address}

Ein numerischer Titel, der die Adresse eines mit dem Internet verbundenen Computers angibt.

## Was sind freigegebene IP-Adressen? {#what-are-shared-ip-addresses}

Dies bezieht sich auf die Fälle, in denen mehrere Absender dieselben IP-Adressen zum Starten von E-Mail-Kampagnen verwenden. Sie teilen alle dieselben Sende-IPs.

## Was ist eine dedizierte IP-Adresse? {#what-is-a-dedicated-ip-address}

Eine benutzerspezifische IP-Adresse, von der nur ein Absender sendet.

## Was ist besser - freigegeben oder dediziert? {#which-is-better-shared-or-dedicated}

Wie üblich gibt es Vor- und Nachteile für beide Optionen.

**Vorteile und Nachteile einer dedizierten IP**

_pros_

**Reputation** - Sie sind vollständig Eigentümer Ihrer Reputation und Zustellbarkeit.\
**Überwachung** - Durch die Überwachung Ihrer Zustellbarkeitsberichte können Sie schnell auf Änderungen in Ihren Versandmetriken reagieren.\
**Problemlösung** - Es ist einfacher, Bereitstellungsprobleme zu untersuchen, zu verstehen und zu lösen.

_cons_

**Volumenänderungen** - Volumenspitzen können sich negativ auf Ihre Reputation auswirken und müssen verwaltet werden.\
**IP-Warmup-Prozess** - Der Ruf wird im Laufe der Zeit aufgebaut. Einige Internet Service Provider (ISPs) drosseln IP-Adressen ohne Volumenverlauf, sodass Sie in den ersten Wochen eine Reputation aufbauen müssen (Marketo kann Ihnen helfen).\
**Kosten** - In der Regel fallen zusätzliche Gebühren an, die von einer dedizierten IP-Adresse an einen beliebigen Anbieter gesendet werden.

**Vorteile und Nachteile einer freigegebenen IP-Adresse**

_pros_

**Gute Mitbewohner** - Wenn die Personen, die Ihre IP-Adresse mit Best Practices teilen, den Versand befolgen, würden Sie davon profitieren.\
**Versandhäufigkeit** - Im Gegensatz zu dedizierten IPs ist keine minimale Versandhäufigkeit erforderlich, um sich für eine freigegebene IP zu qualifizieren.\
**Kosten** - Es fallen niemals zusätzliche Gebühren an, die von einer freigegebenen IP-Adresse gesendet werden.

_cons_

**Unangemessene Mitbewohner** - Wenn die Personen, für die Sie Ihre IP-Adresse freigeben, schlechte Versandpraktiken anwenden, können Ihre E-Mail-Kampagnen beeinträchtigt sein.\
**Kontrolle** - Sie haben wesentlich weniger Kontrolle über die Reputation Ihres Absenders.\
**Problemlösung** - Es kann oft schwieriger sein, ein Problem beim Senden von freigegebenen IPs zu lösen.

>[!NOTE]
>
>Bei der Entscheidungsfindung ist ein weiterer wichtiger Faktor zu beachten: die Sendemenge. Wenn Sie planen, weniger als 100.000 E-Mails pro Monat oder weniger als zwei Mailings pro Monat zu versenden, profitieren Sie wahrscheinlich nicht von einer dedizierten IP. Das Senden von Nummern wie diese werden als niedrig betrachtet, und es wäre schwierig, Ihre dedizierte IP so &quot;warm&quot;zu halten, dass sie von den wichtigsten ISPs als sicher betrachtet werden. Wenn Sie nicht oft genug Nachrichten senden, sehen die ISPs einen E-Mail-Versand als plötzlichen &quot;Anstieg&quot;der Aktivität und blockieren ihn möglicherweise als Spam.

Wenden Sie sich bei Fragen oder Interesse an der Einrichtung einer dedizierten IP-Adresse an Ihren Marketo-Vertriebsmitarbeiter.
