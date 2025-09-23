---
unique-page-id: 12981050
description: Verkaufsvorlage sperren - Marketo-Dokumente - Produktdokumentation
title: Sperren einer Sales Insight-Vorlage
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 4%

---

# Sperren einer Sales Insight-Vorlage {#lock-sales-template}

Um zu verhindern, dass CRM-Benutzer Verkaufsvorlagen bearbeiten, können Administratoren Vorlagen sperren. Dadurch können Benutzer Vorlagen einzeln im E-Mail-Editor sperren.

>[!CAUTION]
>
>Diese Funktion funktioniert nur für [!DNL Salesforce] und ist nicht mit [!DNL Microsoft Dynamics] oder anderen CRMs kompatibel. Vorlagen, auf die über die Plug-ins [!DNL Outlook] oder Gmail zugegriffen wird, werden nicht gesperrt, da der Editor nicht von Marketo gesteuert wird.

## Sperrvorlage aktivieren {#enable-lock-template}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Gehen Sie zu **[!UICONTROL Admin]** und klicken Sie dann auf **[!UICONTROL Sales Insight]**.

   ![](assets/1.png)

1. Klicken **[!UICONTROL unter]** Einstellungen **[!UICONTROL auf]**.

   ![](assets/2.png)

1. Aktivieren Sie **[!UICONTROL Möglichkeit zum Sperren von Vorlagen aktivieren]**. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Standardmäßig ist dieses Kontrollkästchen aktiviert und die Möglichkeit, Vorlagen zu sperren, ist aktiviert. Wenn Sie diese Option deaktivieren, wird die Funktion „Vorlage sperren“ im E-Mail-Editor deaktiviert.

>[!NOTE]
>
>Wenn Sie diese Einstellung als Admin ändern **werden** Vorlagen nicht rückwirkend geändert, d. h. sie werden nicht automatisch gesperrt.

## Vorlage im E-Mail-Editor sperren {#lock-template-in-the-email-editor}

1. Wählen Sie die zu sperrende E-Mail aus und klicken Sie dann auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/5.png)

1. Klicken Sie im E-Mail-Editor auf **[!UICONTROL E-Mail-Einstellungen]**.

   ![](assets/6.png)

1. Markieren Sie **[!UICONTROL In Marketo Sales Insight veröffentlichen]**, falls dies nicht bereits aktiviert ist. Sie können jetzt die Option **[!UICONTROL CRM-Benutzer darf E-Mail bearbeiten]** deaktivieren, um die Vorlage zu sperren. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Standardmäßig ist dieses Kontrollkästchen aktiviert und CRM-Benutzer dürfen E-Mails bearbeiten.
