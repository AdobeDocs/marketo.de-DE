---
unique-page-id: 2951259
description: Glossar zu benutzerdefinierten Feldtypen - Marketo-Dokumente - Produktdokumentation
title: Glossar zum benutzerdefinierten Feldtyp
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# Glossar zum benutzerdefinierten Feldtyp {#custom-field-type-glossary}

Wenn Sie ein benutzerdefiniertes Feld in Marketo erstellen, haben Sie eine Liste von Typen zur Auswahl.

>[!PREREQUISITES]
>
>[Benutzerdefiniertes Feld in Marketo erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Je nach Feldtyp unterscheiden sich der Filter/Trigger [Operatoren](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md).

>[!NOTE]
>
>Die meisten Felder überschreiten nicht die maximale Zeichenanzahl, sondern die maximale Byteanzahl. Daher können wir für jedes Feld keine endgültige Zeichenbegrenzung festlegen. Die Ausnahme ist **String**, der bei 255 Zeichen vorkommt.

## Boolesch {#boolean}

**Beispielname:** Ist Kunde - Kennzeichnen Ihrer Personen als Kunden

**Beispielwerte:** True (aktiviert) / False (deaktiviert)

**Operatoren**: Keine

## Währung {#currency}

**Beispielname:** Budget - Store a number value for a company&#39;s budget

**Beispielwerte:** 100

**Operatoren**: ist, ist nicht zwischen, größer als, kleiner als, zumindest höchstens leer, ist nicht leer.

## Datum {#date}

**Beispielname:** Verlängerungsdatum - Speichern Sie die Verlängerungsdaten Ihrer Kunden.

**Beispielwerte:** 19.8.14

**Operatoren**: ist, ist nicht dazwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitrahmen, nachdem, bevor, an oder danach, an oder davor, leer ist, nicht leer ist.

## Datum/Uhrzeit {#datetime}

**Beispielname:** Erstellungsdatum - Speichern Sie das Datum und die Uhrzeit, zu der eine Person erstellt wird

**Beispielwerte:** 19.8.14 2:00

**Operatoren**: ist, ist nicht dazwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitrahmen, nachdem, bevor, an oder danach, an oder davor, leer ist, nicht leer ist.

## E-Mail {#email}

**Beispielname:** Alternative E-Mail - Behalten Sie eine alternative E-Mail-Adresse für Ihre Personen bei (E-Mails können nicht tatsächlich an dieses Feld gesendet werden, z. B. das standardmäßige Feld für die E-Mail-Adresse; diese Adresse ist spezifisch).

**Beispielwerte:** name@company.com

**Operatoren**: ist, ist nicht, beginnt mit, beginnt nicht mit, enthält, nicht enthält, ist leer, ist nicht leer

## Gleitkomma {#float}

**Beispielname:** Durchschnittswert des Punkts der Bewertung - Behalten Sie den Durchschnittswert des Punktstands einer Person oder einen anderen numerischen Wert mit Dezimalstellen bei.

**Beispielwerte:** 2.47

**Operatoren**: zwischen, größer als, kleiner als, zumindest höchstens leer ist, nicht leer ist

## Formel {#formula}

**Beispielname:** Aufrufe - Verwenden Sie dieses spezielle Feld in einer [Lösung, um die richtige Anrede](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) basierend auf dem Geschlecht zu erhalten.

**Beispielwerte:** prüfen die verknüpfte Lösung

## Ganze Zahl {#integer}

**Beispielname:** Anzahl der Mitarbeiter - speichern Sie einen Zahlenwert, der keine Dezimalstellen erfordert

**Beispielwerte:** 600

**Operatoren**: ist, ist nicht zwischen, größer als, kleiner als, zumindest höchstens leer, ist nicht leer.

## Prozent {#percent}

**Beispielname:** Wahrscheinlich zu kaufen - einen Prozentwert speichern (möglicherweise auf CRM-Seite berechnet)

**Beispielwerte:** 85 %

**Operatoren**: ist, ist nicht zwischen, größer als, kleiner als, zumindest höchstens leer, ist nicht leer.

## Telefon {#phone}

**Beispielname:** Alternatives Telefon - Speichern Sie eine zusätzliche Telefonnummer für Ihre Personen.

**Beispielwert:** 650-555-5555

**Operatoren**: ist, ist nicht, beginnt mit, beginnt nicht mit, enthält, nicht enthält, ist leer, ist nicht leer

## Bewertung {#score}

**Beispielname:** Verhaltensbewertung/demografische Bewertung - Erstellen Sie mehrere Punktzahlfelder, um verschiedene Attribute zu verfolgen.

**Beispielwert:** 14

**Operatoren**: ist, ist nicht zwischen, größer als, kleiner als, zumindest höchstens leer, ist nicht leer.

## Zeichenfolge {#string}

**Beispielname:** Vorname - Speichern eines zusätzlichen Textattributs

**Beispielwert:** Rose

**Operatoren**: ist, ist nicht, beginnt mit, beginnt nicht mit, enthält, nicht enthält, ist leer, ist nicht leer

## Textbereich {#text-area}

**Beispielname:** Kommentare - Fügen Sie ein Kommentarfeld zu Ihren Formularen hinzu, um mehrzeiligen Texteintrag zuzulassen

**Beispielwert:** Dieser Artikel ist fantastisch!

**Operatoren**: ist, ist nicht, beginnt mit, beginnt nicht mit, enthält, nicht enthält, ist leer, ist nicht leer

## URL {#url}

**Beispielname:** Blog - Erstellen Sie ein Feld zum Speichern von Personen-Blog-URLs

**Beispielwert:** www.myblog.com

**Operatoren**: ist, ist nicht, beginnt mit, beginnt nicht mit, enthält, nicht enthält, ist leer, ist nicht leer
