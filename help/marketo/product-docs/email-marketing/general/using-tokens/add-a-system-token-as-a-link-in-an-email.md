---
unique-page-id: 1900573
description: Hinzufügen eines System-Tokens als Link in einer E-Mail - Marketo Docs - Produktdokumentation
title: Hinzufügen eines System-Tokens als Link in einer E-Mail
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Hinzufügen eines System-Tokens als Link in einer E-Mail {#add-a-system-token-as-a-link-in-an-email}

Sie können diese System-Token verwenden, um die Position von speziellen Links in Ihren E-Mails anzupassen.

Die folgenden Token können als Links in einer E-Mail- oder E-Mail-Vorlage verwendet werden:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Diese Token können nur dann auf **nicht** geklickt werden, wenn sie sich in einem Ankerlink befinden. Außerdem können sie **nicht** in ein My Token eingebettet werden.

So fügen Sie sie einer E-Mail hinzu:

1. Suchen und wählen Sie Ihre E-Mail aus und klicken Sie dann auf **Entwurf bearbeiten**.

   ![](assets/one-1.png)

1. Doppelklicken Sie in einen bearbeitbaren Bereich.

   ![](assets/two-1.png)

1. Markieren Sie den Text, den Sie in einen Link konvertieren möchten, der das Token enthält, und klicken Sie auf die Schaltfläche **Link einfügen/bearbeiten** .

   ![](assets/three-1.png)

1. Geben Sie das Token in die Link-URL ein und klicken Sie auf **Einfügen**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Kopieren/Einfügen Sie das gewünschte Token: **`{{system.forwardToFriendLink}}`** oder **`{{system.unsubscribeLink}}`** oder **`{{system.viewAsWebpageLink}}`**

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Wenn Sie diesen Ansatz verwenden, um das System-Token &quot;viewAsWebpageLink&quot;hinzuzufügen, können Sie es mit Token **nicht** überschreiben. Verwenden Sie stattdessen den Ansatz [Als Webseitenlink anzeigen zu einer E-Mail hinzufügen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) , mit dem Sie &quot;viewAsWebPageLink&quot;mithilfe von Token überschreiben können.

>[!NOTE]
>
>Vergessen Sie nicht, nach Abschluss [Ihre E-Mail zu genehmigen](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md).

Schön gemacht! Jetzt wissen Sie, wie Sie ein System-Token als Link in einer E-Mail hinzufügen können.
