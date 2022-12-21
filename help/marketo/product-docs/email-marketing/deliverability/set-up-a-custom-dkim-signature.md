---
unique-page-id: 2360219
description: Einrichten einer benutzerdefinierten DKIM-Signatur - Marketo Docs - Produktdokumentation
title: Einrichten einer benutzerdefinierten DKIM-Signatur
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Einrichten einer benutzerdefinierten DKIM-Signatur {#set-up-a-custom-dkim-signature}

Um die Zustellbarkeit auf höchstem Niveau zu gewährleisten, signieren wir automatisch alle ausgehenden E-Mails mit einer freigegebenen Marketo DKIM-Signatur.

>[!NOTE]
>
>Möglicherweise benötigen Sie die Hilfe Ihres IT-Teams, um einige der Schritte in diesem Artikel durchzuführen.

Sie können die DKIM-Signatur personalisieren, um die Domäne(n) Ihrer Wahl widerzuspiegeln. So geht es.

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >Wenn Sie eine benutzerdefinierte DKIM-Signatur auf die altmodische Art einrichten, funktioniert sie weiterhin und sollte hier angezeigt werden.

1. Klicken **Email**, dann **DKIM** und schließlich **Domäne hinzufügen**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Geben Sie die Domäne ein, die Sie in Marketo-E-Mails als Absenderadresse verwenden möchten, und klicken Sie auf **Hinzufügen**.

   >[!TIP]
   >
   >Wenn Sie eine andere Domäne in Ihrer Absenderadresse verwenden, verwenden wir die von Marketo freigegebene DKIM-Signatur.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Senden Sie die **Hostdatensatz** und **TXT-Wert** zu Ihrer IT hinzufügen. Bitten Sie sie, den Datensatz für Sie zu erstellen und sicherzustellen, dass er an alle Nameserver propagiert wird, die mit der von -Domäne verknüpft sind. Die DKIM-Verifizierung von Marketo erfordert, dass der DKIM-Schlüssel an alle Nameserver weitergegeben wird, die mit der Domäne verknüpft sind, die von DKIM signiert wurde.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Nachdem er bestätigt hat, dass er den Datensatz erstellt hat, kehren Sie zu Marketo zurück, wählen Sie Ihre Domäne aus und klicken Sie auf **DNS überprüfen**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >Wenn die Bestätigung fehlschlägt und Ihre IT-Abteilung den Datensatz korrekt erstellt hat, kann es sich um eine DNS-Weiterleitung handeln. Versuchen Sie es später erneut.

   >[!CAUTION]
   >
   >Das Ändern/Entfernen des entsprechenden DNS-Eintrags beeinträchtigt die Zustellbarkeit. Löschen Sie den Eintrag in Marketo, bevor Sie DNS-Änderungen vornehmen.

   Dies hilft bei der Zustellbarkeit Ihrer E-Mail. Sie sollten die Validierung erhalten, dass der Datensatz vorhanden ist und korrekt ist.
