---
unique-page-id: 1900597
description: Definieren einer Audience durch Importieren einer Liste - Marketing Docs - Produktdokumentation
title: Definieren einer Audience durch Importieren einer Liste
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Definieren einer Audience durch Importieren einer Liste {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[E-Mail für ein E-Mail-Programm erstellen](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Nachdem Sie ein E-Mail-Programm erstellt haben, möchten Sie ihm mitteilen, an wen Sie die E-Mail senden möchten. Dazu [erstellen Sie eine intelligente Liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) oder importieren eine Liste. Hier ist, wie man das durch Importieren einer Liste erreicht.

>[!NOTE]
>
>Die Definition Ihrer Audience funktioniert nur, wenn das E-Mail-Programm nicht genehmigt wurde.
>
>Alle importierten Datums-/Uhrzeitfelder werden als &quot;Central Time&quot;behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (Amerika/Chicago) umzuwandeln.

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-1.png)

   Wählen Sie Ihr E-Mail-Programm aus und klicken Sie dann auf Liste importieren unter der Kachel Audience.
   ![](assets/importlist.png)

1. Das Fenster zum Importieren der Liste wird geöffnet. Klicken Sie auf **Durchsuchen** und wählen Sie die zu importierende Datei aus. Nachdem Sie die Liste der Personen ausgewählt haben, klicken Sie auf Weiter.
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Vergewissern Sie sich, dass die Liste UTF-8, UTF-16, Shift-JIS oder EUC-JP kodiert ist und die Dateigröße 50 MB nicht überschreitet.

   Vergewissern Sie sich, dass die Felder in Ihrer Datei korrekt zugeordnet sind, und klicken Sie auf Weiter.
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo wird sich die Zuordnungen für zukünftige Importe merken!

1. Geben Sie einen **Namen** für Ihre Liste ein und klicken Sie auf **Importieren**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Sobald der Import abgeschlossen ist, kehren Sie zur Registerkarte &quot;Haupt-Programm&quot;zurück. Du wirst sehen, wie viele Leute dich qualifizieren werden.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definition**
>
>Haben Sie die Blocknummer bemerkt? Diese Zahl ist eine Untergruppe der qualifizierten Personen und repräsentiert Personen, die diese E-Mail nicht senden können, weil sie:
>
>* Nicht abonniert
>* Marketing ausgesetzt
>* Auf die Blockierungsliste gesetzt
>* Email ungültig
>* Leere E-Mail

>
>
Klicken Sie auf die Nummer für eine detaillierte Liste der Personen, die von Postings gesperrt sind.
>
>Verwenden Sie die Schaltfläche ![—](assets/image2014-10-23-16-3a32-3a36-1.png) auf der Kachel &quot; **Audience** &quot;, um zu sehen, wie viele Personen aufgrund der Kriterien für intelligente Liste für den Empfang der E-Mail qualifiziert sind. Ziehen Sie die blockierte Zahl von der Anzahl der Personen ab, um die Gesamtanzahl der Personen zu erhalten, die die E-Mail erhalten.

>[!TIP]
>
>Sie müssen nicht warten, bis der Import der Liste abgeschlossen ist. Du kannst weiterarbeiten, wenn du willst.

Fantastisch! Jetzt ist es an der Zeit, eine bereits vorhandene E-Mail auszuwählen oder eine neue E-Mail zu erstellen, die an diese Personen gesendet werden soll.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Vorhandene E-Mail auswählen](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [E-Mail für ein E-Mail-Programm erstellen](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



