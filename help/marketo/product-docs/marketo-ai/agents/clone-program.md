---
description: Das Klonprogramm dupliziert ein vorhandenes Marketo-Programm in einen neuen Ordner mit einem neuen Namen, wobei seine Struktur erhalten bleibt, während Sie die neue Kampagne anpassen können.
title: Programm klonen
badge: Beta
hide: true
source-git-commit: 69749951d0397a837bee77d16baddc3342f68ec2
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 1%

---

# Programm klonen {#clone-program}

Der Agent „Programm klonen“ kopiert ein Arbeitsprogramm, einschließlich der intelligenten Kampagnen, Flussschritte, E-Mail-Assets und der Konfiguration, an einen neuen Speicherort in Ihrer Marketo-Umgebung.

>[!PREREQUISITES]
>
>* Um diese Funktion nutzen zu können, müssen Sie zunächst den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).
>
>* Sie müssen über die Berechtigung zum Erstellen von Programmen im Zielordner verfügen.
>
>* Das Quellprogramm, das Sie klonen möchten, muss bereits in Ihrer Marketo-Umgebung vorhanden sein.

>[!AVAILABILITY]
>
>Diese Funktion befindet sich in der geschlossenen Beta-Phase und wird in den nächsten Monaten schrittweise eingeführt. Wenn die Kachel „Mit KI erstellen“ auf dem Bildschirm &quot;_Marketo&quot; angezeigt wird, erfahren Sie_ wann sie für Ihr Abonnement aktiviert wurde.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in Ihrem Mein Marketo auf die Kachel **Mit KI erstellen**.

1. Geben Sie im Eingabeaufforderungsfenster Ihre Anweisungen ein. Beispiel: „Klonen Sie mein Webinar-Programm für das zweite Quartal in den Ordner für Q3-Kampagnen und nennen Sie es „Produktdemo-Webinar für das dritte Quartal“.

1. Marketo AI bestätigt das Quellprogramm, den Zielordner und den neuen Namen. Überprüfen und bestätigen.

1. Der Klon wird erstellt. Marketo AI bestätigt, wann dies geschehen ist, und teilt Ihnen mit, wo Sie es finden können.

1. Öffnen Sie das neue Programm in Marketo und aktualisieren Sie, was anders ist: E-Mail-Inhalt, Daten, Zielgruppenfilter, Token usw.

1. Führen Sie [Programm-QA](/help/marketo/product-docs/marketo-ai/agents/program-qa.md)-Agent vor der Aktivierung aus.

## Anwendungsszenarien {#use-cases}

**Vierteljährliche Kampagnenwiederverwendung**: Ein Kampagnen-Manager führt jedes Quartal dieselbe Webinar-Reihe durch. Sie bitten Marketo AI, das Webinar-Programm des letzten Quartals unter einem aktualisierten Namen in den Ordner des neuen Quartals zu klonen. Anschließend aktualisieren sie die E-Mail-Kopie, Webinar-Datumstoken und den Anmelde-Link, wodurch die Einrichtungszeit um mehrere Stunden verkürzt wird.

**Erstellen einer Vorlage aus einem bewährten Programm**: Ein Marketing-Opportunity-Spezialist klont ein leistungsstarkes Produkt-Launch-Programm in einen „Vorlagen“-Ordner, der als Ausgangspunkt für zukünftige Launches dient. Der Klon bleibt deaktiviert und wird als Referenzkopie verwendet.

**A/B-Tests nach einem neuen**: Ein Kampagnen-Manager möchte eine andere E-Mail-Kadenz testen, ohne ein laufendes Programm zu ändern. Sie klonen das aktive Programm, ändern die Warteschritte im Klon und aktivieren beide, führen sie für verschiedene Zielgruppensegmente aus, um die Ergebnisse zu vergleichen.

## Zu beachtende Punkte {#things-to-note}

* Klone Programme werden in einem deaktivierten Zustand erstellt. Es wird nichts live geschaltet, bis Sie die Smart-Kampagnen aktivieren.
* E-Mail-Assets im Klon sind Kopien, die nicht mit dem Original geteilt werden. Änderungen an den E-Mails des Klons wirken sich nicht auf das Quellprogramm aus.
* Im Quellprogramm verwendete Token werden in den Klon kopiert. Sie müssen jedoch weiterhin mit neuen Werten (Daten, URLs, Ereignisnamen) aktualisiert werden.
* Die Smart-Kampagnenfilter im Klon verweisen auf dieselben Listen und Felder wie die Original-Kampagnen. Zielgruppen-Targeting vor der Aktivierung überprüfen und aktualisieren.
* Lokale Assets, die auf andere Programme oder freigegebene Listen verweisen, werden in den Klon kopiert. Diese Verweise sollten vor der Aktivierung überprüft werden.
