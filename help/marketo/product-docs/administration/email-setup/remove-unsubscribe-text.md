---
unique-page-id: 2360245
description: Entfernen Sie den standardmäßigen Abmelde-Inhalt aus der Admin-E-Mail, indem Sie beim Einbauen des Links in Vorlagen einen HTML-Kommentar verwenden.
title: Entfernen des Abmeldetexts
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 7%
---
# Entfernen des Abmeldetexts {#remove-unsubscribe-text}

Der einzige Grund, warum Sie den Abmelde-Inhalt jemals vollständig aus dem Bereich **[!UICONTROL Admin]** > **[!UICONTROL E-Mail]** entfernen sollten, ist, wenn Sie sich dafür entscheiden, den Abmelde-Link in die E-Mail-Vorlagen selbst zu integrieren. Das Textfeld verfügt über eine Validierung, die das Speichern ohne Inhalt nicht zulässt. Sie können dies umgehen, indem Sie einen kleinen HTML-Kommentar hinzufügen. Der HTML-Kommentar wird nicht im E-Mail-Client angezeigt, da er die E-Mail in HTML rendert und die Kommentare weggelassen werden.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Markieren Sie den gesamten Text und drücken Sie die **[!UICONTROL Löschen]**-Taste.

   >[!CAUTION]
   >
   >Vor dem Löschen kopieren Sie diese Daten als Sicherung in ein Textdokument.

1. Geben Sie `<!--This is a comment -->` ein.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Klicken Sie **[!UICONTROL Änderungen speichern]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Für den **Text zum Abmelden** müssen Sie ein einzelnes Zeichen hinzufügen. Strich oder Punkt verwenden.
