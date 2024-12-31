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

Ein numerischer Titel, der die Adresse eines Computers angibt, der mit dem Internet verbunden ist.

## Was sind freigegebene IP-Adressen? {#what-are-shared-ip-addresses}

Dies bezieht sich auf den Fall, dass mehrere Absender dieselben IP-Adressen verwenden, um E-Mail-Kampagnen zu starten. Sie nutzen alle dieselben Versand-IPs.

## Was ist eine dedizierte IP-Adresse? {#what-is-a-dedicated-ip-address}

Eine benutzerspezifische IP-Adresse, von der nur ein Absender sendet.

## Was ist besser - Shared oder Dedicated? {#which-is-better-shared-or-dedicated}

Wie üblich gibt es für beide Optionen Vor- und Nachteile.

**Vor- und Nachteile einer dedizierten IP**

_Vorteile_

**Reputation** - Sie besitzen Ihre Reputation und Zustellbarkeit.\
**Monitoring** - Durch die Überwachung der Zustellbarkeitsberichte können Sie schnell auf Änderungen an Ihren Versandmetriken reagieren.\
**Problembehebung** - Es ist einfacher, Bereitstellungsprobleme zu untersuchen, zu verstehen und zu lösen.

_Nachteile_

**Volumenänderungen** - Volumenspitzen können sich negativ auf Ihre Reputation auswirken und müssen bewältigt werden.\
**IP-Aufwärmprozess** - Reputation wird im Laufe der Zeit aufgebaut. Einige Internet Service Provider (ISPs) drosseln IP-Adressen ohne Volumenverlauf, sodass Sie in den ersten Wochen eine Reputation aufbauen müssen (Marketo kann Ihnen dabei helfen).\
**Kosten** - Für den Versand über eine dedizierte IP bei einem beliebigen Anbieter fallen in der Regel zusätzliche Kosten an.

**Vor- und Nachteile einer freigegebenen IP**

_Vorteile_

**Gute Mitbewohner** - Wenn die Personen, mit denen Sie Ihre IP teilen, Best Practices beim Versand befolgen, würden Sie davon profitieren.\
**Mailing-Häufigkeit** - Im Gegensatz zu dedizierten IPs ist keine Mindest-Mailing-Häufigkeit erforderlich, um sich für eine freigegebene IP zu qualifizieren.\
**Kosten** - Für den Versand von einer freigegebenen IP-Adresse fallen keine zusätzlichen Kosten an.

_Nachteile_

**Schlechte Mitbewohner** - Wenn die Personen, mit denen Sie Ihre IP teilen, schlechte Versandpraktiken anwenden, können Ihre E-Mail-Kampagnen beeinträchtigt sein.\
**Kontrolle** - Sie haben viel weniger Kontrolle über Ihre Absender-Reputation.\
**Problembehebung** - Es kann häufig schwieriger sein, ein Problem beim Senden von über freigegebene IPs zu beheben.

>[!NOTE]
>
>Bei einer Entscheidung muss ein weiterer wichtiger Faktor berücksichtigt werden: das Versandvolumen. Wenn Sie weniger als 100.000 E-Mails pro Monat oder weniger als zwei Mailings pro Monat versenden möchten, profitieren Sie wahrscheinlich nicht von einer dedizierten IP-Adresse. Solche Zahlen werden als niedrig eingestuft, und es wäre schwierig, Ihre dedizierte IP so „warm“ zu halten, dass sie von den wichtigsten ISPs als sicher angesehen wird. Wenn Sie nicht häufig genug E-Mails senden, sehen die ISPs im Grunde einen E-Mail-Versand als einen plötzlichen Aktivitätsschub und blockieren ihn möglicherweise als verdächtigen Spam.

Wenden Sie sich bei Fragen oder Interesse an der Einrichtung einer dedizierten IP-Adresse an Ihren Marketo-Vertriebsmitarbeiter.
