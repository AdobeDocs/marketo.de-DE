---
unique-page-id: 5472678
description: Importieren einer Liste nicht lateinischer Zeichen - Marketo-Dokumente - Produktdokumentation
title: Importieren einer Liste nicht lateinischer Zeichen
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Importieren einer Liste nicht lateinischer Zeichen {#import-a-non-latin-characters-list}

Versuchen Sie, eine Datei zu importieren, die nicht auf Englisch ist? Die Liste sieht perfekt aus, wenn Sie sie mit Excel öffnen.

![](assets/image2015-2-10-9-3a34-3a57.png)

Wenn Sie sie jedoch in Marketo importieren, stellen Sie möglicherweise fest, dass die nicht englischen Zeichen nicht korrekt erkannt werden.

![](assets/image2015-2-10-9-3a35-3a49.png)

Dies liegt daran, dass die Datei nicht ordnungsgemäß gespeichert wird, damit Marketo alle nicht lateinischen Zeichen erkennen kann. Die gute Nachricht ist, es gibt ein paar einfache Schritte, die Sie befolgen können, um es zu beheben.

1. Wählen Sie **[!UICONTROL Speichern unter]…** aus dem Menü **[!UICONTROL Datei]** in Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Wählen Sie **[!UICONTROL UTF-16 Unicode Text (.txt)]** als **[!UICONTROL Format]** Option. Dadurch wird die Datei so kodiert, wie Marketo sie anzeigen kann.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo unterstützt auch UTF-8, Shift-JIS oder EUC-JP.

1. Excel speichert die neue Datei als Textdatei mit der Erweiterung .txt. Es konvertiert aber auch alle Kommas in der Datei in Registerkarten. Wir müssen es wieder ändern.

   >[!TIP]
   >
   >Sie können die Textdatei mithilfe von **[!DNL Notepad]** öffnen, wenn Sie Windows verwenden, oder **[!DNL TextEdit]**, wenn Sie eine Mac verwenden.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Wählen Sie eine Registerkarte aus dem Dokument aus und kopieren Sie sie.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Wählen **[!UICONTROL Suchen und Ersetzen]…** aus dem Menü **[!UICONTROL Bearbeiten]** aus.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Die entsprechende Aktion für Windows-Benutzer lautet: **[!UICONTROL Bearbeiten] > [!UICONTROL Ersetzen]…**

1. Fügen Sie die in Schritt 4 kopierte Registerkarte in das erste (zu ersetzende) Feld ein und geben Sie in das zweite (durch ersetzen) Feld ein Komma ein. und klicken Sie auf **[!UICONTROL Alle]**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Und voila, alle Kommas sind zurück und wir sind bereit zu rollen.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importieren Sie die neue Datei in Marketo. Die Informationen sollten diesmal korrekt angezeigt werden.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Alle Datums-/Uhrzeitfelder, die importiert werden, werden als zentrale Zeit behandelt. Wenn Sie Datums-/Zeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

Wir wissen, dass das seltsam ist, aber es funktioniert. Viel Spaß beim Importieren!
