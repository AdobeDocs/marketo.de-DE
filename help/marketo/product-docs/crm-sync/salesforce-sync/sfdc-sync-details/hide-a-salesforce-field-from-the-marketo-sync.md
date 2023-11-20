---
unique-page-id: 4719306
description: Ausblenden eines Salesforce-Felds bei der Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Ausblenden eines Salesforce-Felds in der Marketo-Synchronisierung
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Ausblenden eines Salesforce-Felds in der Marketo-Synchronisierung {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Nicht jedes Feld in Salesforce ist für Marketing nützlich. Sie können die Synchronisierungsleistung optimieren, indem Sie nur die erforderlichen Felder einschließen. So kann man ein Feld vor Marketo Engage verbergen.

1. Klicken Sie auf Ihr Namensmenü und wählen Sie **[!UICONTROL Einrichtung]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Geben Sie &quot;Profile&quot;in die Suchleiste ein und klicken Sie auf **[!UICONTROL Profile]** under **[!UICONTROL Benutzer verwalten]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Unter dem **[!UICONTROL Sicherheit auf Feldebene]** Abschnitt, klicken Sie auf **[!UICONTROL Ansicht]** neben dem Objekt, das das Zielfeld enthält.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Klicks **[!UICONTROL Bearbeiten]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deaktivieren Sie die **[!UICONTROL Sichtbar]** neben dem Feld, das Sie ausblenden möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Wenn das in Salesforce ausgeblendete Feld bereits mit Marketo synchronisiert wurde, müssen Sie es auch in Marketo ausblenden, wenn Sie es nicht verwenden möchten.

   Das ist es! Dieses Feld wird in Marketo nach Abschluss der nächsten Synchronisierung nicht mehr angezeigt.

   >[!MORELIKETHIS]
   >
   >[Ein Feld ausblenden und ausblenden](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
