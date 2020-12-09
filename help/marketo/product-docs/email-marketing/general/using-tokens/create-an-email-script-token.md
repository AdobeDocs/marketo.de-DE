---
unique-page-id: 1900577
description: Erstellen eines E-Mail-Skript-Tokens - Marketing Docs - Produktdokumentation
title: E-Mail-Skript-Token erstellen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# E-Mail-Skript-Token erstellen {#create-an-email-script-token}

Für fortgeschrittene Entwickler können Sie [Velocity-Skripte](http://velocity.apache.org/engine/1.7/user-guide.html) in Ihren E-Mails verwenden. Hier ist, wie man das macht.

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie ein beliebiges Programm (Ereignis, Standard oder Interaktion usw.) aus.

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Ziehen Sie unter der Registerkarte &quot; **Meine Token** &quot;ein Token für ein **E-Mail-Skript** .

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Benennen Sie Ihr E-Mail-Skript-Token und **klicken Sie auf , um den Inhalt zu bearbeiten** .

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Verwenden Sie die Struktur auf der rechten Seite, um Token für **Personen, Chancen** oder **benutzerdefinierte Objekte** einzuziehen.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Beim Zugriff auf ein Array (Gelegenheit oder benutzerdefiniertes Objekt) sind Sie auf die letzten 10 Elemente beschränkt, die der Person zugeordnet sind.

1. Beachten Sie, dass das Token nach dem Ziehen in den Skript-Editor aktiviert/aktiv wird.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Wenn Sie in Token frei eingeben, stellen Sie sicher, dass alle entsprechenden Token im Baum markiert/aktiviert werden. Andernfalls werden sie als normaler Text behandelt und funktionieren nicht.

1. Schreiben Sie Ihr Skript in Velocity. Im Folgenden finden Sie einige nützliche Ressourcen:

   * [Marketing-Entwickler - E-Mail-Skriptdokumentation](http://developers.marketo.com/email-scripting/)
   * [Velocity Benutzerhandbuch](http://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity Reference Guide](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Klicken Sie nach Abschluss des Skripts auf **Speichern**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Klicken Sie erneut auf **Speichern** .

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Nun können Sie dieses Token in Ihren E-Mails verwenden. Das Skript wird jedes Mal ausgeführt, wenn eine E-Mail gesendet wird.

>[!MORELIKETHIS]
>
>* [hinzufügen eines E-Mail-Skript-Tokens an Ihre E-Mail](add-an-email-script-token-to-your-email.md)

>



