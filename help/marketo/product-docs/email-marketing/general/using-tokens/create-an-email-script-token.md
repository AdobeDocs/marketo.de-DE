---
unique-page-id: 1900577
description: Erstellen eines E-Mail-Skript-Tokens - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Skript-Token erstellen
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# E-Mail-Skript-Token erstellen {#create-an-email-script-token}

Für fortgeschrittene Entwickler können Sie [Velocity-Skripte](https://velocity.apache.org/engine/1.7/user-guide.html) in Ihren E-Mails verwenden. Hier ist, wie man das macht.

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Suchen Sie nach einem beliebigen Programm (Ereignis, Standard, Interaktion usw.) und wählen Sie es aus.

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Ziehen Sie auf der Registerkarte **My Tokens** ein Token vom Typ **E-Mail-Skript** .

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Benennen Sie Ihr E-Mail-Skript-Token und **klicken Sie darauf, um den Inhalt von** zu bearbeiten.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Verwenden Sie die Baumstruktur auf der rechten Seite, um die Token **Person, Opportunity** oder **Benutzerdefiniertes Objekt** einzuziehen.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Beim Zugriff auf ein Array (Opportunities oder benutzerdefiniertes Objekt) sind Sie auf die letzten 10 Elemente beschränkt, die mit der Person verknüpft sind.

1. Beachten Sie, dass das Token nach dem Ziehen in den Skript-Editor aktiviert/aktiv wird.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Wenn Sie Token frei eingeben, stellen Sie sicher, dass Sie alle entsprechenden Token im Baum aktivieren/aktivieren. Andernfalls werden sie als normaler Text behandelt und funktionieren nicht.

1. Schreiben Sie Ihr Skript in Velocity. Im Folgenden finden Sie einige nützliche Ressourcen:

   * [Dokumentation für E-Mail-Skripterstellung für Marketo-Entwickler](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Velocity-Benutzerhandbuch](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity-Referenzhandbuch](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Klicken Sie nach Abschluss des Skripts auf **Speichern**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Klicken Sie noch einmal auf **Speichern** .

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Jetzt können Sie dieses Token in Ihren E-Mails verwenden. Das Skript wird jedes Mal ausgeführt, wenn eine E-Mail gesendet wird.

>[!MORELIKETHIS]
>
>[Hinzufügen eines E-Mail-Skript-Tokens zu Ihrer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
