---
unique-page-id: 5472678
description: Importieren einer nicht lateinischen Zeichenliste - Marketo Docs - Produktdokumentation
title: Importieren einer Liste nicht lateinischer Zeichen
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Importieren einer Liste nicht lateinischer Zeichen {#import-a-non-latin-characters-list}

Versuchen Sie, eine Datei zu importieren, die nicht in Englisch ist? Die Liste sieht perfekt aus, wenn Sie sie mit Excel öffnen.

![](assets/image2015-2-10-9-3a34-3a57.png)

Wenn Sie sie jedoch in Marketo importieren, sehen Sie möglicherweise, dass die nicht englischen Zeichen nicht korrekt aufgenommen wurden.

![](assets/image2015-2-10-9-3a35-3a49.png)

Dies liegt daran, dass die Datei nicht ordnungsgemäß gespeichert wird, damit Marketo alle nicht lateinischen Zeichen erkennt. Die gute Nachricht ist, dass es ein paar einfache Schritte gibt, die Sie ausführen können, um es zu beheben.

1. Auswählen **Speichern unter...** von **Datei** in Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Auswählen **UTF-16 Unicode-Text (.txt)** als **Format** -Option. Dadurch wird die Datei so kodiert, wie Marketo sie anzeigen kann.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo unterstützt auch UTF-8, Shift-JIS oder EUC-JP.

1. Excel speichert die neue Datei als Textdatei mit der Erweiterung .txt . Es werden jedoch auch alle Kommas in der Datei in Tabs konvertiert. Wir müssen es wieder ändern.

   >[!TIP]
   >
   >Sie können die Textdatei mit **Notepad** wenn Sie Windows oder **TextEdit** wenn Sie eine Mac verwenden.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Wählen Sie eine Registerkarte aus dem Dokument aus und kopieren Sie es.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Auswählen **Suchen und Ersetzen...** von **Bearbeiten** Menü.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Die entsprechende Aktion für Windows-Benutzer ist: **Bearbeiten > Ersetzen..**

1. Fügen Sie die Registerkarte, die Sie in Schritt 4 kopiert haben, in das erste (zu ersetzende) Feld ein und geben Sie in das zweite Feld (ersetzen durch) ein Komma ein. Und klicken Sie auf **Alle**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Und voila, alle Kommas sind zurück und wir sind bereit zu rollen.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importieren Sie die neue Datei in Marketo, und die Informationen sollten diesmal korrekt angezeigt werden.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Alle Datums-/Uhrzeitfelder, die importiert werden, werden als Central Time behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

Wir wissen, dass das seltsam ist, aber es funktioniert. Alles Gute zum Import!
