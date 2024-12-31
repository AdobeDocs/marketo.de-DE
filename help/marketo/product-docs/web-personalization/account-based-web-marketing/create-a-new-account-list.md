---
unique-page-id: 4720232
description: Erstellen einer neuen Kontoliste - Marketo-Dokumente - Produktdokumentation
title: Erstellen einer neuen Kontoliste
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 8%

---

# Erstellen einer neuen Kontoliste {#create-a-new-account-list}

Erstellen Sie eine Liste mit Organisations- und Domain-Namen und laden Sie sie hoch, um diese wichtigen Konten mit personalisierten Kampagnen anzusprechen.

>[!NOTE]
>
>Dieser Artikel gilt nur für ältere Web ABM-Kunden. Wenn Sie Web ABM nach September 2016 erworben haben, führen Sie stattdessen die Schritte in [diesem Artikel](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) aus.

## Erstellen einer neuen Kontoliste {#create-a-new-account-list-1}

1. Navigieren Sie zu **Kontolisten**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Wählen Sie **Neu erstellen** aus.

   ![](assets/create-new-account-list-hand.jpg)

1. Wählen Sie **Durchsuchen** aus und laden Sie Ihre CSV-Datei hoch (stellen Sie sicher, dass die CSV-Datei die Kriterien erfüllt). Fügen Sie **Name** und &quot;**&quot;**. Klicken Sie auf **Speichern**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Was ist das Format für die CSV-Datei?**
   >
   >Stellen Sie sicher, dass die CSV-Datei des benannten Kontos die folgenden Anforderungen erfüllt:
   >
   >* Als CSV-Format gespeichert
   >* 10 MB nicht überschreiten
   >* Nur 4 Spalten mit der Überschrift Spalte A: Name, Spalte B: Domäne, Spalte C: Land, Spalte D: US-Bundesstaat.
   >* Bis zur Genehmigung hochgeladener Dateien können bis zu 2 Werktage vergehen.
   >* Sie erhalten per E-Mail eine Genehmigung, oder prüfen Sie den Dateistatus auf der Seite für benannte Konten.
   >* Die Gesamtzahl der gesammelten Datensätze/Zeilen für alle hochgeladenen Listen beginnt bei 10.000, wobei das größte Paket 100.000 umfasst.

   >[!NOTE]
   >
   >**Beispiel der CSV-Datei**
   >
   >* Zeile 1 Spalte A Wert = Organisation
   >* Zeile 1 Spalte B Wert = Domäne
   >* Zeile 1 Spalte C Wert = Land
   >* Zeile 1 Spalte D Wert = US-Bundesstaat
   >* Einer der Spaltenwerte ist obligatorisch. Durch die Angabe von Organisations- und Domain-Namen werden jedoch die Übereinstimmungsraten der Kontenliste verbessert.
   >* Land und Bundesland sind optionale Werte.
   >
   >   * Für den Ländernamen verwenden Sie den vollständigen Ländernamen oder den Abkürzungscode. Z. B. Vereinigte Staaten oder USA.
   >   * Für einen US-Bundesstaat verwenden Sie den aus zwei Buchstaben bestehenden Abkürzungscode, d. h. CA. Nur US-Bundesstaaten werden anerkannt.
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Bearbeiten einer Kontoliste {#edit-an-account-list}

Klicken Sie auf der **Kontolisten** auf das Symbol **Bearbeiten** in der Liste.

![](assets/create-new-account-list-edit.jpg)

Wählen Sie **Durchsuchen** aus und laden Sie Ihre neue CSV-Datei hoch. Diese Datei ersetzt die Originaldatei. Klicken Sie auf **Speichern**. Die neue hochgeladene Datei befindet sich im Status „Ausstehend“, bis sie vom Marketo-Support genehmigt wurde. Im Status „Ausstehend“ bleibt die Originaldatei aktiv.

![](assets/set-account-list-edit-hands.jpg)

Die CSV-Datei ersetzt die vorhandene Datei. Die vorhandene Liste bleibt aktiv, bis die Verarbeitung der neuen Datei abgeschlossen ist.

## Löschen einer benannten Kontoliste {#delete-a-named-account-list}

1. Klicken Sie auf **Seite &quot;**&quot; auf das Symbol Löschen der Liste, die Sie löschen möchten.

   ![](assets/create-new-account-list-delete.jpg)

1. Es wird eine Meldung angezeigt, die bestätigt, ob Sie die Liste löschen möchten. Klicken Sie auf **OK**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Erstellen eines Segments mithilfe einer Kontoliste](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
