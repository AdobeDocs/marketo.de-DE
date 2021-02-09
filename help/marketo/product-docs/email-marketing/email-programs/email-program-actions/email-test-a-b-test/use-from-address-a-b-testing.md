---
unique-page-id: 2359504
description: A/B-Tests mit "Von Adresse" - Marketing-Dokumentation - Produktdokumentation
title: A/B-Tests mit "Von Adresse"verwenden
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---


# &quot;Von Adresse&quot; A/B-Tests verwenden {#use-from-address-a-b-testing}

Sie können Ihre E-Mails ganz einfach A/B testen. Ein interessanter Test ist der **From Address**-Test. So richten Sie es ein:

>[!PREREQUISITES]
>
>[hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter der Kachel **E-Mail** mit ausgewählter E-Mail auf **Hinzufügen A/B-Test**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **Aus Adresse** für **Testtyp**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Wenn Sie bereits über vorherige Testinformationen verfügen (z. B. einen Betreff-Test), können Sie sicher auf **Test zurücksetzen** klicken.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Geben Sie die zweiten **Informationen aus der Adresse** ein, die Sie testen möchten.

   >[!NOTE]
   >
   >Auswahl A füllt die in der ausgewählten E-Mail enthaltenen Informationen vorab aus.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Sie können auf **+** klicken, um so viele Von Adressen hinzuzufügen, wie Sie möchten.

1. Verwenden Sie den Schieberegler, um den Prozentwert der Audience auszuwählen, die Sie im A/B-Test verwenden möchten, und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten werden an gleiche Teile der ausgewählten Stichprobengröße gesendet.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100%** festzulegen. Wenn Sie eine statische Liste verwenden, wird bei einer Stichprobengröße von 100 % die E-Mail an alle Benutzer in der Audience gesendet und der Gewinner erhält niemanden. Wenn Sie eine **smart**-Liste verwenden, wird bei einer Stichprobengröße von 100 % die E-Mail an alle Benutzer in der Audience _zu diesem Zeitpunkt_ gesendet. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die intelligente Liste qualifizieren, ebenfalls die E-Mail, da sie jetzt in der Audience enthalten sind.

   OK, wir sind fast da. Jetzt müssen wir [die Kriterien für den Gewinner des A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md) definieren.
