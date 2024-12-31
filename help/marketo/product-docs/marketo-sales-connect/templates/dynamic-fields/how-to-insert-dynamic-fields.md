---
unique-page-id: 14352592
description: Einfügen dynamischer Felder - Marketo-Dokumente - Produktdokumentation
title: Einfügen dynamischer Felder
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Einfügen dynamischer Felder {#how-to-insert-dynamic-fields}

Wir ermöglichen es Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}` zu personalisieren. Mit diesen Feldern können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen, ohne sie für jeden Kontakt separat eingeben zu müssen.

>[!TIP]
>
>Die Felder „Vorname“ und „Firma“ sind die einzigen, die sowohl an Sales Connect als auch an Salesforce gerichtet sind. Wenn also in der [Web-Anwendung](https://toutapp.com/login) kein Kontakt vorhanden ist, prüfen wir in Salesforce, ob wir einen Kontakt-/Lead-Datensatz mit einer entsprechenden E-Mail-Adresse finden können. Anschließend verwenden wir Informationen aus diesem Datensatz, um das Feld auszufüllen.

## Einfügen eines dynamischen Felds in eine Vorlage {#insert-a-dynamic-field-into-a-template}

1. Suchen **unter „Vorlagen und Kampagnen** die Vorlage, die Sie bearbeiten möchten, und klicken Sie auf **Vorlage bearbeiten**.

1. Klicken Sie **Dynamische Felder testen**.

   >[!NOTE]
   >
   >Beim Senden von E-Mails an Kontakte, die in Sales Connect vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese ziehen direkt aus dem Kontakt.

Wenn Sie Kontakte per E-Mail versenden, die bereits in Salesforce vorhanden sind, können Sie die dynamischen Salesforce-Felder nutzen. Diese beginnen alle mit „sfdc“. Sofern Sie über eine Verbindung zu Salesforce verfügen, werden diese Felder direkt den Lead/Kontakt in Salesforce aufrufen, um Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie im Betrefffeld einer E-Mail ein. Achten Sie dabei darauf, dass die korrekte Formatierung gewährleistet ist.
