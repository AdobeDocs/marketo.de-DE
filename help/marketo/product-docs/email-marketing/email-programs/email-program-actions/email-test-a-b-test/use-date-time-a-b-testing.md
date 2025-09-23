---
unique-page-id: 2359520
description: Verwenden von „Datum/Uhrzeit“-A/B-Tests - Marketo-Dokumente - Produktdokumentation
title: Verwenden von A/B-Tests nach Datum/Uhrzeit
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 4%

---

# Verwenden von A/B-Tests nach Datum/Uhrzeit {#use-date-time-a-b-testing}

Sie können Ihre E-Mails einfach mit A/B-Tests überprüfen. Ein Test ist der **[!UICONTROL Datum/Uhrzeit]**-Test. Dadurch wird getestet, zu welcher Tageszeit oder an welchem Wochentag E-Mails am besten gesendet werden. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. Klicken Sie unter **[!UICONTROL Kachel]** E-Mail“ auf **[!UICONTROL A/B-Test hinzufügen]**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **[!UICONTROL Datum/Uhrzeit]** für **[!UICONTROL Testtyp]** aus.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Wenn Sie über frühere Testinformationen verfügen (z. B. einen Betrefftest), können Sie sicher auf „Test **[!UICONTROL &quot;]**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Wählen Sie das Datum für Ihr erstes Datum/Ihre erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Wählen Sie die Uhrzeit für Ihr erstes Datum/Ihre erste Uhrzeit aus.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Tun Sie dasselbe für Ihr zweites Datum/Ihre zweite Uhrzeit.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Wählen Sie mit dem Schieberegler den gewünschten Prozentsatz der Zielgruppe für Ihren A/B-Test aus und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten gelten für gleiche Teile der gewählten Stichprobengröße.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, wird bei Festlegung der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe gesendet und der Gewinner erhält niemanden. Wenn Sie eine **Smart**-Liste verwenden, wird beim Festlegen der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe _zu diesem Zeitpunkt_. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die Smart-Liste qualifizieren, ebenfalls die E-Mail, da sie nun in der Zielgruppe enthalten sind.

   Okay, wir sind einen Schritt näher dran. Jetzt müssen wir [die A/B-Testsieger-Kriterien definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
