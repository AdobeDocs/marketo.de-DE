---
unique-page-id: 557339
description: Duplikat People suchen und zusammenführen - Marketo Docs - Produktdokumentation
title: Duplikat-Personen suchen und zusammenführen
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Duplikat-Personen suchen und zusammenführen {#find-and-merge-duplicate-people}

Marketo entfernt automatisch Duplikat, wenn neue Personen in das System einsteigen. Ihr CRM-System hat jedoch möglicherweise zunächst Duplikat an Marketo gesendet. Hier ist, wie man sie zusammenführt.

>[!NOTE]
>
>Marketo wird nicht automatisch deduplizieren gegen eine Salesforce- oder Microsoft Dynamics-Synchronisierung, oder wenn Sie manuell eingeben.

>[!PREREQUISITES]
>
>Das Suchen und Zusammenführen von Duplikaten erfordert die Verwendung von [integrierten / System intelligenten Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md).

## Duplikat suchen {#find-duplicates}

1. Wechseln Sie zum Bereich **Datenbank**.

   ![](assets/db.png)

   >[!CAUTION]
   >
   >Das Zusammenführen von Personen in Marketo funktioniert möglicherweise nicht, wenn Sie ein Salesforce-Benutzerkonto verwenden. Bitte führen Sie die Unterlagen nach Möglichkeit in Salesforce zusammen.

1. Wählen Sie die Systemintelligente Liste **Mögliche Duplikat** und klicken Sie auf die Registerkarte **Personen**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Sie können auch [Duplikat-Personen mit benutzerdefinierter Logik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md) suchen.

## Personen manuell zusammenführen {#merge-people-manually}

>[!CAUTION]
>
>Wenn beim Zusammenführen von Personen die unterliegende Person ein benutzerdefiniertes Marketo-Objekt hat, wird **nicht** erneut der Gewinner-Person zugeordnet. Überlagern Sie das benutzerdefinierte Objekt erneut, bevor Sie die Zusammenführung durchführen.

1. Wählen Sie die Duplikat aus, indem Sie Strg/Cmd drücken und auf **Personen zusammenführen** klicken.

   ![](assets/three.png)

   >[!TIP]
   >
   >Sie können zwei oder mehr Duplikate für dieselbe Person haben - wählen Sie sie alle gleichzeitig aus.

1. Sie sehen die Werte zwischen den Datensätzen, die _nicht_ übereinstimmen. Wählen Sie den Wert aus, den Sie für die einzelnen Felder beibehalten möchten. Klicken Sie nach Abschluss des Vorgangs auf **Zusammenführen**. Wenn Sie keinen Wert wünschen, können Sie **Benutzerdefiniert** aktivieren und einen Wert Ihrer Wahl eingeben.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Beim manuellen Zusammenführen von Personen wird die erste ausgewählte Person der Gewinner sein. Auf der Registerkarte &quot;Personen&quot;, wenn Sie die Datensatz-IDs 198 und 199 zusammenführen und Sie zufällig auf 199 klicken, wird 199 die Datensatz-ID der zusammengeführten Personen. Dies gilt auch, wenn mehr als zwei Datensätze zusammengeführt werden.

   >[!TIP]
   >
   >Zusammenführen ist besser als Löschen. Sie behalten den gesamten Verlauf bei (Seitenbesuche, Link-Klicks, E-Mail-Öffnen, Ausfüllen von Formularen usw.).

## Effekt in Salesforce {#effect-in-salesforce}

Wenn Sie Salesforce-Integration haben, gibt es einige Hinweise zur Wirkung von Merge Leads in Salesforce.

* Beim Zusammenführen nur Interessenten oder nur Kontakte werden diese gemäß den normalen Salesforce-Regeln zusammengeführt.
* Beim Zusammenführen von Interessenten und Kontakten werden alle Interessenten in Kontakte konvertiert, bevor sie gemäß den normalen Salesforce-Regeln zusammengeführt werden.

Einzelheiten zum Verhalten von Salesforce beim Zusammenführen von Interessenten oder Kontakten finden Sie in den folgenden Salesforce-Dokumenten:

* [Zusammenführen von Duplikat-Interessenten](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [Zusammenführen von Duplikat-Kontakten](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Massenzusammenführung {#bulk-merging}

Wenn Sie zu viele Duplikat zum manuellen Zusammenführen haben, wenden Sie sich an Ihren Kundenbetreuer, um Ihre Optionen zu besprechen.

Super! Wenn Sie mit einem CRM verbunden sind, werden die Datensätze dort gemäß den unten stehenden Regeln zusammengeführt.
