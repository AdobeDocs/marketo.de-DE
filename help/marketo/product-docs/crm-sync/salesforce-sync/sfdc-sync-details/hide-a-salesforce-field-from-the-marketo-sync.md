---
unique-page-id: 4719306
description: Erfahren Sie, wie Sie zur Leistungsoptimierung ein Salesforce-Feld aus der Marketo-Synchronisierung ausblenden. Verwenden Sie die Sicherheit auf Feldebene für das Synchronisierungsbenutzerprofil, um nicht benötigte Felder auszuschließen.
title: Ausblenden eines Salesforce-Felds bei der Marketo-Synchronisierung
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/dUOuEuS689QIwRxhrGKOOjZhG6LC-441ytwyqkPbkDo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 11%

---

# Ausblenden eines [!DNL Salesforce] Felds bei der Marketo-Synchronisierung {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

Nicht jedes Feld in Salesforce ist für das Marketing nützlich. Sie können die Synchronisierungsleistung optimieren, indem Sie nur die von Ihnen benötigten Felder einbeziehen. So können Sie ein Feld in Marketo Engage ausblenden.

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
   >Wenn das Feld, das Sie in [!DNL Salesforce] ausblenden, bereits mit Marketo synchronisiert wurde, müssen Sie es auch in Marketo ausblenden, wenn Sie es nicht verwenden möchten.

   Dieses Feld wird nach Abschluss der nächsten Synchronisierung nicht mehr in Marketo angezeigt.

   >[!MORELIKETHIS]
   >
   >[Ein- und Ausblenden eines Felds](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
