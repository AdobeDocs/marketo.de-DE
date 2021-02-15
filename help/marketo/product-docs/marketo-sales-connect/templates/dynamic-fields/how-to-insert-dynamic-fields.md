---
unique-page-id: 14352592
description: So fügen Sie dynamische Felder ein - Marketing to Docs - Produktdokumentation
title: Dynamische Felder einfügen
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Einfügen dynamischer Felder {#how-to-insert-dynamic-fields}

Sie können Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}` personalisieren. Mit diesen Feldern können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen, ohne sie für jeden Kontakt einzeln eingeben zu müssen.

>[!TIP]
>
>Die Felder &quot;first_name&quot;und &quot;Firma&quot;sind die einzigen Felder, die sowohl auf Sales Connect als auch auf Salesforce ausgerichtet sind. Wenn also in der [Webanwendung](https://toutapp.com/login) kein Kontakt vorhanden ist, suchen wir in Salesforce nach einem Kontakt-/Interessentensdatensatz mit einer entsprechenden E-Mail-Adresse. Dann verwenden wir Informationen aus diesem Datensatz, um das Feld zu füllen.

## Dynamisches Feld in eine Vorlage {#insert-a-dynamic-field-into-a-template} einfügen

1. Suchen Sie unter **Vorlagen und Kampagnen** die zu bearbeitende Vorlage und klicken Sie auf **Vorlage bearbeiten**.

1. Klicken Sie auf **Dynamische Felder abschneiden**.

   >[!NOTE]
   >
   >Beim Versenden von Kontakten, die in Sales Connect vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese werden direkt aus dem Kontakt gezogen.

Wenn Sie Kontakte per E-Mail senden, die in Salesforce vorhanden sind, können Sie die dynamischen Felder von Salesforce nutzen. Diese beginnen alle mit &quot;sfdc&quot;. Solange Sie eine Verbindung zu Salesforce haben, rufen diese Felder direkt an den Interessenten/Kontakt in Salesforce auf, um Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie in das Betreff einer E-Mail ein. Achten Sie dabei darauf, dass Sie die richtige Formatierung haben.
