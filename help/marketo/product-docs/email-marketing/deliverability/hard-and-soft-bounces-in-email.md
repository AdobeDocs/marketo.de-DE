---
unique-page-id: 1147328
description: Hard- und Softbounces in E-Mail - Marketo Docs - Produktdokumentation
title: Hard- und Softbounces in E-Mails
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Hard- und Softbounces in E-Mails {#hard-and-soft-bounces-in-email}

Bei einem Hardbounce kann die E-Mail-Adresse einer Person ungültig werden, wenn ein Mailserver Marketo mitteilt, dass die E-Mail-Adresse der Person nicht zugestellt werden kann. Ein Softbounce bedeutet, dass bei der Zustellung der E-Mail an die Person etwas schiefgelaufen ist. wird automatisch aufgelöst und kann manchmal Tage dauern. Hard- und Softbounces bestehen aus [mehrere Kategorien](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Bounce-Classification {#bounce-classification}

In Marketo gibt es fünf Personenketten, die sich auf den problemlosen E-Mail-Versand beziehen.

1. **E-Mail ausgesetzt** - Auf True setzen, wenn ein bestimmter Hardbounce-Typ auftritt.
1. **Ausgesetzte E-Mail-Ursache** - Es kann viele Gründe geben. In diesem Feld wird versucht, die Ursache zu erklären.
1. **E-Mail ausgesetzt bei** - Wenn der fehlerhafte Bounce auftritt, setzt Marketo den Versand an die Person für 24 Stunden ab diesem Zeitstempel aus.
1. **Email Invalid** - Auf True setzen, wenn ein bestimmter Hardbounce-Typ auftritt.
1. **E-Mail-ungültige Ursache** - Der Grund für den Hardbounce.

>[!NOTE]
>
>Wenn eine Person **E-Mail ausgesetzt** Status, es gibt keine Möglichkeit, das Kontrollkästchen E-Mail ausgesetzt zu deaktivieren. Die Person wird jedoch noch 24 Stunden nach der ersten Aussetzung in Mailboxen versenden.
>
>Wenn eine Person als **email invalid**, können sie nur manuell zurückgesetzt werden (was wir Ihnen nur empfehlen, wenn Sie wissen, dass ihre E-Mail gültig ist), indem Sie das Kontrollkästchen &quot;E-Mail ungültig&quot;auf der Registerkarte &quot;Personen-Info&quot;ihres Datensatzes deaktivieren.

>[!PREREQUISITES]
>
>Folgen [diese Schritte](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) , um einen E-Mail-Leistungsbericht zu erstellen, der Bounce-Daten generiert.

Nach der Erstellung Ihres E-Mail-Leistungsberichts sollte Ihr Bildschirm in etwa wie folgt aussehen:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Spamfilter erzeugen manchmal Hardbounces. Diese &quot;Falsch-Positiv-Werte&quot;sind kein Hinweis auf die wahre Gültigkeit der E-Mail-Adresse der Person.
