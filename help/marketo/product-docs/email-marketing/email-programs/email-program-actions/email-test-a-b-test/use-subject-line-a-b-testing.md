---
unique-page-id: 2359494
description: Verwenden der „Betreffzeile“ von A/B-Tests - Marketo-Dokumente - Produktdokumentation
title: Verwenden von A/B-Tests nach Betreffzeile
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---

# Verwenden von A/B-Tests nach Betreffzeile {#use-subject-line-a-b-testing}

Sie können Ihre E-Mails einfach mit A/B-Tests überprüfen. Einer der häufigsten Tests ist der **[!UICONTROL Betreffzeile]** Test.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter der **[!UICONTROL E-Mail]**-Kachel mit ausgewählter E-Mail auf **[!UICONTROL A/B-Test hinzufügen]**.

![](assets/image2014-9-12-15-3a6-3a2.png)

1. Das Fenster Test-Editor wird geöffnet. Geben Sie eine oder mehrere neue Betreffzeilen ein.

   >[!NOTE]
   >
   >Choice **A** wird vorab mit den in der ausgewählten E-Mail enthaltenen Informationen ausgefüllt.

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >Sie können auf das **+** klicken, um weitere Betreffzeilen hinzuzufügen.

1. Verwenden Sie den Schieberegler, um den Prozentsatz der Zielgruppe auszuwählen, den Sie Ihren A/B-Test erhalten möchten, und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, würde eine Festlegung der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe senden und der Gewinner würde an niemanden gehen. Wenn Sie eine Smart-Liste verwenden, würde eine Einstellung der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe _zu diesem Zeitpunkt_ senden. Und wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die Smart-Liste qualifizieren, ebenfalls die E-Mail, da sie jetzt in der Zielgruppe enthalten sind.

   >[!NOTE]
   >
   >Die verschiedenen Varianten nehmen gerade Teile der ausgewählten Stichprobengröße in Anspruch.

   Okay, wir sind fast da. Jetzt müssen wir [die A/B-Testsieger-Kriterien definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
