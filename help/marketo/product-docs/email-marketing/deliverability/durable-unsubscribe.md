---
unique-page-id: 10094576
description: Dauerhafte Abmeldung - Marketo-Dokumente - Produktdokumentation
title: Dauerhafte Abmeldung
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 35f5b33b01462b1cd00e29360daee465c7f18cf0
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Dauerhafte Abmeldung {#durable-unsubscribe}

Marketo hat das Verhalten der Abmeldefunktion verbessert, um sie &quot;dauerhaft&quot;zu machen. Wir haben einen Master-E-Mail-Status hinzugefügt, der sich von der Abmelde-Markierung unterscheidet, die auf dem Personendetaildatensatz angezeigt wird.

Wenn das Abmelde-Flag von false auf true gesetzt ist, wird der Master-E-Mail-Status aktualisiert und die Änderung wird an andere Personen mit derselben E-Mail-Adresse weitergeleitet. Wenn eine Person entfernt und neu erstellt wird oder wenn ein neuer Datensatz mit derselben E-Mail-Adresse erstellt wird, wird das Abmelde-Flag **not** überschrieben werden.

>[!NOTE]
>
>Die Funktion &quot;Dauerhaftes Abmelden&quot;funktioniert auf allen Partitionen in Ihrer gesamten Marketo-Datenbank.

## Aktualisieren Sie das Abmelde-Flag von True auf False (z. B. Abonnieren einer Person erneut). {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Es gibt mehrere Möglichkeiten, eine Person erneut anzumelden.

In Salesforce **clear** das Feld E-Mail-Opt-out auf dem Datensatz des Leads/Kontakts. Dies wird mit Marketo synchronisiert.

![](assets/one.png)

In Marketo **clear** im Tab Informationen des Datensatzes der Person das Feld für die Abmeldung.

![](assets/two.png)

Führen Sie einen **Datenwert ändern** Flussschritt wie unten gezeigt für ein oder mehrere Personen.

![](assets/three.png)

Aktualisieren einer vorhandenen Person über die SOAP-API.

## Erstellen einer neuen Person {#creating-a-new-person}

Wenn eine neue Person erstellt wird, prüft Marketo sie anhand der Master-E-Mail-Statustabelle. Wenn die Person zuvor abgemeldet wurde, werden wir den Datensatz aktualisieren, der abgemeldet werden soll.

## E-Mail-Adresse ändern {#changing-an-email-address}

Wenn Sie die E-Mail-Adresse einer Person in eine abgemeldete E-Mail-Adresse ändern, wird diese Person abgemeldet. Diese Änderung kann entweder in Marketo oder in Salesforce vorgenommen werden.

Wenn Sie eine abgemeldete E-Mail-Adresse in eine abonnierte Adresse ändern, wird diese Person abonniert.

## Erneute Anmeldung {#re-subscribing}

So wie eine Abmeldung dazu führen würde, dass sich alle Personen mit derselben E-Mail-Adresse abmelden, würde eine erneute Anmeldung tatsächlich jede Person mit derselben E-Mail-Adresse erneut abonnieren.

>[!MORELIKETHIS]
>
>[Grundlegendes zur Abmeldung](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
