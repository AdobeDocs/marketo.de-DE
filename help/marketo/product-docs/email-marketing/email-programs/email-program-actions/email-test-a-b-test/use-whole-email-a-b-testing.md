---
unique-page-id: 2359502
description: Verwenden von A/B-Tests mit "gesamter E-Mail"- Marketo-Dokumente - Produktdokumentation
title: A/B-Tests mit "gesamter E-Mail" verwenden
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# A/B-Tests mit &quot;gesamter E-Mail&quot; verwenden {#use-whole-email-a-b-testing}

Sie können Ihre E-Mails einfach per A/B-Test testen. Ein guter Test ist die **Ganze E-Mail** Test. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter der Kachel E-Mail mit ausgewählter E-Mail auf **A/B-Test hinzufügen**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Ein neues Fenster wird geöffnet. Klicken Sie auf **Testtyp** und wählen Sie **Gesamte E-Mails**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Wenn Sie über vorherige Testinformationen verfügen (z. B. über einen Betrefftest), können Sie sicher auf **Test zurücksetzen**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Wählen Sie Ihre erste E-Mail aus.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Klicks **Hinzufügen** , um die E-Mail anzuwenden.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Sie können mehrere E-Mails hinzufügen. Wenn Sie jedoch zu viele hinzufügen, kann dies den Testprozess verlangsamen.

1. Wählen Sie Ihre zweite E-Mail aus.

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. Klicks **Hinzufügen** um die zweite E-Mail anzuwenden. Ziehen Sie den Schieberegler, um festzulegen, welcher Prozentsatz der Zielgruppe Sie Ihren A/B-Test erhalten möchten, und klicken Sie auf **Nächste**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten werden an gleiche Teile der ausgewählten **Stichprobengröße**.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, sendet die Einstellung der Stichprobengröße auf 100 % die E-Mail an alle Benutzer der Zielgruppe und der Gewinner an niemanden. Wenn Sie eine **smart** Liste, bei der die Stichprobengröße auf 100 % gesetzt wird, sendet die E-Mail an alle Benutzer der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten auch alle neuen Personen, die sich für die Smart-Liste qualifizieren, die E-Mail, da sie jetzt in der Audience enthalten sind.

   Okay, wir sind fast da. Jetzt müssen wir [Definieren der Kriterien für den A/B-Test-Gewinner](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
