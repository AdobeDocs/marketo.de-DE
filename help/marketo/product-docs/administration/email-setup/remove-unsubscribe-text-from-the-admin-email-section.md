---
unique-page-id: 2360245
description: Entfernen Sie den Text für das Abbestellen aus dem Abschnitt "Admin -> E-Mail"- Marketing zu Dokumenten - Produktdokumentation.
title: Entfernen Sie den Text zum Abmelden aus dem Abschnitt "Admin -> E-Mail".
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Entfernen Sie den Text zum Abmelden aus dem Abschnitt &quot;Admin -> E-Mail&quot; {#remove-unsubscribe-text-from-the-admin-email-section}

Der einzige Grund, warum Sie den Inhalt zum Abbestellen des Abonnements aus dem Bereich &quot;Admin > E-Mail&quot;vollständig entfernen sollten, ist, wenn Sie den Link zum Abbestellen des Abonnements in die E-Mail-Vorlagen selbst erstellen. Das Textfeld verfügt über eine Überprüfung, die das Speichern ohne Inhalt nicht zulässt. Sie können dies umgehen, indem Sie einen kleinen HTML-Kommentar hinzufügen. Der HTML-Kommentar wird nicht im E-Mail-Client angezeigt, da er die E-Mail in HTML wiedergibt und die Kommentare weggelassen werden. Hier ist, wie man das macht.

1. Gehen Sie zu **Admin** und klicken Sie auf **E-Mail**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Wählen Sie den gesamten Text aus und drücken Sie die **Entf **Taste.

   >[!CAUTION]
   >
   >Kopieren Sie vor dem Löschen dieses Dokuments als Sicherung in ein Textzeichen.

1. Geben Sie **<!--This is a comment -->** ein.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Klicken Sie auf **Änderungen speichern**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Für den **Abmelden-Text **müssen Sie ein einzelnes Zeichen hinzufügen. Verwenden Sie einen Bindestrich oder einen Punkt.

