---
unique-page-id: 2359520
description: Verwenden von "Datum/Uhrzeit"-A/B-Tests - Marketo-Dokumente - Produktdokumentation
title: Verwenden von A/B-Tests "Datum/Uhrzeit"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Verwenden von A/B-Tests &quot;Datum/Uhrzeit&quot; {#use-date-time-a-b-testing}

Sie können Ihre E-Mails einfach per A/B-Test testen. Ein Test ist **Datum/Uhrzeit** Test. Dadurch wird getestet, welche Tageszeit oder welcher Wochentag für den Versand von E-Mails am besten geeignet ist. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. Unter dem **Email** tile, click **A/B-Test hinzufügen**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Ein neues Fenster wird geöffnet. Auswählen **Datum/Uhrzeit** für **Testtyp**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Wenn Sie über vorherige Testinformationen verfügen (z. B. über einen Betrefftest), können Sie sicher auf **Test zurücksetzen**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Wählen Sie das Datum für Ihr erstes Datum/Ihre erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Wählen Sie die Zeit für Ihr erstes Datum/Ihre erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Wiederholen Sie den Vorgang für das zweite Datum/die zweite Uhrzeit.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Wählen Sie mit dem Schieberegler den Prozentsatz der Audience aus, den Sie für Ihren A/B-Test verwenden möchten, und klicken Sie auf **Nächste**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten gelten für gleiche Teile der ausgewählten Teststichprobengröße.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, sendet die Einstellung der Stichprobengröße auf 100 % die E-Mail an alle Benutzer der Zielgruppe und der Gewinner an niemanden. Wenn Sie eine **smart** Liste, bei der die Stichprobengröße auf 100 % gesetzt wird, sendet die E-Mail an alle Benutzer der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten auch alle neuen Personen, die sich für die Smart-Liste qualifizieren, die E-Mail, da sie jetzt in der Audience enthalten sind.

   Okay, wir sind einen Schritt näher. Jetzt müssen wir [Definieren der Kriterien für den A/B-Test-Gewinner](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
