---
unique-page-id: 10094576
description: Dauerhaftes Abmelden - Marketing Docs - Produktdokumentation
title: Dauerhaftes Abmelden
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Dauerhaftes Abmelden {#durable-unsubscribe}

Marketo hat das Verhalten der Funktion zum Abmelden verbessert, um sie &quot;dauerhaft&quot;zu machen. Wir haben einen Übergeordnet-E-Mail-Status hinzugefügt, der sich von der Markierung für das Abbestellen unterscheidet, die auf dem Personendetaildatensatz sichtbar ist.

Wenn das Flag zum Abmelden von &quot;false&quot;auf &quot;true&quot;gesetzt ist, wird der Übergeordnet-E-Mail-Status aktualisiert und die Änderung an andere Personen mit derselben E-Mail-Adresse weitergeleitet. Wenn eine Person entfernt und neu erstellt wird oder wenn ein neuer Datensatz mit derselben E-Mail-Adresse erstellt wird, wird das Flags zum Abmelden **nicht** überschrieben.

>[!NOTE]
>
>Dauerhaftes Abmelden funktioniert auf allen Partitionen in Ihrer gesamten Marketo-Datenbank.

## Aktualisieren Sie die Markierung &quot;Abmelden&quot;von &quot;True&quot;auf &quot;False&quot;(z. B. &quot;Eine Person erneut abonnieren&quot;). {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Es gibt mehrere Möglichkeiten, wie eine Person erneut abonniert werden kann.

In Salesforce **löschen** Sie das Feld E-Mail-Opt-out im Datensatz des Interessenten/Kontakts. Dies wird mit Marketo synchronisiert.

![](assets/one.png)

Deaktivieren Sie in Marketo auf der Registerkarte &quot;Info&quot;des Datensatzes der Person das Feld zum Abmelden **** .

![](assets/two.png)

Führen Sie einen **Datenwert** ändern-Flussschritt wie unten gezeigt für eine oder mehrere Personen aus.

![](assets/three.png)

Aktualisieren einer vorhandenen Person über die SOAP-API

## Erstellen einer neuen Person {#creating-a-new-person}

Wenn eine neue Person erstellt wird, prüft Marketo sie anhand der Übergeordnet erstellten E-Mail-Statustabelle. Wenn die Person zuvor nicht abonniert wurde, wird der Datensatz aktualisiert, damit er nicht mehr abonniert werden kann.

## Ändern einer E-Mail-Adresse {#changing-an-email-address}

Wenn Sie die E-Mail-Adresse einer Person in eine nicht abonnierte E-Mail-Adresse ändern, wird diese Person abgemeldet. Diese Änderung kann entweder in Marketo oder Salesforce auftreten.

Wenn Sie eine abonnierte E-Mail-Adresse in eine abonnierte ändern, wird diese Person abonniert.

## Abonnement erneut abonnieren {#re-subscribing}

Ebenso wie ein Abmelden dazu führen würde, dass alle Personen mit derselben E-Mail-Adresse abgemeldet würden, würde ein erneutes Abonnieren tatsächlich jede Person mit derselben E-Mail-Adresse erneut abonnieren.

## Aktivitäten-Protokoll {#activity-log}

Definitionen der Datenwertänderung für *updateLeadEmailStatus* und *resetLeadEmailStatus* finden Sie in [diesem Community-Artikel](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!NOTE]
>
>**Verwandte Artikel**
>
>[Abmelden](understanding-unsubscribe.md)

