---
unique-page-id: 2359502
description: A/B-Tests in „ganzen E-Mails“ verwenden - Marketo-Dokumente - Produktdokumentation
title: A/B-Tests für ganze E-Mails verwenden
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# A/B-Tests für ganze E-Mails verwenden {#use-whole-email-a-b-testing}

Sie können Ihre E-Mails einfach mit A/B-Tests überprüfen. Ein großartiger Test ist der **Gesamte E-Mail**-Test. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter der Kachel E-Mail mit ausgewählter E-Mail auf **A/B-Test hinzufügen**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Ein neues Fenster wird geöffnet. Klicken Sie auf **Testtyp** und wählen Sie &quot;**E-Mails** aus.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Wenn Sie über frühere Testinformationen verfügen (z. B. einen Betrefftest), können Sie sicher auf „Test **&quot;**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Wählen Sie Ihre erste E-Mail aus.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Klicken Sie auf **Hinzufügen**, um die E-Mail anzuwenden.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Sie können mehrere E-Mails hinzufügen. Wenn Sie jedoch zu viele hinzufügen, kann dies den Testprozess erheblich verlangsamen.

1. Wählen Sie Ihre zweite E-Mail aus.

   [&#128279;](assets/image2014-9-12-15-3a23-3a49.png)

1. Klicken Sie auf **Hinzufügen**, um die zweite E-Mail anzuwenden. Ziehen Sie den Schieberegler, um den Prozentsatz der Zielgruppe auszuwählen, den Sie Ihren A/B-Test erhalten möchten, und klicken Sie auf **Weiter**.

   [&#128279;](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten senden an gleiche Teile der ausgewählten **Testprobengröße**.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, wird bei Festlegung der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe gesendet und der Gewinner erhält niemanden. Wenn Sie eine **Smart**-Liste verwenden, wird beim Festlegen der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die Smart-Liste qualifizieren, ebenfalls die E-Mail, da sie nun in der Zielgruppe enthalten sind.

   Okay, wir sind fast da. Jetzt müssen wir [die A/B-Testsieger-Kriterien definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
