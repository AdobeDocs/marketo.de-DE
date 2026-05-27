---
description: Erfahren Sie mehr über prädiktive Filter für die Zielgruppenbestimmung mit KI. Verwenden Sie Filter in Smart Lists und Kampagnen, um die richtigen Personen zu erreichen.
title: Vorhersagefilter
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
TQID: https://experienceleague.adobe.com/-P6jjTHT-YDpoEE6yg23rd48s3YYN4kzABbJwZp4rig
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: d0251300-e25f-466f-9856-7e11ce8fa7aaid: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 427
ht-degree: 3%

---

# Vorhersagefilter {#predictive-filters}

Als Teil der Predictive Audiences bietet Marketo eine Gruppe von KI-/ML-basierten Filtern in Smart Lists innerhalb von Smart-Kampagnen.

![Bild eins](assets/predictive-filters-1.png)

>[!NOTE]
>
>Die Filter „Wahrscheinlich anwesend“ und „Wahrscheinlich registriert“ können nur in Veranstaltungsprogrammen verwendet werden. „Wahrscheinlichkeit der Abmeldung“, „Lookalike der Programmmitglieder“ und „Lookalike der Mitglieder der Smart-Liste“ können in allen Programmtypen verwendet werden.

## Wahrscheinlichkeit der Teilnahme {#likelihood-to-attend}

Dieser Filter wird verwendet, um Ihre Audience effektiv einzugrenzen. Dies hilft Ihnen, Leads anzusprechen und einzuladen, die mit höherer Wahrscheinlichkeit an **Webinar** Veranstaltung teilnehmen. Beachten Sie, dass Ihr „Likelihood-Teilnahme-Programm“ Ihr aktuelles Veranstaltungsprogramm ist.

![Bild zwei](assets/predictive-filters-2.png)

## Wahrscheinlichkeit der Registrierung {#likelihood-to-register}

Verwenden Sie diesen Filter ähnlich wie _Filter &quot;_ Teilnahme“, um Ihre Audience einzugrenzen und Leads anzusprechen, die eine höhere Wahrscheinlichkeit haben, sich für Ihr Webinar **Ihre Veranstaltung** registrieren.

![Bild 3](assets/predictive-filters-3.png)

## Wahrscheinlichkeit der Abmeldung {#likelihood-to-unsubscribe}

Dadurch wird die Zielgruppe nach der Wahrscheinlichkeit gefiltert, dass sie sich in den nächsten zwei Wochen mit hoher oder geringer Wahrscheinlichkeit abmeldet. Sie können dies verwenden, um Leads mit hoher Ermüdung anders und effektiver anzusprechen. Der Schwellenwert für die Abmeldung ist dynamisch und wird von einem KI-Modell gesteuert, das mehrere Attribute berücksichtigt, darunter Vorlaufzeit in der Datenbank und Lead-Aktivitäten.

![Bild vier](assets/predictive-filters-4.png)

>[!NOTE]
>
>Die Filter „Wahrscheinlichkeit für die Teilnahme/Registrierung/Abmeldung“ müssen in Verbindung mit anderen Standardfiltern verwendet werden.

## Lookalike der Programmmitglieder/Lookalike der Mitglieder der Smart-Liste {#lookalike-of-members}

Mit diesen beiden Filtern können Sie Ihre aktuelle Audience erweitern, indem Sie zusätzliche Leads ansprechen, die Mitgliedern eines anderen Programms oder einer Smart List ähnlich sind. Die Lookalike-Filter berücksichtigen mehr als 50 Faktoren, einschließlich Lead-Attribute, E-Mail-Aktivität, Web-Aktivität und Interaktion.

Klicken Sie **[!UICONTROL Einschränkung hinzufügen]**, um Erfolgskriterien für Mitglieder des/der ausgewählten Programms/Programme auszuwählen.

Klicken Sie auf das Symbol **+** , um mehrere Programme/Smart-Listen zu einem Filter hinzuzufügen.

![Bild 5](assets/predictive-filters-5.png)

## Zu beachtende Punkte {#things-to-note}

* Sie können auf eine Smart-Kampagne prädiktive Filter anwenden, selbst wenn das übergeordnete Programm erstellt wird, bevor prädiktive Filter aktiviert werden.
* Prädiktive Filter sind für Trigger-Kampagnen nicht verfügbar.
* Das Klonen oder Verschieben von Kampagnen mit prädiktiven Filtern wird nicht unterstützt.
* Sie können bis zu 5 prädiktive Filter in einer Smart-Liste verwenden.
* Wenn Marketo Engage bei der Auswertung prädiktiver Filter einen Fehler auftritt, wird die Kampagnenausführung automatisch abgebrochen und eine Benachrichtigung an das Marketo-Benachrichtigungszentrum gesendet.
* Prädiktive Filter haben derzeit eine Eingabegrenze von 1 Million qualifizierter Personen.
* Sie können bis zu 50 aktive Programme mit prädiktiven Filtern haben.
