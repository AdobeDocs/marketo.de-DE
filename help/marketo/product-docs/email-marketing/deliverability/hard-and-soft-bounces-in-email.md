---
unique-page-id: 1147328
description: Hard- und Soft Bounces in E-Mail - Marketing Docs - Produktdokumentation
title: Hard- und Soft Bounces in E-Mail
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Harte und weiche Absprünge in E-Mail {#hard-and-soft-bounces-in-email}

Bei einem harten Absprung kann die E-Mail-Adresse einer Person ungültig werden, wenn ein E-Mail-Server Marketo mitteilt, dass die E-Mail der Person nicht zugestellt werden kann. Ein weicher Absprung bedeutet, dass etwas bei der Übermittlung der E-Mail an die Person schiefgelaufen ist. wird automatisch aufgelöst und kann manchmal Tage dauern. Sowohl feste als auch weiche Absprünge bestehen aus [mehreren Kategorien](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Absprungklassifizierung {#bounce-classification}

In Marketo gibt es fünf Personen-Zeichenfolgen, die mit problembelasteten E-Mail-Versänden in Zusammenhang stehen.

1. **E-Mail ausgesetzt** : Auf &quot;True&quot;setzen, wenn ein bestimmter Typ von Absprung auftritt.
1. **E-Mail ausgesetzte Ursache**  - Es kann viele Gründe geben. Dieses Feld versucht, die Ursache zu erklären.
1. **E-Mail ausgesetzt am** : Wenn der verletzende Absprung eintritt, setzt Marketo den Versand an die Person für 24 Stunden ab diesem Zeitstempel aus.
1. **E-Mail ungültig** : Auf &quot;True&quot;setzen, wenn ein bestimmter Typ von Absprung auftritt.
1. **E-Mail-Ungültige Ursache**  - Der Grund für den Absprung.

>[!NOTE]
>
>Wenn eine Person den Status **E-Mail ausgesetzt** erreicht hat, kann das Kontrollkästchen &quot;E-Mail ausgesetzt&quot;nicht mehr gelöscht werden. Die Person wird jedoch noch 24 Stunden nach der ersten Aussetzung versandfähig.
>
>Wenn eine Person als **E-Mail ungültig** markiert ist, kann sie nur manuell zurückgesetzt werden (was wir Ihnen nur empfehlen, wenn Sie wissen, dass ihre E-Mail gültig ist), indem Sie das Feld &quot;E-Mail ungültig&quot;auf der Registerkarte &quot;Personeninfo&quot;ihres Datensatzes deaktivieren.

>[!PREREQUISITES]
>
>Führen Sie [diese Schritte](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) aus, um einen E-Mail-Leistungsbericht zu erstellen, der Absprungdaten generiert.

Nach der Erstellung des E-Mail-Leistungsberichts sollte Ihr Bildschirm wie folgt aussehen:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Spam-Filter erzeugen manchmal harte Absprünge. Diese &quot;Falsch-Positiv-Werte&quot;sind kein Hinweis auf die tatsächliche Gültigkeit der E-Mail-Adresse der Person.
