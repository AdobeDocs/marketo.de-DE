---
unique-page-id: 12981145
description: Einrichten von Leistungseinblicken - Marketo-Dokumente - Produktdokumentation
title: Einrichten von Leistungseinblicken
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 3%

---

# Einrichten von Leistungseinblicken {#setting-up-performance-insights}

Gehen Sie wie folgt vor, um MPI einzurichten.

## Einrichtung von Chancen {#opportunity-setup}

1. Klicken Sie auf **Admin**.

   ![](assets/admin.png)

1. Klicken Sie auf **Umsatzzyklusanalysen**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Wenn Sie keine RCA haben, müssen Sie für Schritt 2 die Option **Programmanalyse** auswählen.

1. Klicken Sie unter &quot;Attribution&quot;auf **Bearbeiten**.

   ![](assets/three-1.png)

1. Die Attributionseinstellungen werden angezeigt.

   ![](assets/four-2.png)

   Wenn die Attribution explizit ist, stellen Sie sicher, dass die Kontaktrolle &quot;Chancen&quot;ausgefüllt wurde (entweder über den Endpunkt &quot;Angebotsrolle&quot;oder über die CRM-Integration).

   Wenn Attribution implizit ist, stellen Sie sicher, dass das Unternehmensfeld auf dem Lead/Kontakt mit dem Kontonamen der Opportunity übereinstimmt.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass alle Möglichkeiten die entsprechenden Felder ausgefüllt haben:
   >
   >* Opportunity-Betrag
   >* Ist geschlossen
   >* Ist gewonnen
   >* Erstellungsdatum (in Ihrem Fall kann dies nicht festgelegt werden)
   >* Geschlossenes Datum (in Ihrem Fall kann dies nicht festgelegt werden)
   >* Opportunity-Typ

## Programm-Installation {#program-setup}

Aktualisieren Sie die Programmkosten für mindestens 12 Monate. Sie können dies manuell oder mithilfe der Programm-API tun. In diesem Beispiel machen wir es manuell.

1. Klicken Sie auf **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie Ihr Programm aus.

   ![](assets/select-program.png)

1. Klicken Sie auf die Registerkarte **Setup**.

   ![](assets/setup-tab.png)

1. Ziehen Sie **Period Cost** auf die Arbeitsfläche.

   ![](assets/period-cost.png)

1. Legen Sie den Programmmonat vor mindestens 12 Monaten fest und klicken Sie auf **OK**.

   ![](assets/set-period.png)

1. Legen Sie die Zeitraumkosten fest und klicken Sie auf **Speichern**.

   ![](assets/set-cost.png)

Überprüfen Sie anschließend das Analytics-Verhalten, um anzugeben, ob ein bestimmter Kanal in die Analyse einbezogen werden soll. Legen Sie das Analytics-Verhalten fest (Normal, Einschließen, Operativ).

1. Klicken Sie auf **Admin**.

   ![](assets/admin.png)

1. Klicken Sie auf **Tags**.

   ![](assets/tags.png)

1. Klicken Sie auf &quot;**+**&quot;, um die Kanalliste zu erweitern.

   ![](assets/channel.png)

1. Doppelklicken Sie auf den gewünschten Kanal.

   ![](assets/channel-click.png)

1. Klicken Sie auf die Dropdownliste **Analytics-Verhalten** und wählen Sie das gewünschte Verhalten aus.

   ![](assets/edit-channel.png)

1. Festlegen der Erfolgskriterien.

   ![](assets/success.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/save.png)

## das Programm an die Person binden {#tie-the-program-to-the-person}

1. Stellen Sie sicher, dass das Akquiseprogramm und das Akquisedatum für jede Person in Ihrer Datenbank festgelegt wurden, damit die Erstkontaktzuordnung funktioniert.
1. Stellen Sie sicher, dass Ihre Programme Erfolgsstatus für Ihre Menschen festlegen.

>[!NOTE]
>
>Die vorgenommenen Änderungen sind nicht unmittelbar. Bevor Änderungen wirksam werden, ist eine Übernachtungsperiode erforderlich.
