---
unique-page-id: 2359520
description: Verwenden von "Datum/Uhrzeit"-A/B-Tests - Marketo-Dokumente - Produktdokumentation
title: Verwenden von A/B-Tests "Datum/Uhrzeit"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Verwenden von A/B-Tests &quot;Datum/Uhrzeit&quot; {#use-date-time-a-b-testing}

Sie können Ihre E-Mails einfach per A/B-Test testen. Ein Test ist der Test **Datum/Uhrzeit** . Dadurch wird getestet, zu welcher Tageszeit oder an welchem Wochentag E-Mails am besten gesendet werden. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. Klicken Sie unter der Kachel **E-Mail** auf **A/B-Test hinzufügen**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **Datum/Uhrzeit** für **Testtyp** aus.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Wenn Sie über vorherige Testinformationen verfügen (z. B. über einen Betrefftest), können Sie sicher auf **Test zurücksetzen** klicken.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Wählen Sie das Datum für Ihr erstes Datum/Ihre erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Wählen Sie die Zeit für Ihr erstes Datum/Ihre erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Wiederholen Sie den Vorgang für das zweite Datum/die zweite Uhrzeit.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Verwenden Sie den Schieberegler, um festzulegen, welcher Prozentsatz der Zielgruppe Sie in Ihrem A/B-Test verwenden möchten, und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten gelten für gleiche Teile der ausgewählten Teststichprobengröße.

   >[!CAUTION]
   >
   >**Wir empfehlen, die Stichprobengröße nicht auf 100 %** festzulegen. Wenn Sie eine statische Liste verwenden, sendet die Einstellung der Stichprobengröße auf 100 % die E-Mail an alle Benutzer der Zielgruppe und der Gewinner an niemanden. Wenn Sie eine **intelligente** Liste verwenden, sendet die Einstellung der Stichprobengröße auf 100 % die E-Mail an jeden in der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten auch alle neuen Personen, die sich für die Smart-Liste qualifizieren, die E-Mail, da sie jetzt in der Audience enthalten sind.

   Okay, wir sind einen Schritt näher. Jetzt müssen wir [die Kriterien für den A/B-Test-Gewinner definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
