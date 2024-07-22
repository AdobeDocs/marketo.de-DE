---
unique-page-id: 2359504
description: A/B-Tests mit "Von Adresse"verwenden - Marketo-Dokumente - Produktdokumentation
title: A/B-Tests mit "Von Adresse"verwenden
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# A/B-Tests mit &quot;Von Adresse&quot;verwenden {#use-from-address-a-b-testing}

Sie können Ihre E-Mails einfach per A/B-Test testen. Ein interessanter Test ist der Test **Von Adresse** . So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter der Kachel **E-Mail** bei ausgewählter E-Mail auf **A/B-Test hinzufügen** .

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **Von Adresse** für **Testtyp** aus.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Wenn Sie über vorherige Testinformationen verfügen (z. B. über einen Betrefftest), können Sie sicher auf **Test zurücksetzen** klicken.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Geben Sie die zweiten **Von Adresse** Informationen ein, die Sie testen möchten.

   >[!NOTE]
   >
   >Bei Auswahl A werden die in der ausgewählten E-Mail enthaltenen Informationen vorausgefüllt.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Sie können auf **+** klicken, um so viele Von-Adressen hinzuzufügen, wie Sie möchten.

1. Verwenden Sie den Schieberegler, um festzulegen, welcher Prozentsatz der Zielgruppe Sie in Ihrem A/B-Test verwenden möchten, und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten werden an gleiche Teile der ausgewählten Teststichprobengröße gesendet.

   >[!CAUTION]
   >
   >**Wir empfehlen, die Stichprobengröße nicht auf 100 %** festzulegen. Wenn Sie eine statische Liste verwenden, sendet die Einstellung der Stichprobengröße auf 100 % die E-Mail an alle Benutzer der Zielgruppe und der Gewinner an niemanden. Wenn Sie eine **intelligente** Liste verwenden, sendet die Einstellung der Stichprobengröße auf 100 % die E-Mail an jeden in der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten auch alle neuen Personen, die sich für die Smart-Liste qualifizieren, die E-Mail, da sie jetzt in der Audience enthalten sind.

   OK, wir sind fast da. Jetzt müssen wir [die Kriterien für den A/B-Test-Gewinner definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
