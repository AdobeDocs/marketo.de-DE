---
unique-page-id: 2951259
description: Glossar "Benutzerdefinierter Feldtyp"- Marketing-Dokumente - Produktdokumentation
title: Glossar "Benutzerdefinierter Feldtyp"
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---


# Glossar für benutzerdefinierten Feldtyp {#custom-field-type-glossary}

Wenn Sie ein benutzerdefiniertes Feld in Marketing erstellen, haben Sie eine Liste von Typen zur Auswahl.

>[!PREREQUISITES]
>
>[Benutzerdefiniertes Feld in Marketing erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Abhängig vom Feldtyp unterscheiden sich Filter/Trigger [Operatoren](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md).

>[!NOTE]
>
>Die meisten Felder können nicht bei der Anzahl der Zeichen, sondern bei der Anzahl der Byte aussteigen. Daher können wir für jedes Feld keine endgültige Zeichenbeschränkung festlegen. Die Ausnahme ist **String**, was bei 255 Zeichen ausfällt.

## Boolean {#boolean}

**Beispielname:** Ist Kunde - Kennzeichnen Sie Ihre Mitarbeiter als Kunden

**Beispielwerte:** True (aktiviert) / False (deaktiviert)

**Operatoren**: Keines

## Währung {#currency}

**Beispielname:** Budget - Wert für eine Firma speichern

**Beispielwerte:** 100

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Datum {#date}

**Beispielname:** Verlängerungsdatum - Speichern Sie die Verlängerungsdaten Ihrer Kunden

**Beispielwerte:19.** 8.14

**Operatoren**: ist, nicht dazwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitraum, nachdem, bevor, am oder danach, am oder vorher, leer ist, nicht leer ist

## Datum {#datetime}

**Beispielname:** Erstellungsdatum - Speichern Sie das Datum und die Uhrzeit, zu der eine Person erstellt wurde

**Beispielwerte:19.** 8.14 2.00

**Operatoren**: ist, nicht dazwischen, in der Vergangenheit, in der Vergangenheit, in Zukunft, nachdem, im Zeitraum, nachdem, bevor, am oder danach, am oder vorher, leer ist, nicht leer ist

## Email {#email}

**Beispielname:** Alternative E-Mail - Behalten Sie eine alternative E-Mail-Adresse für Ihre Mitarbeiter bei (E-Mails können nicht tatsächlich an dieses Feld gesendet werden, wie z. B. das Standardfeld für die E-Mail-Adresse, das ist eine spezielle Adresse)

**Beispielwerte:** name@company.com

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## Float {#float}

**Beispielname:Durchschnittlicher** Grade-Punkt-Durchschnitt - Beibehalten des Grade-Punktdurchschnitts einer Person oder eines anderen numerischen Werts mit Dezimalstellen

**Beispielwerte:** 2.47

**Operatoren**: dazwischen, größer als, kleiner als zumindest höchstens leer ist, nicht leer ist

## Formel {#formula}

**Beispielname:** Salutationen - verwenden Sie dieses spezielle Feld in einer  [Lösung, um die richtige ](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) geschlechtsspezifische Begrüßung zu erhalten

**Beispielwerte:verknüpfte Lösung** überprüfen

## Integer {#integer}

**Beispielname:** Anzahl der Mitarbeiter - Wert einer Zahl ohne Dezimalstellen speichern

**Beispielwerte:** 600

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Prozent {#percent}

**Beispielname:** Wahrscheinlich kaufen - Einen Prozentwert speichern (möglicherweise auf der CRM-Seite berechnet)

**Beispielwerte:** 85 %

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Telefon {#phone}

**Beispielname:** Alternatives Telefon - Speichern Sie eine zusätzliche Telefonnummer für Ihre Mitarbeiter

**Beispielwert:** 650-555-5555

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## Ergebnis {#score}

**Beispielname:** Verhaltensbasierte Bewertung/demografische Bewertung - Erstellen Sie mehrere Ergebnisfelder, um verschiedene Attribute nachzuverfolgen.

**Beispielwert:** 14

**Operatoren**: ist, ist nicht, zwischen, größer als, kleiner, als zumindest höchstens leer ist, ist nicht leer

## Zeichenfolge {#string}

**Beispielname:** Mittlerer Name - zusätzliches Textattribut speichern

**Beispielwert:** Rose

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## Textbereich {#text-area}

**Beispielname:** Kommentare - Fügen Sie ein Kommentarfeld zu Ihren Formularen hinzu, um die mehrzeilige Texteingabe zuzulassen

**Beispielwert:** Dieser Artikel ist fantastisch!

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty

## URL {#url}

**Beispielname:** Blog - Erstellen Sie ein Feld, in dem persönliche Blog-URLs gespeichert werden

**Beispielwert:** www.myblog.com

**Operatoren**: is, is not, Beginn with, not Beginns with, contains, not contains, is empty, is not empty
