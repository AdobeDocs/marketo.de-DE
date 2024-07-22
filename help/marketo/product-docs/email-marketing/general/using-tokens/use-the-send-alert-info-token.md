---
unique-page-id: 2952678
description: Verwenden Sie das Warnhinweisinformationen-Token senden {{SP_Send_Alert_Info}} - Marketo Docs - Produktdokumentation
title: Verwenden des Tokens "Send Alert Info"
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Verwenden des Tokens &quot;Send Alert Info&quot; {#use-the-send-alert-info-token-sp-send-alert-info}

Das `{{SP_Send_Alert_Info}}` -Token ist ein spezielles Token, das beim Erstellen von Warnhinweis-E-Mails für Ihr Verkaufsteam verwendet wird.

>[!TIP]
>
>Dieses Token funktioniert nur wie vorgesehen, wenn die E-Mail, die es enthält, mit dem Flussschritt [Warnung senden](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) gesendet wird. Sie funktioniert nicht, wenn sie in einem Schritt E-Mail-Ablauf senden verwendet wird.

Beispiel-Warnhinweis:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Kopf hoch! URLs in Warnhinweisen haben Ablaufdaten. Stellen Sie daher sicher, dass sie über eine Kadenz verfügen, die diese Arten von Nachrichten unterstützt. Ablaufdaten werden von einem Administrator konfiguriert ](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).[

Die folgenden Informationen sind als Teil von `{{SP_Send_Alert_Info}}` enthalten:

* Vor- und Nachname als Link zu den Personendetails in Marketo
* Link zur Person in Ihrem CRM
* Der Kampagnenname in Marketo, an den die Warnung gesendet wurde
* Zeitpunkt des Versands der Warnung

>[!NOTE]
>
>Der Link zum CRM-System erscheint nur, wenn sich die Person im CRM-System befindet (derzeit nicht mit Dynamics CRM verfügbar). Auf den Link können sowohl Marketo- als auch Nicht-Marketo-Benutzer zugreifen.

## SP_Send_Alert_Info-Token zu einer E-Mail hinzufügen {#add-the-sp-send-alert-info-token-to-an-email}

1. Wählen Sie die E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/one-3.png)

1. Doppelklicken Sie auf den bearbeitbaren Bereich, dem Sie das Token hinzufügen möchten.

   ![](assets/two-3.png)

1. Platzieren Sie den Cursor an die Stelle, an der das Token platziert werden soll, und klicken Sie dann auf die Schaltfläche **Token einfügen** .

   ![](assets/three-3.png)

1. Suchen und wählen Sie das Token **`{{SP_Send_Alert_Info}}`** aus und klicken Sie auf **Einfügen**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>Vergessen Sie nicht, Ihre E-Mail zu genehmigen.

Gut! Dieses Token ist sehr nützlich und sollte in allen Warnungen verwendet werden, die Sie für Ihr Verkaufsteam erstellen.
