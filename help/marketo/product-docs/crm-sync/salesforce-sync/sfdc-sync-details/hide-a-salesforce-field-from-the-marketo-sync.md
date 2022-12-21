---
unique-page-id: 4719306
description: Ausblenden eines Salesforce-Felds bei der Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Ausblenden eines Salesforce-Felds in der Marketo-Synchronisierung
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Ausblenden eines Salesforce-Felds in der Marketo-Synchronisierung {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Nicht jedes Feld in Salesforce ist für Marketing nützlich. Sie können die Synchronisierungsleistung optimieren, indem Sie nur die erforderlichen Felder einschließen. So können Sie ein Feld in Marketo ausblenden.

1. Klicken Sie auf Ihr Namensmenü und wählen Sie **Einrichtung**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Eingabe **profiles** in der Suchleiste und klicken Sie auf **Profile** under **Benutzer verwalten**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Unter dem **Sicherheit auf Feldebene** Abschnitt, klicken Sie auf **Ansicht** neben dem Objekt, das das Zielfeld enthält.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Klicken **Bearbeiten**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deaktivieren Sie die **Sichtbar** neben dem Feld, das Sie ausblenden möchten. Klicken **Speichern**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Wenn das in Salesforce ausgeblendete Feld bereits mit Marketo synchronisiert wurde, müssen Sie es auch in Marketo ausblenden, wenn Sie es nicht verwenden möchten.

   Das ist es! Dieses Feld wird in Marketo nach Abschluss der nächsten Synchronisierung nicht mehr angezeigt.

   >[!MORELIKETHIS]
   >
   >[Ein Feld ausblenden und ausblenden](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
