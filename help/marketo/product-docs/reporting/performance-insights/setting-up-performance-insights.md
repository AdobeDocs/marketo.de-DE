---
unique-page-id: 12981145
description: Einrichten von Performance Insights - Marketo-Dokumente - Produktdokumentation
title: Einrichten von Performance Insights
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# Einrichten von [!UICONTROL Performance Insights] {#setting-up-performance-insights}

Gehen Sie wie folgt vor, um MPI einzurichten.

## Opportunity-Setup {#opportunity-setup}

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicken Sie **[!UICONTROL Umsatzzyklusanalyse]**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Wenn Sie keine RCA haben, müssen Sie für Schritt 2 **[!UICONTROL Programmanalyse]** auswählen.

1. Klicken Sie unter Attribution auf **[!UICONTROL Bearbeiten]**.

   ![](assets/three-1.png)

1. Attributionseinstellungen werden angezeigt.

   ![](assets/four-2.png)

   Wenn die Attribution explizit ist, stellen Sie sicher, dass die Rolle des Opportunity-Kontakts ausgefüllt wurde (entweder über den Opportunity-Rollenendpunkt oder über die CRM-Integration).

   Wenn die Attribution implizit ist, stellen Sie sicher, dass das Unternehmensfeld auf dem Lead/Kontakt mit dem Kontonamen der Opportunity übereinstimmt.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass bei allen Opportunitys die entsprechenden Felder ausgefüllt sind:
   >
   >* [!UICONTROL Opportunity-Betrag]
   >* [!UICONTROL Ist geschlossen]
   >* [!UICONTROL Ist gewonnen]
   >* [!UICONTROL Erstellungsdatum] (kann in Ihrem Fall nicht festgelegt werden)
   >* [!UICONTROL Abschlussdatum] (kann in Ihrem Fall nicht festgelegt werden)
   >* [!UICONTROL Opportunity-Typ]

## Programm-Installation {#program-setup}

Aktualisieren Sie die Programmkosten für mindestens 12 Monate. Sie können dies manuell oder mithilfe der Programm-API tun. In diesem Beispiel machen wir es manuell.

1. Klicken Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/ma.png)

1. Suchen und wählen Sie Ihr Programm aus.

   ![](assets/select-program.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Setup“.

   ![](assets/setup-tab.png)

1. Ziehen Sie **[!UICONTROL Periodenkosten]** auf die Arbeitsfläche.

   ![](assets/period-cost.png)

1. Legen Sie den Programmmonat auf mindestens 12 Monate fest und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/set-period.png)

1. Legen Sie die Periodenkosten fest und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/set-cost.png)

Überprüfen Sie anschließend das Analytics-Verhalten, um anzugeben, ob ein bestimmter Kanal in Analytics einbezogen werden soll. Legen Sie das Analytics-Verhalten fest (normal, einschließlich, betriebsbereit).

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicken Sie auf **[!UICONTROL Tags]**.

   ![](assets/tags.png)

1. Klicken Sie auf **+**, um die Kanalliste zu erweitern.

   ![](assets/channel.png)

1. Doppelklicken Sie auf den gewünschten Kanal.

   ![](assets/channel-click.png)

1. Klicken Sie auf die **[!UICONTROL Analytics-Verhalten]** und wählen Sie das gewünschte Verhalten aus.

   ![](assets/edit-channel.png)

1. Festlegen der Erfolgskriterien.

   ![](assets/success.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/save.png)

## Programm mit der Person verknüpfen {#tie-the-program-to-the-person}

1. Stellen Sie sicher, dass das Akquiseprogramm und das Akquisedatum für jede Person in Ihrer Datenbank festgelegt wurden, damit die Erstkontakt-Attribution funktioniert.
1. Stellen Sie sicher, dass Ihre Programme Erfolgsstatus für Ihre Mitarbeiter festlegen.

>[!NOTE]
>
>Vorgenommene Änderungen werden nicht sofort wirksam. Bevor Änderungen in Kraft treten, ist ein Übernachtungszeitraum erforderlich.
