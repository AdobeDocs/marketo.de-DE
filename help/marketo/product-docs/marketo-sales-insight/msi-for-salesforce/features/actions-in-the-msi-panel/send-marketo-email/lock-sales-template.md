---
unique-page-id: 12981050
description: Verkaufsvorlage sperren - Marketo-Dokumente - Produktdokumentation
title: Verkaufsvorlage sperren
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 1%

---

# Verkaufsvorlage sperren {#lock-sales-template}

Um zu verhindern, dass CRM-Benutzer Verkaufsvorlagen bearbeiten, können Administratoren Vorlagen sperren. Dadurch können Benutzer Vorlagen einzeln im E-Mail-Editor sperren.

>[!CAUTION]
>
>Diese Funktion funktioniert nur für Salesforce und ist nicht mit Microsoft Dynamics oder anderen CRMs kompatibel. Vorlagen, auf die über das Outlook- oder Gmail-Plug-in zugegriffen wird, werden nicht gesperrt, da der Editor nicht von Marketo gesteuert wird.

## Sperrvorlage aktivieren {#enable-lock-template}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Gehen Sie zu **Admin** und klicken Sie dann auf **Sales Insight**.

   ![](assets/1.png)

1. Klicken **unter** Einstellungen **auf**.

   ![](assets/2.png)

1. Aktivieren Sie **Möglichkeit zum Sperren von Vorlagen aktivieren**. Klicken Sie auf **Speichern**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Standardmäßig ist dieses Kontrollkästchen aktiviert und die Möglichkeit, Vorlagen zu sperren, ist aktiviert. Wenn Sie diese Option deaktivieren, wird die Funktion „Vorlage sperren“ im E-Mail-Editor deaktiviert.

>[!NOTE]
>
>Wenn Sie diese Einstellung als Admin ändern **werden** Vorlagen nicht rückwirkend geändert, d. h. sie werden nicht automatisch gesperrt.

## Vorlage im E-Mail-Editor sperren {#lock-template-in-the-email-editor}

1. Wählen Sie die zu sperrende E-Mail aus und klicken Sie dann auf **Entwurf bearbeiten**.

   ![](assets/5.png)

1. Klicken Sie im E-Mail-Editor auf **E-Mail-Einstellungen**.

   ![](assets/6.png)

1. Überprüfen Sie **Publish to Marketo Sales Insight**, falls noch nicht aktiviert. Sie können jetzt die Option **CRM-Benutzer darf E-Mail bearbeiten** deaktivieren, um die Vorlage zu sperren. Klicken Sie auf **Speichern**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Standardmäßig ist dieses Kontrollkästchen aktiviert und CRM-Benutzer dürfen E-Mails bearbeiten.
