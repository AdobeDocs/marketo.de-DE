---
unique-page-id: 2951259
description: Glossar zu benutzerdefinierten Feldtypen - Marketo-Dokumente - Produktdokumentation
title: Glossar zum benutzerdefinierten Feldtyp
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Glossar zum benutzerdefinierten Feldtyp {#custom-field-type-glossary}

Wenn Sie ein benutzerdefiniertes Feld in Marketo erstellen, haben Sie eine Liste von Typen zur Auswahl.

>[!PREREQUISITES]
>
>[Benutzerdefiniertes Feld in Marketo erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Abhängig vom Feldtyp, Filter/Trigger [Operatoren](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) wird anders sein.

>[!NOTE]
>
>Die meisten Felder überschreiten nicht die maximale Zeichenanzahl, sondern die maximale Byte-Zeichenanzahl. Daher können wir für jedes Feld keine endgültige Zeichenbegrenzung festlegen. Die Ausnahme ist **Zeichenfolge**, der bei 255 Zeichen maximal zulässig ist.

## Boolesch {#boolean}

**Beispielname:** Is Customer - Kennzeichnen Ihrer Personen als Kunden

**Beispielwerte:** True (aktiviert) / False (deaktiviert)

**Benutzer**: Keines

## Währung {#currency}

**Beispielname:** Budget - Store einen Zahlenwert für das Budget eines Unternehmens

**Beispielwerte:** 100

**Benutzer**: ist, nicht zwischen, größer, kleiner als, zumindest höchstens leer ist, nicht leer ist

## Datum {#date}

**Beispielname:** Verlängerungsdatum - Speichern Sie die Verlängerungsdaten Ihrer Kunden

**Beispielwerte:** 19.08.14

**Benutzer**: ist, ist nicht zwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitrahmen, nachdem, bevor, an oder danach, an oder davor, leer ist, nicht leer ist

## Datum/Uhrzeit {#datetime}

**Beispielname:** Erstellungsdatum - Speichern Sie Datum und Uhrzeit der Erstellung einer Person.

**Beispielwerte:** 19.08.14 2:00

**Benutzer**: ist, ist nicht zwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitrahmen, nachdem, bevor, an oder danach, an oder davor, leer ist, nicht leer ist

## E-Mail {#email}

**Beispielname:** Alternative E-Mail - Behalten Sie eine alternative E-Mail-Adresse für Ihre Personen bei (E-Mails können nicht tatsächlich an dieses Feld gesendet werden, wie im Standard-Feld für die E-Mail-Adresse, da diese speziell ist).

**Beispielwerte:** name@company.com

**Benutzer**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## Gleitkomma {#float}

**Beispielname:** Durchschnittswert des Punkts der Bewertung - Behalten Sie den Durchschnittswert des Punkts einer Person oder einen anderen numerischen Wert mit Dezimalstellen bei.

**Beispielwerte:** 2,47

**Benutzer**: zwischen, größer als, kleiner als, zumindest höchstens leer ist, nicht leer ist

## Formel {#formula}

**Beispielname:** Lösungen - verwenden Sie dieses spezielle Feld in einer [Lösung, um die richtige Anrede zu erhalten](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) auf der Grundlage des Geschlechts

**Beispielwerte:** die verknüpfte Lösung überprüfen

## Ganze Zahl {#integer}

**Beispielname:** Anzahl der Mitarbeiter - Speichern Sie einen Zahlenwert, der keine Dezimalstellen erfordert

**Beispielwerte:** 600

**Benutzer**: ist, nicht zwischen, größer, kleiner als, zumindest höchstens leer ist, nicht leer ist

## Prozent {#percent}

**Beispielname:** Wahrscheinlich zu kaufen - Speichern Sie einen Prozentwert (möglicherweise auf CRM-Seite berechnet).

**Beispielwerte:** 85 %

**Benutzer**: ist, nicht zwischen, größer, kleiner als, zumindest höchstens leer ist, nicht leer ist

## Telefon {#phone}

**Beispielname:** Alternatives Telefon - Speichern Sie eine zusätzliche Telefonnummer für Ihre Personen.

**Beispielwert:** 650-555-5555

**Benutzer**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## Bewertung {#score}

**Beispielname:** Verhaltensbewertung/demografische Punktzahl - Erstellen Sie mehrere Punktfelder, um verschiedene Attribute zu verfolgen.

**Beispielwert:** 14

**Benutzer**: ist, nicht zwischen, größer, kleiner als, zumindest höchstens leer ist, nicht leer ist

## Zeichenfolge {#string}

**Beispielname:** Mittlerer Name: Speichern Sie ein zusätzliches Textattribut

**Beispielwert:** Rose

**Benutzer**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## Textbereich {#text-area}

**Beispielname:** Kommentare - Fügen Sie Ihren Formularen ein Kommentarfeld hinzu, um die mehrzeilige Texteingabe zu ermöglichen

**Beispielwert:** Dieser Artikel ist fantastisch!

**Benutzer**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## URL {#url}

**Beispielname:** Blog - Erstellen eines Felds zum Speichern von Personen-Blog-URLs

**Beispielwert:** www.myblog.com

**Benutzer**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty
