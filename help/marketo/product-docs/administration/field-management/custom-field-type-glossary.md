---
unique-page-id: 2951259
description: Glossar "Benutzerdefinierter Feldtyp"- Marketing-Dokumente - Produktdokumentation
title: Glossar "Benutzerdefinierter Feldtyp"
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# Glossar &quot;Benutzerdefinierter Feldtyp&quot; {#custom-field-type-glossary}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Wenn Sie ein benutzerdefiniertes Feld in Marketing erstellen, haben Sie eine Liste von Typen zur Auswahl.

>[!NOTE]
>
>**Voraussetzungen**
>
>* [Benutzerdefiniertes Feld in Marketing erstellen](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>Je nach Feldtyp unterscheiden sich die Filter-/Auslöser- [Operatoren](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) .

>[!NOTE]
>
>Die meisten Felder können nicht bei der Anzahl der Zeichen, sondern bei der Anzahl der Byte aussteigen. Daher können wir für jedes Feld keine endgültige Zeichenbeschränkung festlegen. Die Ausnahme ist **String**, der mit 255 Zeichen gefüllt wird.

## Boolesch {#boolean}

**Beispielname:** Ist Kunde - Kennzeichnen Sie Ihre Mitarbeiter als Kunden

**Beispielwerte:** True (aktiviert) / False (deaktiviert)

**Operatoren**: Keines

## Währung {#currency}

**Beispielname:** Budget - Wert für das Budget einer Firma speichern

**Beispielwerte:** 100

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Datum {#date}

**Beispielname:** Verlängerungsdatum - Speichern Sie die Verlängerungsdaten Ihrer Kunden

**Beispielwerte:** 19.08.14

**Operatoren**: ist, nicht dazwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitraum, nachdem, bevor, am oder danach, am oder vorher, leer ist, nicht leer ist

## Zeitraum {#datetime}

**Beispielname:** Erstellungsdatum - Speichern Sie das Datum und die Uhrzeit, zu der eine Person erstellt wurde.

**Beispielwerte:** 19.08.14 2:00

**Operatoren**: ist, nicht dazwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitraum, nachdem, bevor, am oder danach, am oder vorher, leer ist, nicht leer ist

## Email {#email}

**Beispielname:** Alternative E-Mail - Behalten Sie eine alternative E-Mail-Adresse für Ihre Mitarbeiter bei (E-Mails können nicht tatsächlich an dieses Feld gesendet werden, wie z. B. das Feld für die Standard-E-Mail-Adresse, das Feld ist etwas Besonderes)

**Beispielwerte:** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## Float {#float}

**Beispielname:** Durchschnittlicher Gradpunkt: Beibehalten des Gradungspunktdurchschnitts einer Person oder eines anderen numerischen Werts mit Dezimalstellen

**Beispielwerte:** 2,47

**Operatoren**: dazwischen, größer als, kleiner als zumindest höchstens leer ist, nicht leer ist

## Formel {#formula}

**Beispielname:** Ansprachen - verwenden Sie diesen speziellen Bereich in einer [Lösung, um die richtige](create-and-use-a-concatenated-string-formula-field.md) , geschlechtsspezifische Begrüßung zu erhalten

**Beispielwerte:** die verknüpfte Lösung überprüfen

## Integer {#integer}

**Beispielname:** Anzahl der Mitarbeiter - Speichern Sie einen Zahlenwert, für den keine Dezimalstellen erforderlich sind

**Beispielwerte:** 600

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Prozent {#percent}

**Beispielname:** Wahrscheinlich zu kaufen - Speichern Sie einen Prozentwert (berechnet auf der CRM-Seite)

**Beispielwerte:** 85%

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Telefon {#phone}

**Beispielname:** Alternative Telefonnummer - Speichern Sie eine zusätzliche Telefonnummer für Ihre Mitarbeiter

**Beispielwert:** 650-555-5555

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## Ergebnis {#score}

**Beispielname:** Verhaltensbasierte Bewertung/demografische Bewertung - Erstellen Sie mehrere Ergebnisfelder, um unterschiedliche Attribute nachzuverfolgen.

**Beispielwert:** 14

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Zeichenfolge {#string}

**Beispielname:** Mittlerer Name - Speichern eines zusätzlichen Textattributs

**Beispielwert:** Rose

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## Textbereich {#text-area}

**Beispielname:** Kommentare - Fügen Sie Ihren Formularen ein Kommentarfeld hinzu, um die mehrzeilige Texteingabe zuzulassen

**Beispielwert:** Dieser Artikel ist fantastisch!

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## URL {#url}

**Beispielname:** Blog - Erstellen Sie ein Feld, um persönliche Blog-URLs zu speichern

**Beispielwert:** www.myblog.com

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty
