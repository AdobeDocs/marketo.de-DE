---
unique-page-id: 1900577
description: Erstellen eines E-Mail-Skript-Tokens - Marketing Docs - Produktdokumentation
title: E-Mail-Skript-Token erstellen
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Erstellen eines E-Mail-Skript-Tokens {#create-an-email-script-token}

Für fortgeschrittene Entwickler können Sie [Velocity-Skripte](https://velocity.apache.org/engine/1.7/user-guide.html) in Ihren E-Mails verwenden. Hier ist, wie man das macht.

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Suchen und wählen Sie ein beliebiges Programm (Ereignis, Standard oder Interaktion usw.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Ziehen Sie unter der Registerkarte **Meine Token** ein Token **E-Mail-Skript**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Benennen Sie Ihr E-Mail-Skript-Token und **klicken Sie auf , um den Inhalt zu bearbeiten.**

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Verwenden Sie die Struktur auf der rechten Seite, um die Token **Person, Gelegenheit** oder **Benutzerdefiniertes Objekt** zu ziehen.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Beim Zugriff auf ein Array (Gelegenheit oder benutzerdefiniertes Objekt) sind Sie auf die letzten 10 Elemente beschränkt, die der Person zugeordnet sind.

1. Beachten Sie, dass das Token nach dem Ziehen in den Skript-Editor aktiviert/aktiv wird.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Wenn Sie in Token frei eingeben, stellen Sie sicher, dass alle entsprechenden Token im Baum markiert/aktiviert werden. Andernfalls werden sie als normaler Text behandelt und funktionieren nicht.

1. Schreiben Sie Ihr Skript in Velocity. Im Folgenden finden Sie einige nützliche Ressourcen:

   * [Marketing-Entwickler - E-Mail-Skriptdokumentation](https://developers.marketo.com/email-scripting/)
   * [Velocity Benutzerhandbuch](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity Reference Guide](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Klicken Sie nach Abschluss des Skripts auf **Speichern**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Klicken Sie noch einmal auf **Speichern**.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Nun können Sie dieses Token in Ihren E-Mails verwenden. Das Skript wird jedes Mal ausgeführt, wenn eine E-Mail gesendet wird.

>[!MORELIKETHIS]
>
>[hinzufügen eines E-Mail-Skript-Tokens an Ihre E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
