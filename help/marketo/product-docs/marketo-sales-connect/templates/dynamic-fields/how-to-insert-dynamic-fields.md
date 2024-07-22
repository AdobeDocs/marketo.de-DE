---
unique-page-id: 14352592
description: Hinzufügen dynamischer Felder - Marketo-Dokumente - Produktdokumentation
title: Dynamische Felder einfügen
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Dynamische Felder einfügen {#how-to-insert-dynamic-fields}

Sie können Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}` personalisieren. Mithilfe dieser Felder können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen lassen, ohne sie für jeden Kontakt einzeln eingeben zu müssen.

>[!TIP]
>
>Die Felder &quot;first_name&quot;und &quot;company&quot;sind die einzigen Felder, die sowohl für Sales Connect als auch für Salesforce gelten. Wenn also kein Kontakt in der [Webanwendung](https://toutapp.com/login) vorhanden ist, suchen wir in Salesforce nach einem Kontakt, um zu sehen, ob wir einen Kontakt-/Lead-Datensatz mit einer übereinstimmenden E-Mail-Adresse finden können. Dann verwenden wir Informationen aus diesem Datensatz, um das Feld zu füllen.

## Dynamisches Feld in eine Vorlage einfügen {#insert-a-dynamic-field-into-a-template}

1. Suchen Sie in **Vorlagen und Kampagnen** die Vorlage, die Sie bearbeiten möchten, und klicken Sie auf **Vorlage bearbeiten**.

1. Klicken Sie auf **Dynamische Felder ausfüllen**.

   >[!NOTE]
   >
   >Wenn Sie Kontakte per E-Mail senden, die in Sales Connect vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese werden direkt vom Kontakt abgerufen.

Wenn Sie Kontakte per E-Mail versenden, die in Salesforce vorhanden sind, können Sie die dynamischen Felder von Salesforce nutzen. Diese beginnen alle mit &quot;sfdc&quot;. Solange Sie eine Verbindung zu Salesforce haben, rufen diese Felder direkt an den Lead/Kontakt in Salesforce auf, um Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie in das Betrefffeld einer E-Mail ein. Achten Sie dabei darauf, dass Sie über die richtige Formatierung verfügen.
