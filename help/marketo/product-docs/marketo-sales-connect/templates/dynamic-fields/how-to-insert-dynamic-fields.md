---
unique-page-id: 14352592
description: Erfahren Sie, wie Sie dynamische Felder in Sales Connect-Vorlagen einfügen. Fügen Sie die Felder „Vorname“, „Firma“ und „Andere Zusammenführungsfelder“ im Vorlageneditor hinzu.
title: Einfügen dynamischer Felder
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/WwKaorfXBu5Ah9wD6pXf5U4YzlpP9MoUMg-TtDzXDRo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 4%

---

# Einfügen dynamischer Felder {#how-to-insert-dynamic-fields}

Wir ermöglichen es Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}` zu personalisieren. Mit diesen Feldern können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen, ohne sie für jeden Kontakt separat eingeben zu müssen.

>[!TIP]
>
>Die Felder „first_name“ und „company“ sind die einzigen Felder, die sowohl an [!DNL Sales Connect] als auch an [!DNL Salesforce] gerichtet sind. Wenn also in der [Web-Anwendung](https://toutapp.com/login) kein Kontakt vorhanden ist, überprüfen wir [!DNL Salesforce], ob wir einen Kontakt-/Lead-Datensatz mit einer entsprechenden E-Mail-Adresse finden können. Anschließend verwenden wir Informationen aus diesem Datensatz, um das Feld auszufüllen.

## Einfügen eines dynamischen Felds in eine Vorlage {#insert-a-dynamic-field-into-a-template}

1. Suchen **[!UICONTROL unter „Vorlagen und Kampagnen]** die Vorlage, die Sie bearbeiten möchten, und klicken Sie auf **[!UICONTROL Vorlage bearbeiten]**.

1. Klicken Sie **[!UICONTROL Dynamische Felder testen]**.

   >[!NOTE]
   >
   >Beim Senden von E-Mails an Kontakte, die in [!DNL Sales Connect] vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese ziehen direkt aus dem Kontakt.

Wenn Sie Kontakte per E-Mail versenden, die bereits in [!DNL Salesforce] vorhanden sind, können Sie die [!DNL Salesforce] dynamischen Felder nutzen. Diese beginnen alle mit „sfdc“. Sofern Sie über eine Verbindung zu [!DNL Salesforce] verfügen, werden diese Felder direkt den Lead/Kontakt aufrufen, [!DNL Salesforce] Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie im Betrefffeld einer E-Mail ein. Achten Sie dabei darauf, dass die korrekte Formatierung gewährleistet ist.
