---
unique-page-id: 4719306
description: Ausblenden eines Salesforce-Felds in der Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Ausblenden eines Salesforce-Felds bei der Marketo-Synchronisierung
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 3%

---

# Ausblenden eines Salesforce-Felds bei der Marketo-Synchronisierung {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Nicht jedes Feld in Salesforce ist für das Marketing nützlich. Sie können die Synchronisierungsleistung optimieren, indem Sie nur die von Ihnen benötigten Felder einbeziehen. So kann man ein Feld vor dem Marketo Engage ausblenden.

1. Klicken Sie auf das Namensmenü und wählen Sie **[!UICONTROL Setup]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Geben Sie in der Suchleiste „Profile“ ein und klicken Sie unter **[!UICONTROL Benutzer verwalten]** auf **[!UICONTROL Profile]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Klicken Sie auf das Profil des Benutzers synchronisieren.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Klicken Sie **[!UICONTROL Abschnitt Sicherheit auf]** auf **[!UICONTROL Anzeigen]** neben dem Objekt, das das Zielfeld enthält.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deaktivieren Sie das **[!UICONTROL Sichtbar]** neben dem Feld, das Sie ausblenden möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Wenn das in Salesforce ausgeblendete Feld bereits mit Marketo synchronisiert wurde, müssen Sie es auch in Marketo ausblenden, wenn Sie es nicht verwenden möchten.

   Das ist alles! Dieses Feld wird nach Abschluss der nächsten Synchronisierung nicht mehr in Marketo angezeigt.

   >[!MORELIKETHIS]
   >
   >[Ein- und Ausblenden eines Felds](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
