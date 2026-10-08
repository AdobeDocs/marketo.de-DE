---
unique-page-id: 2359494
description: Erfahren Sie, wie Sie Betreffzeilen-A/B-Tests in E-Mail-Programmen ausführen. Testen Sie verschiedene Betreffzeilen und wählen Sie einen Gewinner nach Leistung.
title: Verwenden von A/B-Tests nach Betreffzeile
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/jF6mldDXXbl9YOWTOfwgvxvbh-QmIH6sqnnELOv1lxQ'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: 69a7f8d6-582c-5b66-841e-32cf07fd164c
    internal-label: A/B Testing
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: c0f0afc1-a5a8-4b01-8b43-cc38f9169499
    internal-label: Email programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 4%
---
# Verwenden von A/B-Tests des Typs „Betreffzeile“ {#use-subject-line-a-b-testing}

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
