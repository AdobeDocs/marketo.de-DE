---
unique-page-id: 2360245
description: Entfernen Sie den Abmeldungstext aus dem Abschnitt "Admin-E-Mail"- Marketo-Dokumente - Produktdokumentation
title: Entfernen Sie den Abmelde-Text aus dem Abschnitt "Admin-E-Mail".
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 3%

---

# Entfernen Sie den Abmelde-Text aus dem Abschnitt &quot;Admin-E-Mail&quot;. {#remove-unsubscribe-text-from-the-admin-email-section}

Der einzige Grund, warum Sie den Inhalt der Abmeldung jemals vollständig aus der **[!UICONTROL Admin]** > **[!UICONTROL Email]** ist, wenn Sie den Abmelde-Link in die E-Mail-Vorlagen selbst erstellen möchten. Das Textfeld verfügt über eine Validierung, die das Speichern ohne Inhalt nicht erlaubt. Sie können dies umgehen, indem Sie einen kleinen HTML-Kommentar hinzufügen. Der HTML-Kommentar wird nicht im E-Mail-Client angezeigt, da er die E-Mail in HTML rendert und die Kommentare weggelassen werden. Hier ist, wie man das macht.

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Klicks **[!UICONTROL Email]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Wählen Sie den gesamten Text aus und drücken Sie die **[!UICONTROL Löschen]** Schlüssel.

   >[!CAUTION]
   >
   >Kopieren Sie vor dem Löschen das Dokument als Sicherung in ein Textdokument.

1. Geben Sie ein `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Klicks **[!UICONTROL Änderungen speichern]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Für **Text abmelden** müssen Sie ein einzelnes Zeichen hinzufügen. Verwenden Sie einen Bindestrich oder einen Punkt.
