---
unique-page-id: 4719306
description: Ausblenden eines Salesforce-Felds aus der Marketo-Synchronisierung - Marketo Docs - Produktdokumentation
title: Ausblenden eines Salesforce-Felds aus der Marketo-Synchronisierung
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Ausblenden eines Salesforce-Felds in der Marketo-Synchronisierung {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Nicht jedes Feld in Salesforce ist nützlich für Marketing. Sie können die Synchronisierungsleistung optimieren, indem Sie nur die erforderlichen Felder einschließen. So kann man ein Feld vor Marketo ausblenden.

1. Klicken Sie auf Ihr Namensmenü und wählen Sie **Setup**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Geben Sie **Profil** in die Suchleiste ein und klicken Sie unter **Benutzer verwalten** auf **Profil**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Klicken Sie unter dem Abschnitt **Sicherheit auf Feldebene** auf **Ansicht** neben dem Objekt, das das Feld Zielgruppe enthält.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Klicken Sie auf **Bearbeiten**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deaktivieren Sie das Kontrollkästchen **Sichtbar** neben dem Feld, das Sie ausblenden möchten. Klicken Sie auf **Speichern**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Wenn das in Salesforce ausgeblendete Feld bereits mit Marketo synchronisiert wurde, müssen Sie es auch in Marketo ausblenden, wenn Sie es nicht verwenden möchten.

   Das ist&#39;s! Dieses Feld wird in Marketo nach Abschluss der nächsten Synchronisierung nicht mehr angezeigt.

   >[!MORELIKETHIS]
   >
   >[Ein Feld ein- und ausblenden](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
