---
unique-page-id: 557339
description: Suchen und Zusammenführen doppelter Personen - Marketo-Dokumente - Produktdokumentation
title: Duplizierte Personen suchen und zusammenführen
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Duplizierte Personen suchen und zusammenführen {#find-and-merge-duplicate-people}

Marketo dedupliziert automatisch, wenn neue Personen in das System eintreten. Ihr CRM-System hat jedoch möglicherweise zunächst Duplikate an Marketo gesendet. So werden sie zusammengeführt.

>[!NOTE]
>
>Marketo wird das Duplizieren für eine Salesforce- oder Microsoft Dynamics-Synchronisation nicht automatisch deaktivieren oder wenn Sie Personen manuell eingeben.

>[!PREREQUISITES]
>
>Das Suchen und Zusammenführen von Duplikaten erfordert die Verwendung von [integrierte/System-Smart-Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md).

## Duplikate suchen {#find-duplicates}

1. Navigieren Sie zu **Datenbank** Bereich.

   ![](assets/db.png)

   >[!CAUTION]
   >
   >Die Zusammenführung von Personen in Marketo funktioniert möglicherweise nicht, wenn Sie ein Salesforce-Personenkonto verwenden. Führen Sie die Datensätze nach Möglichkeit in Salesforce zusammen.

1. Wählen Sie die **Mögliche Duplikate** Smart-Liste des Systems und klicken Sie auf **Personen** Registerkarte.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Sie können auch [Duplizierte Personen mit benutzerdefinierter Logik suchen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md).

## Personen manuell zusammenführen {#merge-people-manually}

>[!CAUTION]
>
>Wenn beim Zusammenführen von Personen die untergeordnete Person über ein benutzerdefiniertes Marketo-Objekt verfügt, wird **not** erneut mit der Gewinnerperson in Verbindung gebracht werden. Überlagern Sie das benutzerdefinierte Objekt erneut, bevor Sie die Zusammenführung durchführen.

1. Wählen Sie die Duplikate aus, indem Sie die Strg-/Befehlstaste gedrückt halten und auf klicken. Klicken Sie dann auf **Personen zusammenführen**.

   ![](assets/three.png)

   >[!TIP]
   >
   >Es können zwei oder mehr Duplikate für dieselbe Person vorhanden sein. Wählen Sie alle Duplikate gleichzeitig aus.

1. Sie sehen die Werte zwischen den Datensätzen, die _don&#39;t_ übereinstimmen. Wählen Sie für jedes Feld den Wert aus, den Sie beibehalten möchten. Klicken **Zusammenführen** wann geschehen. Wenn Sie keinen der Werte wünschen, können Sie **Benutzerdefiniert** und geben Sie einen Wert Ihrer Wahl ein.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Beim manuellen Zusammenführen von Personen wird die erste ausgewählte Person der &quot;Gewinner&quot;sein. Wenn Sie also auf der Registerkarte Personen die Datensatz-IDs 198 und 199 zusammenführen und zufällig zuerst auf 199 klicken, wird 199 die Datensatz-ID der zusammengeführten Personen sein. Dies gilt auch, wenn mehr als zwei Datensätze zusammengeführt werden.

   >[!TIP]
   >
   >Das Zusammenführen ist besser als das Löschen. Sie sparen alle Verläufe (Seitenbesuche, Link-Klicks, E-Mail-Öffnungen, Formulare usw.).

## Wirkung in Salesforce {#effect-in-salesforce}

Wenn Sie über eine Salesforce-Integration verfügen, gibt es einige Hinweise zu den Auswirkungen von &quot;Leads zusammenführen&quot;in Salesforce.

* Beim Zusammenführen von Leads oder nur Kontakten werden diese nach normalen Salesforce-Regeln zusammengeführt.
* Beim Zusammenführen von Leads und Kontakten werden alle Leads gemäß den normalen Salesforce-Regeln in Kontakte umgewandelt.

Weitere Informationen zum Salesforce-Verhalten beim Zusammenführen von Leads oder Kontakten finden Sie in den folgenden Salesforce-Dokumenten:

* [Zusammenführen doppelter Leads](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [Zusammenführen doppelter Kontakte](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Massenzusammenführung {#bulk-merging}

Wenn Sie zu viele Duplikate zum manuellen Zusammenführen haben, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer), um Ihre Optionen zu besprechen.

Wenn Sie mit einem CRM verbunden sind, werden die Datensätze dort gemäß den unten stehenden Regeln zusammengeführt.
