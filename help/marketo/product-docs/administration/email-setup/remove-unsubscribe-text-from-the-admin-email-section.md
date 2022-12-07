---
unique-page-id: 2360245
description: Entfernen Sie den Abmeldungstext aus dem Abschnitt "Admin-E-Mail"- Marketo-Dokumente - Produktdokumentation
title: Entfernen Sie den Abmelde-Text aus dem Abschnitt "Admin-E-Mail".
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 3%

---

# Entfernen Sie den Abmelde-Text aus dem Abschnitt &quot;Admin-E-Mail&quot;. {#remove-unsubscribe-text-from-the-admin-email-section}

Der einzige Grund, warum Sie den Inhalt der Abmeldung vollständig aus dem Bereich &quot;Admin > E-Mail&quot;entfernen sollten, besteht darin, den Abmelde-Link in die E-Mail-Vorlagen selbst zu integrieren. Das Textfeld verfügt über eine Validierung, die das Speichern ohne Inhalt nicht zulässt. Sie können dies umgehen, indem Sie einen kleinen HTML-Kommentar hinzufügen. Der HTML-Kommentar wird nicht im E-Mail-Client angezeigt, da er die E-Mail in HTML rendert und die Kommentare weggelassen werden. Hier ist, wie man das macht.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Klicken **Email**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Wählen Sie den gesamten Text aus und drücken Sie die **Löschen** Schlüssel.

   >[!CAUTION]
   >
   >Kopieren Sie vor dem Löschen das Dokument als Sicherung in ein Textdokument.

1. Geben Sie ein `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Klicken **Änderungen speichern**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Für **Text abmelden** müssen Sie ein einzelnes Zeichen hinzufügen. Verwenden Sie einen Bindestrich oder einen Punkt.
