---
unique-page-id: 14352592
description: So fügen Sie dynamische Felder ein - Marketing to Docs - Produktdokumentation
title: Dynamische Felder einfügen
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Dynamische Felder einfügen {#how-to-insert-dynamic-fields}

Wir ermöglichen Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}`zu personalisieren. Mit diesen Feldern können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen, ohne sie für jeden Kontakt einzeln eingeben zu müssen.

>[!TIP]
>
>Das Feld &quot;first_name&quot;und &quot;Firma&quot;sind die Felder `only fields that will look to both Sales Connect and Salesforce.` &quot;Das heißt, wenn in der [Webanwendung](http://toutapp.com/login)kein Kontakt vorhanden ist, suchen wir in Salesforce nach einem Kontakt-/Interessentensdatensatz mit einer entsprechenden E-Mail-Adresse. Dann verwenden wir Informationen aus diesem Datensatz, um das Feld zu füllen.

## Dynamisches Feld in eine Vorlage einfügen {#insert-a-dynamic-field-into-a-template}

1. Suchen Sie unter **Vorlagen und Kampagnen** die zu bearbeitende Vorlage und klicken Sie auf Vorlage **bearbeiten**.
1. Klicken Sie auf Dynamische Felder **ausblenden**.

   >[!NOTE]
   >
   >Beim Versenden von Kontakten, die in Sales Connect vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese werden direkt aus dem Kontakt gezogen.

Wenn Sie Kontakte per E-Mail senden, die in Salesforce vorhanden sind, können Sie die dynamischen Felder von Salesforce nutzen. Diese beginnen alle mit &quot;sfdc&quot;. Solange Sie eine Verbindung zu Salesforce haben, rufen diese Felder direkt an den Interessenten/Kontakt in Salesforce auf, um Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie in das Betreff einer E-Mail ein. Achten Sie dabei darauf, dass Sie die richtige Formatierung haben.
