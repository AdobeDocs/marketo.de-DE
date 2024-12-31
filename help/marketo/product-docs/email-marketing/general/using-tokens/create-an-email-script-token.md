---
unique-page-id: 1900577
description: Erstellen eines E-Mail-Skript-Tokens - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines E-Mail-Skript-Tokens
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Erstellen eines E-Mail-Skript-Tokens {#create-an-email-script-token}

Für fortgeschrittene Entwickler können Sie [Velocity-Skripte](https://velocity.apache.org/engine/1.7/user-guide.html) in Ihren E-Mails verwenden. So geht das.

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Suchen Sie nach einem beliebigen Programm (Ereignis, Standard oder Interaktion usw.) und wählen Sie es aus.

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Ziehen Sie auf **Registerkarte** Meine Token“ ein Token **E-Mail-Skript** in den Arbeitsbereich.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Benennen Sie Ihr E-Mail-Skript-Token und **Sie zum Bearbeiten auf** Inhalt.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Verwenden Sie die Struktur auf der rechten Seite, um Token **Person, Opportunity** oder **Benutzerdefiniertes Objekt** einzufügen.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Beim Zugriff auf ein Array (Opportunity oder benutzerdefiniertes Objekt) sind Sie auf die letzten 10 Elemente beschränkt, die der Person zugeordnet sind.

1. Beachten Sie, dass das Token aktiviert/aktiviert wird, nachdem Sie es in den Skripteditor gezogen haben.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Wenn Sie Freiform-Token eingeben, aktivieren/aktivieren Sie alle entsprechenden Token in der Struktur, da sie sonst als Klartext behandelt werden und nicht funktionieren.

1. Schreiben Sie Ihr Skript in Velocity. Im Folgenden finden Sie einige nützliche Ressourcen:

   * [E-Mail-Skripterstellung für Marketo-Entwickler](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Velocity-Benutzerhandbuch](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity-Referenzhandbuch](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Klicken Sie nach Abschluss des Skripts auf **Speichern**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Klicken **noch** auf „Speichern“.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Jetzt können Sie dieses Token in Ihren E-Mails verwenden. Das Skript wird bei jedem Versand einer E-Mail ausgeführt.

>[!MORELIKETHIS]
>
>[Hinzufügen eines E-Mail-Skript-Tokens zu Ihrer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
