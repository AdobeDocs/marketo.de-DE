---
unique-page-id: 2950396
description: Priorität, Dringlichkeit, relativer Punktstand und beste Bets - Marketo Docs - Produktdokumentation
title: Priorität, Dringlichkeit, relatives Ergebnis und beste Beta
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 3%

---

# Priorität, Dringlichkeit, relatives Ergebnis und beste Beta {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight wählt für Sie die besten Leads und Kontakte entsprechend der Priorität aus. Die Priorität eines Leads oder Kontakts besteht aus zwei Komponenten: Dringlichkeit und relatives Ergebnis.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Diese werden aus dem Lead-Score abgeleitet - einem Maß für das Interesse der Person an Ihrem Produkt/Ihren Produkten. Je höher das Ergebnis ist, desto wahrscheinlicher wird eine positive Reaktion auf einen Aufruf Ihres Verkaufsteams sein.

>[!NOTE]
>
>Sie benötigen mehrere Scoring-Kampagnen, um den vollen Wert aus Priorität, Dringlichkeit und relativem Ergebnis zu erhalten.  Bei zu wenigen oder gar keinen Scoring-Kampagnen sind diese Felder nicht nützlich.

## Dringlichkeit {#urgency}

Die Flammen stellen die Dringlichkeit dar - wie sehr sich das Lead-Ergebnis dieser Person in letzter Zeit geändert hat. Eine hohe Dringlichkeit (mehr Flammen) bedeutet, dass der Punktstand dieses Leads in letzter Zeit stark zugenommen hat. Es ist ein gutes Zeichen, dass dieser Lead an Ihrem Angebot interessiert ist. Du solltest diese Person schnell verfolgen!

Beispielsweise wird ein Lead, der eine Demo angefordert und mehrere Webseiten besucht hat, wahrscheinlich eine sehr hohe Dringlichkeit haben. Ein Lead, der Ihre Webseite nicht besucht oder Ihre E-Mails geöffnet hat, hat eine geringe Dringlichkeit. Verwenden Sie die Dringlichkeit, um die Personen zu priorisieren, die als Nächstes kontaktiert werden müssen.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Relative Bewertung {#relative-score}

Die Sterne stellen den relativen Wert dar - ein Maß dafür, wie der Lead-Wert dieser Person mit dem aller anderen verglichen wird. Eine hohe relative Punktzahl bedeutet, dass diese Person wahrscheinlich mehr Interesse an Ihrem Angebot hat als Personen mit niedrigeren relativen Punktzahlen.

Wenn zwei Leads die gleiche Dringlichkeit haben, können Sie mit dem relativen Wert feststellen, welche zuerst einen Anruf verdient. Der mit dem höheren relativen Ergebnis kann auf Ihr Angebot im Vergleich zum niedrigeren Angebot günstiger reagieren.

## Vielversprechende Kontakte {#best-bets}

Ihre besten Wetten sind Ihre Leads und Kontakte mit höchster Dringlichkeit und relativem Ergebnis. Nur die Leads, deren Inhaber Sie sind, sind in dieser Liste sichtbar und die Liste wird aktualisiert, wenn sich die Lead-Punktzahlen ändern.

>[!NOTE]
>
>Wenn Ihre besten Wetten nicht mit den besten Leads und Kontakten übereinstimmen, die Sie besitzen, sprechen Sie mit einer Person in Ihrem Unternehmen, die Zugriff auf Marketo hat, über die Aktualisierung Ihrer [Bewertungsregeln](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Berechnung von Dringlichkeit und relativer Punktzahl

Um die Anzahl der Sterne und Flammen zu berechnen, werden Ihre Leads und Kontakte zuerst nach Punktänderung oder Punktänderung sortiert (für relative Punktzahl bzw. Urnität). Dann sind sie in Stufen unterteilt — die oberste Ebene erhält die meisten Sterne oder Flammen, die nächste erhält weniger, und so weiter.

Wenn sich die Bewertungen ändern, werden Dringlichkeit, Priorität und relative Punktzahl sofort neu berechnet. Die Dringlichkeitsstufen und die relativen Punktzahlen werden auf Marketo-Servern jede Nacht automatisch berechnet.

>[!NOTE]
>
>Die Zählungen Relative Dringlichkeit (Flammen) und Relative Punktzahl (Sterne) sind Ganzzahlen in Marketo. Mögliche Werte sind 0-3.
