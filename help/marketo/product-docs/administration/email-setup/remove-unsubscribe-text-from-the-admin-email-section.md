---
unique-page-id: 2360245
description: Entfernen Sie den Abmeldetext aus dem Admin-E-Mail-Abschnitt - Marketo-Dokumente - Produktdokumentation
title: Entfernen Sie den Abmelde-Text aus dem Admin-E-Mail-Abschnitt
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Entfernen Sie den Abmelde-Text aus dem Abschnitt Admin > E-Mail . {#remove-unsubscribe-text-from-the-admin-email-section}

Der einzige Grund, warum Sie den Abmelde-Inhalt jemals vollständig aus dem Bereich **[!UICONTROL Admin]** > **[!UICONTROL E-Mail]** entfernen sollten, ist, wenn Sie sich dafür entscheiden, den Abmelde-Link in die E-Mail-Vorlagen selbst zu integrieren. Das Textfeld verfügt über eine Validierung, die das Speichern ohne Inhalt nicht zulässt. Sie können dies umgehen, indem Sie einen kleinen HTML-Kommentar hinzufügen. Der HTML-Kommentar wird nicht im E-Mail-Client angezeigt, da er die E-Mail in HTML rendert und die Kommentare weggelassen werden. So geht das.

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
