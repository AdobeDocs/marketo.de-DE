---
unique-page-id: 2950396
description: Priorität, Dringlichkeit, relatives Ergebnis und Best Bets - Marketo-Dokumente - Produktdokumentation
title: Priorität, Dringlichkeit, relative Punktzahl und Best Bets
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Priorität, Dringlichkeit, relativer Wert und [!DNL Best Bets] {#priority-urgency-relative-score-and-best-bets}

[!DNL Marketo Sales Insight] wählt die besten Leads und Kontakte anhand ihrer Priorität aus. Die Priorität eines Leads oder Kontakts besteht aus zwei Komponenten: Dringlichkeit und relativer Punktzahl.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Diese werden aus dem Lead-Score abgeleitet - einem Maß für das Interesse der Person an Ihren Produkten. Je höher die Punktzahl ist, desto wahrscheinlicher ist es, dass der Kunde positiv auf einen Anruf Ihres Vertriebsteams reagiert.

>[!NOTE]
>
>Sie benötigen mehrere Scoring-Kampagnen, um den vollen Wert aus Priorität, Dringlichkeit und relativem Score zu erhalten.  Mit zu wenigen oder gar keinen Scoring-Kampagnen sind diese Felder nicht nützlich.

## Dringlichkeit {#urgency}

Die Flammen zeigen die Dringlichkeit — wie sehr sich die Bewertung dieser Person in letzter Zeit geändert hat. Eine hohe Dringlichkeit (mehr Flammen) bedeutet, dass die Punktzahl dieses Leads in letzter Zeit stark zugenommen hat. Dies ist ein gutes Zeichen dafür, dass dieser Lead an Ihrem Angebot interessiert ist. Du solltest schnell mit dieser Person Kontakt aufnehmen!

So wird beispielsweise ein Lead, der eine Demo angefordert und mehrere Web-Seiten besucht hat, wahrscheinlich eine sehr hohe Dringlichkeit haben. Leads, die Ihre Web-Seite nicht besucht oder Ihre E-Mails nicht geöffnet haben, haben eine niedrige Dringlichkeit. Dringlichkeit verwenden, um zu priorisieren, wer als Nächstes kontaktiert werden muss.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Relative Bewertung {#relative-score}

Die Sterne stellen einen relativen Wert dar - ein Maß dafür, wie der Lead-Wert dieser Person im Vergleich zum Wert aller anderen abschneidet. Ein hoher relativer Wert bedeutet, dass diese Person wahrscheinlich mehr an Ihrem Angebot interessiert und darüber informiert ist als Personen mit niedrigeren relativen Werten.

Wenn zwei Leads dieselbe Dringlichkeit haben, können Sie anhand der relativen Punktzahl ermitteln, wer zuerst einen Telefonanruf verdient. Die Person mit der höheren relativen Bewertung kann besser auf Ihr Angebot reagieren als die niedrigere.

## [!DNL Best Bets] {#best-bets}

Ihre [!DNL Best Bets] sind Ihre Leads und Kontakte mit der höchsten Dringlichkeit und relativen Punktzahl. Nur die Leads, deren Inhaber Sie sind, sind in dieser Liste sichtbar und die Liste wird aktualisiert, wenn sich die Lead-Bewertungen ändern.

>[!NOTE]
>
>Wenn Ihre besten Einsätze nicht den besten Leads und Kontakten entsprechen, die Sie besitzen, sprechen Sie mit jemandem in Ihrem Unternehmen, der Zugriff auf Marketo hat, über die Aktualisierung Ihrer [Scoring-Regeln](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Berechnen der Dringlichkeit und des relativen Werts

Um die Anzahl der Sterne und Flammen zu berechnen, werden Ihre Leads und Kontakte zunächst nach Bewertung oder Bewertungsänderung (für „Relativ“ bzw. „Dringlichkeit„) sortiert. Dann werden sie in verschiedene Stufen unterteilt — die oberste Stufe erhält die meisten Sterne oder Flammen, die nächste weniger und so weiter.

Wenn sich die Bewertungen ändern, werden Dringlichkeit, Priorität und relative Werte der Bewertung sofort neu berechnet. Die Dringlichkeits- und Bewertungsstufen werden auf den Marketo-Servern automatisch jede Nacht berechnet.

>[!NOTE]
>
>Die Zahlen für die relative Dringlichkeit (Flammen) und die relative Bewertung (Sterne) sind in Marketo ganze Zahlen. Mögliche Werte für jede sind 0-3.
