---
unique-page-id: 1147340
description: Senden von E-Mails vom Lead-Inhaber - Marketo-Dokumente - Produktdokumentation
title: Senden von E-Mails von der Lead-Inhaberin bzw. dem Lead-Inhaber
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 7%

---

# Senden von E-Mails von der Lead-Inhaberin bzw. dem Lead-Inhaber {#send-emails-from-the-lead-owner}

Was passiert, wenn Sie eine E-Mail an einen Lead im Namen des Lead-Inhabers senden möchten?  Und so geht das.

1. Suchen Sie Ihre E-Mail, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/one.png)

1. Klicken Sie in das Feld **[!UICONTROL Von]** (Löschen eines vorhandenen Namens) und klicken Sie auf die Schaltfläche **Token einfügen**.

   ![](assets/two.png)

1. Beginnen Sie mit der Eingabe von &quot;`{{lead.Lead Owner`&quot; und wählen Sie das **`{{lead.Lead Owner First Name}}`** Token aus.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Geben Sie einen Standardwert ein, falls der Lead noch keinen Lead-Inhaber hat, und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Klicken Sie nach dem ersten Token, fügen Sie ein Leerzeichen hinzu und klicken Sie dann auf die Schaltfläche **Token einfügen**.

   ![](assets/five.png)

1. Beginnen Sie mit der Eingabe von &quot;`{{lead.Lead Owner`&quot; und wählen Sie das **`{{lead.Lead Owner Last Name}}`** Token aus.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Geben Sie einen Standardwert ein, falls der Lead noch keinen Lead-Inhaber hat, und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Stellen Sie sicher, dass Sie ein Leerzeichen zwischen dem Vor- und Nachnamen-Token hinzugefügt haben.

1. Klicken Sie in das Feld **[!UICONTROL Absenderadresse]** (löschen Sie eine vorhandene E-Mail-Adresse) und klicken Sie auf die Schaltfläche **Token einfügen**.

   ![](assets/eight.png)

1. Beginnen Sie mit der Eingabe von &quot;`{{lead.Lead Owner`&quot; und wählen Sie das **`{{lead.Lead Owner Email Address}}`** Token aus.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Geben Sie einen Standardwert ein, falls der Lead noch keinen Lead-Inhaber hat, und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/ten.png)

1. Stellen Sie sicher **[!UICONTROL dass die Felder]** Antwort an **[!UICONTROL und]** Betreff“ ausgefüllt sind und Sie fertig sind!

   ![](assets/eleven.png)
