---
unique-page-id: 557339
description: Suchen und Zusammenführen doppelter Personen - Marketo-Dokumente - Produktdokumentation
title: Duplizierte Personen suchen und zusammenführen
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Duplizierte Personen suchen und zusammenführen {#find-and-merge-duplicate-people}

Marketo Engage dedupliziert automatisch, wenn neue Benutzer in das System eintreten. Ihr CRM-System kann jedoch anfangs über Duplikate gesendet worden sein. So werden sie zusammengeführt.

>[!CAUTION]
>
>Die Zusammenführung von Personen ist dauerhaft, es gibt keine &quot;Rückgängig&quot;-Option.

>[!PREREQUISITES]
>
>Das Suchen und Zusammenführen von Duplikaten erfordert die Verwendung von [integrierten/systemspezifischen Smart-Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo wird das Duplizieren für eine Salesforce- oder Microsoft Dynamics-Synchronisation nicht automatisch deaktivieren oder wenn Sie Personen manuell eingeben.

## Duplikate suchen {#find-duplicates}

1. Wechseln Sie zum Bereich **[!UICONTROL Datenbank]** .

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >Die Zusammenführung von Personen in Marketo funktioniert möglicherweise nicht, wenn Sie ein Salesforce-Personenkonto verwenden. Führen Sie die Datensätze nach Möglichkeit in Salesforce zusammen.

1. Wählen Sie die Liste **[!UICONTROL Mögliche Duplikate]** System-Smart-Liste aus und klicken Sie auf die Registerkarte **[!UICONTROL Personen]** .

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >Sie können auch [Duplizierte Personen mit benutzerdefinierter Logik finden](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## Personen manuell zusammenführen {#merge-people-manually}

>[!CAUTION]
>
>Wenn beim Zusammenführen von Personen die verlierende Person über ein benutzerdefiniertes Marketo-Objekt verfügt, wird es _nicht_ erneut mit der Gewinnerperson verknüpft. Überlagern Sie das benutzerdefinierte Objekt erneut, bevor Sie die Zusammenführung durchführen.

1. Wählen Sie die Duplikate aus, indem Sie die Strg-/Befehlstaste gedrückt halten und auf klicken und dann auf **[!UICONTROL Personen zusammenführen]** klicken.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Es können zwei oder mehr Duplikate für dieselbe Person vorhanden sein. Wählen Sie diese alle gleichzeitig aus.

1. Sie sehen die Werte zwischen den Datensätzen, die _nicht_ entsprechen. Wählen Sie für jedes Feld den Wert aus, den Sie beibehalten möchten. Klicken Sie abschließend auf **[!UICONTROL Zusammenführen]** . Wenn Sie keinen der Werte wünschen, können Sie **[!UICONTROL Benutzerdefiniert]** aktivieren und einen Wert Ihrer Wahl eingeben.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >Beim manuellen Zusammenführen von Personen wird die erste ausgewählte Person der &quot;Gewinner&quot;sein. Wenn Sie also auf der Registerkarte Personen die Datensatz-IDs 198 und 199 zusammenführen und zufällig zuerst auf 199 klicken, wird 199 die Datensatz-ID der zusammengeführten Personen sein. Dies gilt auch, wenn mehr als zwei Datensätze zusammengeführt werden.

   >[!TIP]
   >
   >Das Zusammenführen ist besser als das Löschen. Sie sparen alle Verläufe (Seitenbesuche, Link-Klicks, E-Mail-Öffnungen, Formulare usw.).

## Wirkung in Salesforce {#effect-in-salesforce}

Wenn Sie über eine Salesforce-Integration verfügen, gibt es einige Hinweise zu den Auswirkungen der Zusammenführung von Leads in Salesforce.

* Beim Zusammenführen von Leads oder nur Kontakten werden diese gemäß den normalen Salesforce-Regeln zusammengeführt.
* Beim Zusammenführen von Leads und Kontakten werden alle Leads gemäß den normalen Salesforce-Regeln in Kontakte umgewandelt.

Weitere Informationen zum Salesforce-Verhalten beim Zusammenführen von Leads oder Kontakten finden Sie in den folgenden Salesforce-Dokumenten:

* [Zusammenführen doppelter Leads](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US){target="_blank"}
* [Zusammenführen doppelter Kontakte](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US){target="_blank"}

## Massenzusammenführung {#bulk-merging}

Wenn Sie zu viele Duplikate zum manuellen Zusammenführen haben, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer), um Ihre Optionen zu besprechen.
