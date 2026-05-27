---
unique-page-id: 12981145
description: Erfahren Sie, wie Sie Performance Insights einrichten, indem Sie Opportunity-Einrichtung, Programmkosten, Analytics-Verhalten und Erfolgskriterien konfigurieren. Sicherstellen einer ordnungsgemäßen Attribution und eines ordnungsgemäßen Datenflusses für ein genaues Reporting.
title: Einrichten von Performance Insights
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
TQID: https://experienceleague.adobe.com/xH9HG3hKoUFG3428IngBYFG6n4W3k1Bd-baVI7WTMrE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: b9f06cb0-cdf7-4b83-a9d1-a701d132779b
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 331
ht-degree: 2%

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
