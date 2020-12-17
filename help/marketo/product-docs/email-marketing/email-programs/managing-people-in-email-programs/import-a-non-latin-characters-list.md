---
unique-page-id: 5472678
description: Importieren einer Liste für nicht lateinische Zeichen - Marketing Docs - Produktdokumentation
title: Importieren einer Liste mit nicht lateinischen Zeichen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Liste für nicht lateinische Zeichen {#import-a-non-latin-characters-list} importieren

Sie versuchen, eine Datei zu importieren, die nicht in Englisch? Die Liste sieht perfekt aus, wenn Sie sie mit Excel öffnen.

![](assets/image2015-2-10-9-3a34-3a57.png)

Aber wenn man es in Marketo importiert, sieht man vielleicht, dass die nicht-englischen Zeichen nicht richtig aufgenommen werden.

![](assets/image2015-2-10-9-3a35-3a49.png)

Dies liegt daran, dass die Datei nicht ordnungsgemäß gespeichert wurde, damit Marketo alle nicht-lateinischen Zeichen erkennen kann. Die gute Nachricht ist, dass es ein paar einfache Schritte gibt, die Sie ausführen können, um es zu beheben.

1. Wählen Sie **Speichern unter...** aus dem Menü **Datei** in Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Wählen Sie **UTF-16 Unicode Text (.txt)** als Option **Format**. Dadurch wird die Datei so kodiert, wie Marketo sie anzeigen kann.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo unterstützt auch UTF-8, Shift-JIS oder EUC-JP.

1. Excel speichert die neue Datei als Textdatei mit der Erweiterung .txt. Aber es konvertiert auch alle Kommas in der Datei in Registerkarten. Wir müssen es zurückändern.

   >[!TIP]
   >
   >Sie können die Textdatei mit **Notepad** öffnen, wenn Sie Windows verwenden, oder **TextEdit**, wenn Sie einen Mac verwenden.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Wählen Sie eine Registerkarte aus dem Dokument und kopieren Sie sie.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Wählen Sie **Suchen und Ersetzen...** aus dem Menü **Bearbeiten**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Entsprechende Aktion für Windows-Benutzer: **Bearbeiten > Ersetzen...**

1. Fügen Sie die Registerkarte, die Sie in Schritt 4 kopiert haben, in das erste (zu ersetzende) Feld ein und geben Sie im zweiten Feld (durch) ein Komma ein. Klicken Sie auf **All**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Und voila, alle Kommas sind zurück und wir sind bereit zu rollen.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importieren Sie die neue Datei nach Marketo, und die Informationen sollten diesmal korrekt angezeigt werden.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Alle importierten Datums-/Uhrzeitfelder werden als &quot;Central Time&quot;behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (Amerika/Chicago) umzuwandeln.

Wir wissen, dass das seltsam ist, aber es funktioniert. Alles Gute zum Import!