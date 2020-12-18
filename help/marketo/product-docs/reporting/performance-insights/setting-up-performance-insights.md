---
unique-page-id: 12981145
description: Einrichten von Leistungseinschätzungen - Marketing Docs - Produktdokumentation
title: Einrichten der Leistungseinblicke
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Einrichten der Leistungseinblicke {#setting-up-performance-insights}

Gehen Sie wie folgt vor, um MPI einzurichten.

## Opportunity Setup {#opportunity-setup}

1. Klicken Sie auf **Admin**.

   ![](assets/admin.png)

1. Klicken Sie auf **Revenue Cycle Analytics**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Wenn Sie kein RCA haben, müssen Sie für Schritt 2 **Programm-Analyse** auswählen.

1. Klicken Sie unter Zuordnung auf **Bearbeiten**.

   ![](assets/three-1.png)

1. Zuordnungseinstellungen werden angezeigt.

   ![](assets/four-2.png)

   Wenn die Zuordnung explizit ist, stellen Sie sicher, dass die Kontaktrolle &quot;Chancen&quot;ausgefüllt wurde (entweder über den Endpunkt &quot;Chancen-Rolle&quot;oder über CRM-Integration).

   Wenn die Zuordnung implizit ist, stellen Sie sicher, dass das Feld Firma auf dem Interessenten/Kontakt mit dem Kontonamen der Gelegenheit identisch ist.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass alle Möglichkeiten die entsprechenden Felder enthalten:
   >
   >    
   >    
   >    * Opportunity Amount
   >    * Ist geschlossen
   >    * Ist gewonnen
   >    * Erstellungsdatum (in Ihrem Fall möglicherweise nicht festgelegt)
   >    * Datum geschlossen (in Ihrem Fall nicht festgelegt)
   >    * Opportunity-Typ


## Programm-Setup {#program-setup}

Aktualisieren Sie die Programm-Kosten für mindestens 12 Monate. Sie können dies manuell oder mithilfe der Programm-API tun. In diesem Beispiel machen wir es manuell.

1. Klicken Sie auf **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Suchen und wählen Sie Ihr Programm aus.

   ![](assets/select-program.png)

1. Klicken Sie auf die Registerkarte **Setup**.

   ![](assets/setup-tab.png)

1. Ziehen Sie **Period Cost** auf die Arbeitsfläche.

   ![](assets/period-cost.png)

1. Legen Sie den Programm-Monat vor mindestens 12 Monaten fest und klicken Sie auf **OK**.

   ![](assets/set-period.png)

1. Legen Sie die Zeitraumkosten fest und klicken Sie auf **Speichern**.

   ![](assets/set-cost.png)

Überprüfen Sie anschließend das Analyseverhalten, um anzugeben, ob ein bestimmter Kanal in die Analyse einbezogen werden soll. Legen Sie das Analytics-Verhalten fest (Normal, Einschließen, Operativ).

1. Klicken Sie auf **Admin**.

   ![](assets/admin.png)

1. Klicken Sie auf **Tags**.

   ![](assets/tags.png)

1. Klicken Sie auf **+**, um die Liste des Kanals zu erweitern.

   ![](assets/channel.png)

1. Klicken Sie mit der Dublette auf den gewünschten Kanal.

   ![](assets/channel-click.png)

1. Klicken Sie auf die Dropdownliste **Analytics-Verhalten** und wählen Sie das gewünschte Verhalten aus.

   ![](assets/edit-channel.png)

1. Legen Sie die Erfolgskriterien fest.

   ![](assets/success.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/save.png)

## Verbinden Sie das Programm mit der Person {#tie-the-program-to-the-person}

1. Stellen Sie sicher, dass für jede Person in Ihrer Datenbank Akquise-Programm und Akquise-Datum festgelegt wurden, damit die Zuordnung von First Touch funktioniert.
1. Stellen Sie sicher, dass Ihre Programm Erfolgsstatus für Ihre Mitarbeiter festlegen.

>[!NOTE]
>
>Änderungen werden nicht sofort vorgenommen. Vor dem Inkrafttreten der Änderungen ist eine Übernachtungsperiode erforderlich.

