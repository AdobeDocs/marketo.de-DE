---
unique-page-id: 10094576
description: Erfahren Sie mehr über dauerhafte Abmeldungen und darüber, wie sich der Master-E-Mail-Status über Personen hinweg ausbreitet. Verwalten von Abonnements und Personendatensätzen in Marketo.
title: Dauerhafte Abmeldung
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
TQID: https://experienceleague.adobe.com/Zr7XyDDSHtWW4lp4ATAM6xlPrNnTJlqoOOjjln-YuqI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 304
ht-degree: 1%

---

# Dauerhafte Abmeldung {#durable-unsubscribe}

Marketo hat das Verhalten der Abmeldefunktion verbessert, sodass sie „dauerhaft“ ist. Es wurde ein E-Mail-Master-Status hinzugefügt, der getrennt von der Abmelde-Markierung ist, die im Personendetaildatensatz sichtbar ist.

Wenn für das Abmelde-Flag „false“ die Einstellung „true“ festgelegt ist, wird der Master-E-Mail-Status aktualisiert und die Änderung wird an andere Personen mit derselben E-Mail-Adresse weitergegeben. Wenn eine Person entfernt und neu erstellt wird oder wenn ein neuer Datensatz mit derselben E-Mail-Adresse erstellt wird, wird das Abmelde-Flag **nicht** überschrieben.

>[!NOTE]
>
>Eine dauerhafte Abmeldung funktioniert auf allen Partitionen in der gesamten Marketo-Datenbank.

## Aktualisieren Sie das Abmelde-Flag von „True“ auf „False“ (z. B. erneutes Abonnieren einer Person). {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Es gibt mehrere Möglichkeiten, wie eine Person erneut abonniert werden kann.

Löschen Sie in Salesforce das Feld E-Mail-Abmeldung im Datensatz des Leads/Kontakts. Dadurch wird mit Marketo synchronisiert.

![Salesforce-Bildschirm](assets/durable-unsubscribe-1.png)

Deaktivieren Sie in Marketo das Feld Abgemeldet auf der Registerkarte Info des Datensatzes der Person.

![Löschen des Abmeldefelds in einem Personendatensatz](assets/durable-unsubscribe-2.png)

Führen Sie einen **[!UICONTROL Datenwert ändern]**-Flussschritt wie unten gezeigt auf einem oder mehreren Personen aus.

![Schritt „Datenwert-Fluss ändern“](assets/durable-unsubscribe-3.png)

## Erstellen einer neuen Person {#creating-a-new-person}

Wenn eine neue Person erstellt wird, vergleicht Marketo sie mit der übergeordneten E-Mail-Statustabelle. Wenn die Person sich zuvor abgemeldet hat, wird der Datensatz auf „Abgemeldet“ aktualisiert.

## E-Mail-Adresse ändern {#changing-an-email-address}

Wenn Sie die E-Mail-Adresse einer Person in eine abgemeldete E-Mail-Adresse ändern, wird diese Person abgemeldet. Diese Änderung kann entweder in Marketo oder [!DNL Salesforce] auftreten.

## Erneute Anmeldung {#re-subscribing}

Genau wie eine Abmeldung dazu führen würde, dass alle Personen mit derselben E-Mail-Adresse das Abonnement kündigen, wird eine Abmeldung auch jede Person mit derselben E-Mail-Adresse erneut abonnieren.

>[!MORELIKETHIS]
>
>[Grundlagen zum Abmelden](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
