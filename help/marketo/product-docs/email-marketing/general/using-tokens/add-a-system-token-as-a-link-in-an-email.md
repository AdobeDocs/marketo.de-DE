---
unique-page-id: 1900573
description: Hinzufügen eines System-Tokens als Link in einer E-Mail - Marketo Docs - Produktdokumentation
title: Hinzufügen eines System-Tokens als Link in einer E-Mail
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
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
>Diese Token werden **not** auf anklickbar sein, es sei denn, sie befinden sich in einem Ankerlink. Außerdem können sie **not** in ein My Token eingebettet sein.

So fügen Sie sie einer E-Mail hinzu:

1. Suchen und wählen Sie Ihre E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/one-1.png)

1. Doppelklicken Sie in einen bearbeitbaren Bereich.

   ![](assets/two-1.png)

1. Markieren Sie den Text, den Sie in einen Link konvertieren möchten, der das Token enthält, und klicken Sie auf **Link einfügen/bearbeiten** Schaltfläche.

   ![](assets/three-1.png)

1. Geben Sie das Token in die Link-URL ein und klicken Sie auf **Einfügen**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Kopieren/Fügen Sie das gewünschte Token ein: **`{{system.forwardToFriendLink}}`** oder **`{{system.unsubscribeLink}}`** oder **`{{system.viewAsWebpageLink}}`**

1. Klicken **Speichern**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Wenn Sie diesen Ansatz verwenden, um das System-Token &quot;viewAsWebpageLink&quot;hinzuzufügen, können Sie **not** mit Token überschreiben. Verwenden Sie stattdessen [Hinzufügen eines Links &quot;Als Webseite anzeigen&quot;zu einer E-Mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) -Ansatz, bei dem Sie &quot;viewAsWebPageLink&quot;mithilfe von Token überschreiben können.

>[!NOTE]
>
>Vergiss nicht, [E-Mail validieren](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) wann geschehen.

Gut gemacht! Jetzt wissen Sie, wie Sie ein System-Token als Link in einer E-Mail hinzufügen können.
