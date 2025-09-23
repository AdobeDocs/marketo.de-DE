---
unique-page-id: 1147328
description: Hardbounces und Softbounces in E-Mails - Marketo-Dokumente - Produktdokumentation
title: Hard- und Softbounces in E-Mails
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 15%

---

# Hard- und Softbounces in E-Mails {#hard-and-soft-bounces-in-email}

Ein Hardbounce kann die E-Mail-Adresse einer Person ungültig machen, wenn ein Mailserver Marketo mitteilt, dass die E-Mail der Person nicht zugestellt werden kann. Ein Softbounce bedeutet, dass beim Versand der E-Mail an die Person etwas schiefgelaufen ist. Dies wird automatisch behoben und kann manchmal Tage dauern. Sowohl Hardbounces als auch Softbounces weisen [verschiedene Kategorien](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838) auf.

## Bounce-Klassifizierung {#bounce-classification}

Es gibt 5 Personen-Zeichenfolgen in Marketo, die mit einem problematischen E-Mail-Versand zusammenhängen.

1. **E-Mail ausgesetzt** - Auf „True“ gesetzt, wenn ein bestimmter Hardbounce auftritt.
1. **Grund für ausgesetztes E-Mail** - Es kann viele Gründe geben. Dieses Feld versucht, die Ursache zu erklären.
1. **E-Mail ausgesetzt um** - Wenn der fehlerhafte Bounce auftritt, setzt Marketo den Versand an die Person für 24 Stunden ab diesem Zeitstempel aus.
1. **E-Mail ungültig** - Auf „True“ gesetzt, wenn ein bestimmter Typ von Hardbounce auftritt.
1. **Ungültige E-Mail-**: Der Grund für den Hardbounce.

>[!NOTE]
>
>Nachdem eine Person den Status **E-Mail ausgesetzt** erreicht hat, gibt es keine Möglichkeit, das Kontrollkästchen „E-Mail ausgesetzt“ zu deaktivieren. Die Person wird jedoch 24 Stunden nach der ersten Aussetzung noch per E-Mail erreichbar sein.
>
>Wenn eine Person als **E-Mail ungültig** markiert wird, kann sie nur manuell zurückgesetzt werden (was wir nur empfehlen, wenn Sie wissen, dass ihre E-Mail-Adresse mit Sicherheit gültig ist), indem Sie das Kontrollkästchen „E-Mail ungültig“ auf der Registerkarte Personeninformationen ihres Datensatzes deaktivieren.

>[!PREREQUISITES]
>
>Führen Sie [diese Schritte](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) aus, um einen E-Mail-Leistungsbericht zu erstellen, der Bounce-Daten generiert.

Nach der Erstellung des E-Mail-Leistungsberichts sollte Ihr Bildschirm etwa wie folgt aussehen:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Spam-Filter verursachen manchmal Hardbounces. Diese „falsch-positiven Ergebnisse“ sind kein Hinweis auf die wahre Gültigkeit der E-Mail-Adresse der Person.
