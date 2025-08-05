---
unique-page-id: 2951259
description: Glossar für benutzerdefinierten Feldtyp - Marketo-Dokumente - Produktdokumentation
title: Glossar für benutzerdefinierten Feldtyp
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 2%

---

# Glossar für benutzerdefinierten Feldtyp {#custom-field-type-glossary}

Wenn Sie ein benutzerdefiniertes Feld in Marketo erstellen, können Sie aus einer Liste von Typen auswählen.

>[!PREREQUISITES]
>
>[Erstellen eines benutzerdefinierten Felds in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Je nach Feldtyp sind Filter/Trigger [Operatoren](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) unterschiedlich.

>[!NOTE]
>
>Die meisten Felder überschreiten nicht die maximale Anzahl an Zeichen, sondern die Anzahl an Bytes. Aus diesem Grund können wir keine endgültige Zeichenbeschränkung für jedes Feld angeben. Die Ausnahme ist **String**, der maximal 255 Zeichen lang ist.

## Boolesch {#boolean}

**Beispielname:** Ist Kunde - Markieren Sie Ihre Mitarbeiter als Kunden

**Beispielwerte:** true (aktiviert) / false (deaktiviert)

**Operatoren**: Keine

## Währung {#currency}

**Beispielname:** Budget - Speichern eines Zahlenwerts für das Budget einer Firma

**Beispielwerte:** 100

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner als, mindestens, ist leer, ist nicht leer

## Datum {#date}

**Beispielname:** Verlängerungsdatum - Speichern Sie die Verlängerungsdaten Ihrer Kunden

**Beispielwerte:** 8/19/14

**Operatoren**: ist, ist nicht, zwischen, in der Vergangenheit, in der Vergangenheit vor, in der Zukunft, in der Zukunft nach, im Zeitrahmen, nach, vor, am oder nach, an oder vor, ist leer, ist nicht leer

## Datum/Uhrzeit {#datetime}

**Beispielname:** Erstellungsdatum - Speichern Sie Datum und Uhrzeit der Erstellung einer Person

**Beispielwerte:** 8/19/14 2:00

**Operatoren**: ist, ist nicht, zwischen, in der Vergangenheit, in der Vergangenheit vor, in der Zukunft, in der Zukunft nach, im Zeitrahmen, nach, vor, am oder nach, an oder vor, ist leer, ist nicht leer

## E-Mail {#email}

**Beispielname:** Alternative E-Mail - Verwenden Sie eine alternative E-Mail-Adresse für Ihre Mitarbeiter (Sie können tatsächlich keine E-Mails an dieses Feld senden, wie das Feld Standard-E-Mail-Adresse, das speziell ist)

**Beispielwerte:** <name@company.com>

**Operatoren**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## Gleitkomma {#float}

**Beispielname:** Notendurchschnitt - Notendurchschnitt einer Person oder ein anderer numerischer Wert mit Dezimalstellen beibehalten

**Beispielwerte:** 2.47

**Operatoren**: zwischen, größer als, kleiner als, mindestens, ist leer, ist nicht leer

## Formel {#formula}

**Beispielname:** Anrede - Verwenden Sie dieses spezielle Feld in einer [Lösung, um die richtige Anrede basierend ](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) Geschlecht zu erhalten

**Beispielwerte:** Überprüfen der verknüpften Lösung

## Ganzzahl {#integer}

**Beispielname:** Anzahl der Mitarbeiter - Speichern Sie einen Zahlenwert, für den keine Dezimalstellen erforderlich sind

**Beispielwerte:** 600

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner als, mindestens, ist leer, ist nicht leer

## Prozent {#percent}

**Beispielname:** Kaufwahrscheinlich - Speichern eines Prozentwerts (möglicherweise auf CRM-Seite berechnet)

**Beispielwerte:** 85%

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner als, mindestens, ist leer, ist nicht leer

## Telefon {#phone}

**Beispielname:** Alternative Telefonnummer - Speichern Sie eine zusätzliche Telefonnummer für Ihre Mitarbeiter

**Beispielwert:** 650-555-5555

**Operatoren**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## Ergebnis {#score}

**Beispielname:** Verhaltensbewertung/Demografischer Wert - Erstellen Sie mehrere Bewertungsfelder, um verschiedene Attribute zu verfolgen

**Beispielwert:** 14

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner als, mindestens, ist leer, ist nicht leer

## String {#string}

**Beispielname:** Zweiter Vorname - Speichern eines zusätzlichen Textattributs

**Beispielwert:** Rose

**Operatoren**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## Textbereich {#text-area}

**Beispielname:** Kommentare - Fügen Sie Ihren Formularen ein Kommentarfeld hinzu, um die mehrzeilige Texteingabe zu ermöglichen

**Beispielwert:** Dieser Artikel ist fantastisch!

**Operatoren**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## URL {#url}

**Beispielname:** Blog - Erstellen eines Felds zum Speichern von Personen-Blog-URLs

**Beispielwert:** &lt;www.myblog.com>

**Operatoren**: is, is not, starts with, not starts with, contains, not contains, is empty, is not empty
