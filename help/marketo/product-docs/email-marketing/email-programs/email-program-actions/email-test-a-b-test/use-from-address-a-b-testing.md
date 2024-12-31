---
unique-page-id: 2359504
description: Verwenden von A/B-Tests „Von Adresse“ - Marketo-Dokumente - Produktdokumentation
title: A/B-Tests von „Absenderadresse“ verwenden
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# A/B-Tests von „Absenderadresse“ verwenden {#use-from-address-a-b-testing}

Sie können Ihre E-Mails einfach mit A/B-Tests überprüfen. Ein interessanter Test ist der **Von Adresse** Test. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter **Kachel** E-Mail“ bei ausgewählter E-Mail auf **A/B-Test hinzufügen**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **Absenderadresse** für **Testtyp**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Wenn Sie über frühere Testinformationen verfügen (z. B. einen Betrefftest), können Sie sicher auf „Test **&quot;**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Geben Sie die zweite **Absenderadresse** ein, die Sie testen möchten.

   >[!NOTE]
   >
   >Bei Auswahl A werden die in der ausgewählten E-Mail enthaltenen Informationen vorab ausgefüllt.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Sie können auf das **+** klicken, um beliebig viele Absenderadressen hinzuzufügen.

1. Wählen Sie mit dem Schieberegler den gewünschten Prozentsatz der Zielgruppe für Ihren A/B-Test aus und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten senden an gleiche Teile der ausgewählten Testprobengröße.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, wird bei Festlegung der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe gesendet und der Gewinner erhält niemanden. Wenn Sie eine **Smart**-Liste verwenden, wird beim Festlegen der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die Smart-Liste qualifizieren, ebenfalls die E-Mail, da sie nun in der Zielgruppe enthalten sind.

   Ok, wir sind fast da. Jetzt müssen wir [die A/B-Testsieger-Kriterien definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
