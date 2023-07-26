---
unique-page-id: 1900577
description: Erstellen eines E-Mail-Skript-Tokens - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Skript-Token erstellen
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# E-Mail-Skript-Token erstellen {#create-an-email-script-token}

Für fortgeschrittene Entwickler können Sie [Velocity-Skripte](https://velocity.apache.org/engine/1.7/user-guide.html) in Ihren E-Mails. Hier ist, wie man das macht.

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Suchen Sie nach einem beliebigen Programm (Ereignis, Standard, Interaktion usw.) und wählen Sie es aus.

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Unter dem **Meine Token** Registerkarte, ziehen Sie eine **Email Script** Token.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Benennen Sie Ihr E-Mail-Skript-Token und **Klicken Sie zum Bearbeiten** Inhalt.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Verwenden Sie die Baumstruktur auf der rechten Seite, um einzuziehen. **Person, Chancen** oder **Benutzerdefiniertes Objekt** Token.

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

   * [Dokumentation zu Marketo Developers Email Scripting](https://developers.marketo.com/email-scripting/)
   * [Velocity-Benutzerhandbuch](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity-Referenzhandbuch](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Klicken Sie nach Abschluss des Skripts auf **Speichern**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Klicks **Speichern** einmalig.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Jetzt können Sie dieses Token in Ihren E-Mails verwenden. Das Skript wird jedes Mal ausgeführt, wenn eine E-Mail gesendet wird.

>[!MORELIKETHIS]
>
>[E-Mail-Skript-Token hinzufügen](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
