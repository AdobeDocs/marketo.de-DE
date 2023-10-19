---
unique-page-id: 2360219
description: Einrichten einer benutzerdefinierten DKIM-Signatur - Marketo Docs - Produktdokumentation
title: Einrichten einer benutzerdefinierten DKIM-Signatur
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 9e731fa02cd20b34f48c7f85241b97f4c507d4a9
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 1%

---

# Einrichten einer benutzerdefinierten DKIM-Signatur {#set-up-a-custom-dkim-signature}

Um die Zustellbarkeit auf höchstem Niveau zu gewährleisten, signieren wir automatisch alle ausgehenden E-Mails mit einer freigegebenen Marketo DKIM-Signatur.

>[!NOTE]
>
>Möglicherweise benötigen Sie die Hilfe Ihres IT-Teams, um einige der Schritte in diesem Artikel durchzuführen.

Sie können die DKIM-Signatur personalisieren, um die Domäne(n) Ihrer Wahl widerzuspiegeln. So geht es.

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Wenn Sie eine benutzerdefinierte DKIM-Signatur auf die altmodische Art einrichten, funktioniert sie weiterhin und sollte hier angezeigt werden.

1. Klicks **Email**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Klicken Sie auf die **SPF/DKIM** tab, dann **Domäne hinzufügen**.

![](assets/set-up-a-custom-dkim-signature-3.png)

1. Geben Sie die Domäne ein, die Sie in Marketo-E-Mails als Absenderadresse verwenden werden. Wählen Sie einen Selektor und eine Schlüsselgröße. Klicks **Hinzufügen** wann geschehen.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   >[!TIP]
   >
   >* Wir empfehlen eine Schlüsselgröße von 2048.
   >* Wenn Sie eine andere Domäne in Ihrer Absenderadresse verwenden, verwenden wir die von Marketo freigegebene DKIM-Signatur.

1. Senden Sie die **Hostdatensatz** und **TXT-Wert** zu Ihrer IT hinzufügen. Bitten Sie sie, den Datensatz für Sie zu erstellen und sicherzustellen, dass er an alle Nameserver propagiert wird, die mit der von -Domäne verknüpft sind. Die DKIM-Verifizierung von Marketo erfordert, dass der DKIM-Schlüssel an alle Nameserver weitergegeben wird, die mit der Domäne verknüpft sind, die von DKIM signiert wurde.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Nachdem er bestätigt hat, dass er den Datensatz erstellt hat, kehren Sie zu Marketo zurück, wählen Sie Ihre Domäne aus und klicken Sie auf **DNS überprüfen**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Wenn die Bestätigung fehlschlägt und Ihre IT-Abteilung den Datensatz korrekt erstellt hat, kann es sich um eine DNS-Weiterleitung handeln. Versuchen Sie es später erneut.

   >[!CAUTION]
   >
   >Das Ändern/Entfernen des entsprechenden DNS-Eintrags beeinträchtigt die Zustellbarkeit. Löschen Sie den Eintrag in Marketo, bevor Sie DNS-Änderungen vornehmen.

   Dies hilft bei der Zustellbarkeit Ihrer E-Mail. Sie sollten die Validierung erhalten, dass der Datensatz vorhanden ist und korrekt ist.
