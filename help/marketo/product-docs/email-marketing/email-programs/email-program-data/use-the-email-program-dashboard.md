---
unique-page-id: 2359476
description: Verwenden des Dashboards "E-Mail-Programm"- Marketo-Dokumente - Produktdokumentation
title: Verwenden des Dashboards E-Mail-Programm
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: b2ceefb068005d916027fb71be0dc4e25849ae23
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Verwenden des Dashboards E-Mail-Programm {#use-the-email-program-dashboard}

In dieser Dashboard-Ansicht erfahren Sie, wie Ihre E-Mail-Programme funktionieren.

>[!CAUTION]
>
>Für genaue Berichte vermeiden Sie _Wiederverwendung_ eine E-Mail aus einem E-Mail-Programm, entweder durch Referenzierung in einer Smart-Kampagne oder durch Verschieben des Assets aus dem gestarteten E-Mail-Programm in ein neues. Auf diese Weise werden alle Daten in jedem Bericht-Dashboard, das an diese E-Mail angehängt ist, aggregiert. Wenn Sie eine E-Mail wiederverwenden müssen, wenden Sie sich bitte an [Klonen](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"} , da dadurch die E-Mail kopiert, aber eine neue mit einer neuen E-Mail-ID erstellt wird.

>[!NOTE]
>
>Wenn Ihr Programm über einen A/B-Test verfügt, überprüfen Sie die [E-Mail-Programm-Dashboard - A/B-Testansicht](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}.

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>Alle Daten in dieser Ansicht sind aggregiert (einschließlich A/B-Test und E-Mail-Versand).

## E-Mail gesendet {#email-send}

Hier können Sie sehen, wie viele E-Mails gesendet, abgeschnitten und zugestellt wurden.

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>Aufgrund von E-Mail-Zustellbarkeitsstandards, die außerhalb der Kontrolle von Marketo liegen, sind die Statistiken &quot;Bounce&quot;und &quot;Delivered&quot;ungefährlich und nicht exakt.

## Öffnungen/Klicks {#opens-clicks}

Diese Grafik zeigt die Anzahl der geöffneten/angeklickten E-Mails während eines bestimmten Zeitraums nach der Ausführung des E-Mail-Programms.

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>Beachten Sie, wie die Anzahl der Öffnungen/Klicks mit der Zeit abnimmt.

## Zusammenfassung - Interaktion {#summary-engagement}

Dies zeigt Ihnen die Gesamtübersicht [Interaktionswert](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

![](assets/image2014-9-12-14-3a13-3a11.png)

## Zusammenfassung - Rest {#summary-rest}

Der Rest der Daten zeigt Öffnungen, Klicks, Klick-/Öffnungsverhältnis und Abmeldungen an.

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>Die **Abmelden** Die im obigen Beispiel angegebene Rate war so klein, dass Marketo einzoomte, um Ihnen einen besseren Einblick zu geben. Die zweite Zahl innerhalb der Leiste wird lediglich als Skalierungswert hinzugefügt.

>[!NOTE]
>
>**Definition**
>
>**Öffnungen** werden gezählt, wenn der E-Mail-Empfänger die E-Mail-Bilder herunterlädt, die ein von Marketo eingefügtes Tracking-Pixel enthalten. Wenn der Empfänger die E-Mail anzeigt, aber keine Bilder herunterlädt, zählt dies nicht als Öffnung. Wenn die Bilder im Vorschaufenster des Empfängers geladen werden, zählt dies normalerweise als Öffnung, doch variiert dies je nach E-Mail-Client.
>
>**Zum Öffnen klicken** misst den Prozentsatz der E-Mails, die sowohl geöffnet als auch in der E-Mail auf einen Link geklickt wurden. Wir nehmen die Anzahl der Einzelklicks dividiert durch die Anzahl der Einzelöffnungen und multiplizieren sie dann mit 100, um sie als Prozentsatz anzuzeigen.

## Dashboard aktualisieren {#refresh-dashboard}

Um die aktuellsten Daten anzuzeigen, klicken Sie einfach auf das Aktualisierungssymbol im Dashboard.

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[Verwenden des Dashboards &quot;E-Mail-Programm&quot;- A/B-Testansicht](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
