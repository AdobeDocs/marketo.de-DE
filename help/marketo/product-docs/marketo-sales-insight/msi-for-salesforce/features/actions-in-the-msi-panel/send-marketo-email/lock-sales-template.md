---
unique-page-id: 12981050
description: Verkaufsvorlage sperren - Marketing-Dokumente - Produktdokumentation
title: Verkaufsvorlage sperren
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Verkaufsvorlage sperren {#lock-sales-template}

Um zu verhindern, dass CRM-Benutzer Verkaufsvorlagen bearbeiten, können Administratoren die Möglichkeit zum Sperren von Vorlagen aktivieren, wodurch Benutzer Vorlagen einzeln im E-Mail-Editor sperren können.

>[!CAUTION]
>
>Diese Funktion funktioniert nur für Salesforce und ist nicht mit Microsoft Dynamics oder anderen CRMs kompatibel. Vorlagen, auf die über die Outlook- oder Gmail-Plugins zugegriffen wird, werden nicht gesperrt, da der Editor nicht von Marketo gesteuert wird.

## Vorlage sperren {#enable-lock-template}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Gehen Sie zu **Admin** und klicken Sie dann auf **Sales Insight**.

   ![](assets/1.png)

1. Klicken Sie unter **Einstellungen** auf **Bearbeiten**.

   ![](assets/2.png)

1. Aktivieren Sie die Option **Fähigkeit zum Sperren von Vorlagen** aktivieren. Klicken Sie auf **Speichern**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Standardmäßig ist dieses Kontrollkästchen aktiviert und die Möglichkeit, Vorlagen zu sperren, ist aktiviert. Wenn Sie diese Option deaktivieren, wird die Funktion &quot;Vorlage sperren&quot;im E-Mail-Editor deaktiviert.

>[!NOTE]
>
>Eine Änderung dieser Einstellung als Administrator hat **keine** rückwirkenden Auswirkungen auf vorhandene Vorlagen. Das heißt, sie werden nicht automatisch gesperrt.

## Vorlage im E-Mail-Editor sperren {#lock-template-in-the-email-editor}

1. Wählen Sie die E-Mail, die Sie sperren möchten, und klicken Sie dann auf Entwurf **bearbeiten**.

   ![](assets/5.png)

1. Klicken Sie im E-Mail-Editor auf **E-Mail-Einstellungen**.

   ![](assets/6.png)

1. Markieren Sie **Auf Marketing Publish Sales Insight** veröffentlichen, wenn es nicht bereits markiert ist. Sie können jetzt die Option **CRM-Benutzer zum Bearbeiten von E-Mails** zulassen deaktivieren, um die Vorlage zu sperren. Klicken Sie auf **Speichern**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Standardmäßig ist dieses Kontrollkästchen aktiviert und CRM-Benutzer dürfen E-Mails bearbeiten.

