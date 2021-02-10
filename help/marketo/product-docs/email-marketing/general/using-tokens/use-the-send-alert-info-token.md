---
unique-page-id: 2952678
description: Verwenden Sie das Token "Warnhinweisinformationen senden"{SP_Send_Alert_Info} - "Marketing to Docs"- Produktdokumentation
title: Verwenden des Tokens "Warnhinweisinformationen senden"
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---


# Verwenden Sie das Token für die Versandwarnungsinformationen {#use-the-send-alert-info-token-sp-send-alert-info}

Das Token `{{SP_Send_Alert_Info}}` ist ein spezielles Token, das beim Erstellen von Warn-E-Mails für Ihr Vertriebsteam verwendet wird.

>[!TIP]
>
>Dieses Token funktioniert nur wie vorgesehen, wenn die E-Mail mit dem Textfluss [Warnung senden](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) gesendet wird. Es funktioniert nicht, wenn es in einem Schritt zum Senden einer E-Mail-Benachrichtigung verwendet wird.

Beispiel-Warnung:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Kopf hoch! URLs in Warnungen haben Ablaufdaten, um sicherzustellen, dass sie über eine Kadenz verfügen, die diese Arten von Nachrichten unterstützt. Ablaufdaten werden von einem Admin](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md) konfiguriert.[

Die folgenden Informationen sind Teil von `{{SP_Send_Alert_Info}}`:

* Vorname und Nachname als Link zu den Personendetails in Marketo
* Ein Link zur Person in Ihrem CRM-System
* Der Name der Kampagne in Marketo, die die Warnung gesendet hat
* Zeitpunkt der Versendung der Ausschreibung

>[!NOTE]
>
>Der Link zum CRM erscheint nur, wenn sich die Person im CRM-System befindet (derzeit nicht mit Dynamics CRM verfügbar). Der Link ist sowohl für Marketo- als auch für Nicht-Marketo-Benutzer zugänglich.

## hinzufügen des Tokens SP_Send_Alert_Info an eine E-Mail {#add-the-sp-send-alert-info-token-to-an-email}

1. Wählen Sie die E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/one-3.png)

1. Klicken Sie bei gedrückter Dublette auf den bearbeitbaren Bereich, dem Sie das Token hinzufügen möchten.

   ![](assets/two-3.png)

1. Platzieren Sie den Cursor an der Stelle, an der das Token stehen soll, und klicken Sie dann auf die Schaltfläche **Token einfügen**.

   ![](assets/three-3.png)

1. Suchen Sie das Token **`{{SP_Send_Alert_Info}}`** und klicken Sie auf **Einfügen**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>Vergiss nicht, deine E-Mail zu genehmigen!

Gut! Dieses Token ist sehr nützlich und Sie sollten es in allen Warnungen verwenden, die Sie für Ihr Verkaufsteam erstellen.
