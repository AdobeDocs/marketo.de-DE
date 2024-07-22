---
unique-page-id: 2359494
description: Verwenden von A/B-Tests mit "Betreffzeile"- Marketo-Dokumente - Produktdokumentation
title: A/B-Tests mit "Betreffzeile"verwenden
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# A/B-Tests mit &quot;Betreffzeile&quot;verwenden {#use-subject-line-a-b-testing}

Sie können Ihre E-Mails einfach per A/B-Test testen. Einer der häufigsten Tests ist der Test **Betreffzeile** .

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter der Kachel E-Mail mit ausgewählter E-Mail auf A/B-Test hinzufügen .

![](assets/image2014-9-12-15-3a6-3a2.png)

1. Daraufhin wird das Fenster des Testeditors geöffnet. Geben Sie eine oder mehrere neue Betreffzeilen ein.

   >[!NOTE]
   >
   >Auswahl **A** füllt die in der ausgewählten E-Mail enthaltenen Informationen vorab.

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >Sie können auf **+** klicken, um weitere Betreffzeilen hinzuzufügen.

1. Verwenden Sie den Schieberegler, um festzulegen, welcher Prozentsatz der Zielgruppe Sie Ihren A/B-Test erhalten möchten, und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**Wir empfehlen, die Stichprobengröße nicht auf 100 %** festzulegen. Wenn Sie eine statische Liste verwenden, würde die Einstellung der Stichprobengröße auf 100 % dazu führen, dass die E-Mail an alle Benutzer der Zielgruppe gesendet wird und der Gewinner an niemanden weitergeleitet wird. Wenn Sie eine intelligente Liste verwenden, würde die Einstellung der Stichprobengröße auf 100 % die E-Mail an jeden in der Audience senden _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten auch alle neuen Personen, die sich für die intelligente Liste qualifizieren, die E-Mail, da sie nun in der Audience enthalten sind.

   >[!NOTE]
   >
   >Die unterschiedlichen Themenvarianten nehmen sogar Teile der ausgewählten Teststichprobengröße an.

   Okay, wir sind fast da. Jetzt müssen wir [die Kriterien für den A/B-Test-Gewinner definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
