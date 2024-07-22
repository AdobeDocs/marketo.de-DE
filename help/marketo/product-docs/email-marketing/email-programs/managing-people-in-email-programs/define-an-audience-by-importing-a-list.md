---
unique-page-id: 1900597
description: Definieren einer Zielgruppe durch Importieren einer Liste - Marketo Docs - Produktdokumentation
title: Definieren einer Zielgruppe durch Importieren einer Liste
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Definieren einer Zielgruppe durch Importieren einer Liste {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[E-Mail für ein E-Mail-Programm erstellen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Nachdem Sie ein E-Mail-Programm erstellt haben, möchten Sie ihm mitteilen, an wen die E-Mail gesendet werden soll. Erstellen Sie dazu eine Smart-Liste ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) oder importieren Sie eine Liste. [ Hier erfahren Sie, wie Sie dies durch Importieren einer Liste erreichen.

>[!NOTE]
>
>Die Bestimmung der Audience funktioniert nur, wenn das E-Mail-Programm nicht genehmigt wurde.
>
>Alle Datums-/Uhrzeitfelder, die importiert werden, werden als Central Time behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie Ihr E-Mail-Programm aus und klicken Sie dann unter der Kachel Zielgruppe auf Liste importieren .

   ![](assets/importlist.png)

1. Das Listenimportfenster wird geöffnet. Klicken Sie auf **Durchsuchen** und wählen Sie die zu importierende Datei aus. Nachdem Sie Ihre Personenliste ausgewählt haben, klicken Sie auf **Weiter**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass die Liste UTF-8-, UTF-16-, Shift-JIS- oder EUC-JP-kodiert ist und die Dateigröße 50 MB nicht überschreitet.

1. Vergewissern Sie sich, dass die Felder in Ihrer Datei korrekt zugeordnet sind, und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo wird sich an die Zuordnungen für zukünftige Importe erinnern!

1. Geben Sie einen **Namen** für Ihre Liste ein und klicken Sie auf **Importieren**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Gehen Sie nach Abschluss des Imports in den Tab Hauptprogramm . Du wirst sehen, wie viele Leute dich qualifizieren werden.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definition**
>
>Haben Sie die Blockierungsnummer bemerkt? Diese Zahl ist eine Untergruppe der qualifizierten Personen und stellt Personen dar, die diese E-Mail nicht erhalten können, weil sie:
>
>* Abbestellt
>* Marketing eingestellt
>* Auf der Sperrliste
>* E-Mail-Adresse ungültig
>* Leere E-Mail
>
>Klicken Sie auf die Nummer für eine detaillierte Liste der Personen, die von Mailings ausgeschlossen sind.
>
>Verwenden Sie die Schaltfläche ![—](assets/image2014-10-23-16-3a32-3a36-1.png) auf der Kachel **Zielgruppe** , um zu sehen, wie viele Personen sich für den Erhalt der E-Mail anhand von Kriterien mit intelligenten Listen qualifiziert haben. Ziehen Sie die Zahl Blockiert von der Zahl Personen ab, um die Gesamtzahl der Personen zu erhalten, die die E-Mail erhalten werden.

>[!TIP]
>
>Sie müssen nicht warten, bis der Listenimport abgeschlossen ist. Du kannst weiterarbeiten, wenn du willst.

Fantastisch! Jetzt ist es an der Zeit, eine bereits existierende E-Mail auszuwählen oder eine neue E-Mail zu erstellen, die an diese Personen gesendet wird.

>[!MORELIKETHIS]
>
>* [Vorhandene E-Mail auswählen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [E-Mail für ein E-Mail-Programm erstellen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
