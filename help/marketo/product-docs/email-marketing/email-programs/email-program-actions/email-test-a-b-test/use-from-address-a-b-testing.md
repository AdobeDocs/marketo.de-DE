---
unique-page-id: 2359504
description: Erfahren Sie, wie Sie A/B-Tests von Adressen aus ausführen. Testen Sie verschiedene Absenderadressen und wählen Sie einen Gewinner nach Leistung aus.
title: Verwenden von A/B-Tests des Typs „Absenderadresse“
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/rerG-Wyn1X53QQBDXFwyg74uEOznGcYcBis9EwX4vQU'
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
source-wordcount: '277'
ht-degree: 2%
---
# A/B[!UICONTROL Tests &quot;]&quot; verwenden {#use-from-address-a-b-testing}

Sie können Ihre E-Mails einfach mit A/B-Tests überprüfen. Ein interessanter Test ist der **[!UICONTROL Von Adresse]** Test. So richten Sie es ein.

>[!PREREQUISITES]
>
>[Hinzufügen eines A/B-Tests](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicken Sie unter **[!UICONTROL Kachel]** E-Mail“ bei ausgewählter E-Mail auf **[!UICONTROL A/B-Test hinzufügen]**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ein neues Fenster wird geöffnet. Wählen Sie **[!UICONTROL Absenderadresse]** für **[!UICONTROL Testtyp]**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Wenn Sie über frühere Testinformationen verfügen (z. B. einen Betrefftest), können Sie sicher auf „Test **[!UICONTROL &quot;]**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Geben Sie die zweite **[!UICONTROL Absenderadresse]** ein, die Sie testen möchten.

   >[!NOTE]
   >
   >Bei Auswahl A werden die in der ausgewählten E-Mail enthaltenen Informationen vorab ausgefüllt.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Sie können auf das **+** klicken, um beliebig viele Absenderadressen hinzuzufügen.

1. Wählen Sie mit dem Schieberegler den gewünschten Prozentsatz der Zielgruppe für Ihren A/B-Test aus und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Die verschiedenen Varianten senden an gleiche Teile der ausgewählten Testprobengröße.

   >[!CAUTION]
   >
   >**Es wird empfohlen, die Stichprobengröße nicht auf 100 % festzulegen**. Wenn Sie eine statische Liste verwenden, wird bei Festlegung der Stichprobengröße auf 100 % die E-Mail an alle Personen in der Zielgruppe gesendet und der Gewinner erhält niemanden. Wenn Sie eine **Smart**-Liste verwenden, wird bei einer Stichprobengröße von 100 % die E-Mail an alle Personen in der Zielgruppe _zu diesem Zeitpunkt_ gesendet. Wenn das E-Mail-Programm zu einem späteren Zeitpunkt erneut ausgeführt wird, erhalten alle neuen Personen, die sich für die Smart-Liste qualifizieren, ebenfalls die E-Mail, da sie nun in der Zielgruppe enthalten sind.

   Ok, wir sind fast da. Jetzt müssen wir [die A/B-Testsieger-Kriterien definieren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
