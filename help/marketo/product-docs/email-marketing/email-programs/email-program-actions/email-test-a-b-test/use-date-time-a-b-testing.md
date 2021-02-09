---
unique-page-id: 2359520
description: '"Datum/Uhrzeit" A/B-Test - Marketing Docs - Produktdokumentation'
title: Verwendung von "Datum/Uhrzeit" A/B-Tests
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---


# &quot;Datum/Uhrzeit&quot; A/B-Tests verwenden {#use-date-time-a-b-testing}

Sie können Ihre E-Mails ganz einfach A/B testen. Ein Test ist der **Date/Time**-Test. Dadurch wird getestet, zu welcher Tageszeit oder an welchem Wochentag E-Mails am besten gesendet werden. So richten Sie es ein:

>[!PREREQUISITES]
>
>[hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)


1. Klicken Sie unter der Kachel **E-Mail** auf **Hinzufügen A/B-Test**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **Datum/Uhrzeit** für **Testtyp**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Wenn Sie bereits über vorherige Testinformationen verfügen (z. B. einen Betreff-Test), können Sie sicher auf **Test zurücksetzen** klicken.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Wählen Sie das Datum für das erste Datum/die erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Wählen Sie die Zeit für das erste Datum/die erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Dasselbe gilt für das zweite Datum/die zweite Uhrzeit.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Verwenden Sie den Schieberegler, um den Prozentwert der Audience auszuwählen, die Sie im A/B-Test verwenden möchten, und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten gelten für gleiche Teile der ausgewählten Stichprobengröße.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100%** festzulegen. Wenn Sie eine statische Liste verwenden, wird bei einer Stichprobengröße von 100 % die E-Mail an alle Benutzer in der Audience gesendet und der Gewinner erhält niemanden. Wenn Sie eine **smart**-Liste verwenden, wird bei einer Stichprobengröße von 100 % die E-Mail an alle Benutzer in der Audience _zu diesem Zeitpunkt_ gesendet. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die intelligente Liste qualifizieren, ebenfalls die E-Mail, da sie jetzt in der Audience enthalten sind.

   Okay, wir sind einen Schritt näher. Jetzt müssen wir [die Kriterien für den Gewinner des A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md) definieren.
