---
unique-page-id: 2360245
description: Entfernen Sie den Abmeldungstext aus dem Abschnitt "Admin-E-Mail"- Marketo-Dokumente - Produktdokumentation
title: Entfernen Sie den Abmelde-Text aus dem Abschnitt "Admin-E-Mail".
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Entfernen Sie den Abmelde-Text aus dem Abschnitt Admin > E-Mail . {#remove-unsubscribe-text-from-the-admin-email-section}

Der einzige Grund, warum Sie den Inhalt zum Abmelden jemals vollständig aus dem Bereich **[!UICONTROL Admin]** > **[!UICONTROL E-Mail]** entfernen sollten, besteht darin, den Abmelde-Link in die E-Mail-Vorlagen selbst zu erstellen. Das Textfeld verfügt über eine Validierung, die das Speichern ohne Inhalt nicht erlaubt. Sie können dies umgehen, indem Sie einen kleinen HTML-Kommentar hinzufügen. Der HTML-Kommentar wird nicht im E-Mail-Client angezeigt, da er die E-Mail in HTML rendert und die Kommentare weggelassen werden. Hier ist, wie man das macht.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Wählen Sie den gesamten Text aus und drücken Sie die Taste **[!UICONTROL Löschen]**.

   >[!CAUTION]
   >
   >Kopieren Sie vor dem Löschen das Dokument als Sicherung in ein Textdokument.

1. Geben Sie in `<!--This is a comment -->` ein.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Für den **Text abmelden** müssen Sie ein einzelnes Zeichen hinzufügen. Verwenden Sie einen Bindestrich oder einen Punkt.
