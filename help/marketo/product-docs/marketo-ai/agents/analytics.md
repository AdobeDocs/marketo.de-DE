---
description: Sprechen Sie mit Marketo AI über Ihre Marketo Engage-Leistungsdaten. Stellen Sie Fragen in einfacher Sprache und erhalten Sie Antworten, die in Ihrer Marketo-Umgebung basieren.
title: Analytics
badge: Beta
hide: true
source-git-commit: 69749951d0397a837bee77d16baddc3342f68ec2
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Analytics {#analytics}

Mit Analytics können Sie über Ihre Marketo-Leistungsdaten sprechen. Stellen Sie Fragen in einfacher Sprache und erhalten Sie Antworten, die in Ihrer Marketo-Umgebung basieren.

>[!PREREQUISITES]
>
>* Um diese Funktion nutzen zu können, müssen Sie zunächst den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).
>
>* Sie müssen Zugriff auf die Programme und Berichte haben, die Sie anfragen.

>[!AVAILABILITY]
>
>Diese Funktion befindet sich in der geschlossenen Beta-Phase und wird in den nächsten Monaten schrittweise eingeführt. Wenn die Kachel „Mit KI erstellen“ auf dem Bildschirm &quot;_Marketo&quot; angezeigt wird, erfahren Sie_ wann sie für Ihr Abonnement aktiviert wurde.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in Ihrem Mein Marketo auf die Kachel **Mit KI erstellen**.

1. Stellen Sie im Eingabeaufforderungsfenster eine Frage zur Leistung. Geben Sie den Zeitrahmen oder das Programm genau an, wenn Sie dies im Sinn haben.

1. Überprüfen Sie die Zusammenfassung der Marketo-KI-Rückgaben. Sie enthält Schlüsselmetriken wie Öffnungsraten, Klickraten, Konversionsraten und Lead-Zahlen, je nachdem, was Sie gefragt haben.

1. Stellen Sie Folgefragen, um bestimmte Bereiche zu untersuchen (z. B. „Welche E-Mail in diesem Programm hatte die höchste Klickrate?“ oder „Wie ist das im Vergleich zum letzten Quartal?„).

## Anwendungsszenarien {#use-cases}

**Vierteljährliche Programmüberprüfung**: Ein Manager für die Nachfragengenerierung bereitet sich auf ein Meeting zur Kampagnenüberprüfung vor. Sie fragen: „Wie haben sich meine Pflegeprogramme im 2. Quartal insgesamt entwickelt?“ Marketo AI gibt Öffnungsraten, Clickto-Open-Raten, Abmelderaten und die Anzahl der Personen/Leads zurück, die in allen Q2 Nurture-Programmen zu MQL weitergeleitet wurden, mit einer Anmerkung dazu, welche Programme den Gruppendurchschnitt übertroffen haben.

**Vergleich zweier Kampagnen**: Ein Kampagnen-Manager hat zwei Versionen einer Webinar-Einladungsserie mit unterschiedlichen Betreffzeilen ausgeführt. Sie fragen: „Wie hat sich das Webinar-Programm im April im Vergleich zum Webinar im März hinsichtlich der Registrierungsrate entwickelt?“ Marketo AI gibt die Registrierungsnummern für jede aus und hebt den Unterschied hervor, damit sie sehen können, welcher Ansatz besser funktioniert hat.

**Suche nach leistungsstarken Inhalten**: Ein Spezialist für Marketing-Opportunities möchte wissen, welche E-Mail-Assets im letzten Monat am meisten Interaktionen hervorgerufen haben. Sie fragen: „Welche E-Mails hatten im Mai die höchsten Klickraten?“ Marketo-KI gibt eine Rangfolge von E-Mail-Assets mit Klickraten zurück, damit sie identifizieren können, was bei Ihren Inhaltsentscheidungen Resonanz gefunden hat, und so in künftige Inhaltsentscheidungen einfließen können.

## Zu beachtende Punkte {#things-to-note}

* Analytics-Antworten basieren auf den Daten, die in Ihrer Marketo-Instanz verfügbar sind. Wenn ein Programm nicht verfolgt wird oder keine Metrik erfasst wird, kann Marketo AI keinen Bericht dazu erstellen.
* Sehr große Datumsbereiche oder allgemeine Fragen geben möglicherweise allgemeine Zusammenfassungen anstelle detaillierter Details zurück. Zum Beispiel: „Wie haben alle meine Programme in den letzten zwei Jahren abgeschnitten?“
* Marketo-KI kann Daten einblenden, aber basierend auf den gefundenen Elementen keine Änderungen an Ihren Programmen oder Berichten vornehmen.
* Für ein detailliertes benutzerdefiniertes Reporting mit bestimmten Filtern und Aufschlüsselungen sind die integrierten Reporting-Tools von Marketo oder eine BI-Integration möglicherweise besser geeignet.
* Die Attribution auf Multi-Touch-Kampagnen erfordert eine ordnungsgemäße Programmeinrichtung. Die Marketo-KI meldet, was verfolgt wird, und leitet keine Attribution ab, die nicht konfiguriert wurde.
