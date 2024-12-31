---
unique-page-id: 1147340
description: Senden von E-Mails vom Lead-Inhaber - Marketo-Dokumente - Produktdokumentation
title: Senden von E-Mails vom Lead-Inhaber
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Senden von E-Mails vom Lead-Inhaber {#send-emails-from-the-lead-owner}

Was passiert, wenn Sie eine E-Mail an einen Lead im Namen des Lead-Inhabers senden möchten?  So geht&#39;s.

1. Suchen Sie Ihre E-Mail, wählen Sie sie aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/one.png)

1. Klicken Sie in das Feld **Von** (Löschen eines vorhandenen Namens) und klicken Sie auf die Schaltfläche **Token einfügen**.

   ![](assets/two.png)

1. Beginnen Sie mit der Eingabe von &quot;`{{lead.Lead Owner`&quot; und wählen Sie das **`{{lead.Lead Owner First Name}}`** Token aus.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Geben Sie einen Standardwert ein, falls der Lead noch keinen Lead-Inhaber hat, und klicken Sie auf **Einfügen**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Klicken Sie nach dem ersten Token, fügen Sie ein Leerzeichen hinzu und klicken Sie dann auf die Schaltfläche **Token einfügen**.

   ![](assets/five.png)

1. Beginnen Sie mit der Eingabe von &quot;`{{lead.Lead Owner`&quot; und wählen Sie das **`{{lead.Lead Owner Last Name}}`** Token aus.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Geben Sie einen Standardwert ein, falls der Lead noch keinen Lead-Inhaber hat, und klicken Sie auf **Einfügen**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie ein Leerzeichen zwischen dem Vor- und Nachnamen-Token hinzugefügt haben.

1. Klicken Sie in das Feld Von E-Mail (löschen Sie eine vorhandene E-Mail-Adresse) und klicken Sie auf die Schaltfläche Token einfügen .

   ![](assets/eight.png)

1. Beginnen Sie mit der Eingabe von &quot;`{{lead.Lead Owner`&quot; und wählen Sie das **`{{lead.Lead Owner Email Address}}`** Token aus.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Geben Sie einen Standardwert ein, falls der Lead noch keinen Lead-Inhaber hat, und klicken Sie auf **Einfügen**.

   ![](assets/ten.png)

1. Stellen Sie sicher **dass die Felder** Antwort an **und** Betreff“ ausgefüllt sind und Sie fertig sind!

   ![](assets/eleven.png)
