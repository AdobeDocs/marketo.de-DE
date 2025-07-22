---
unique-page-id: 18317669
description: Salesforce-Synchronisierungseinstellungen - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisationseinstellungen
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---

# Salesforce-Synchronisationseinstellungen {#salesforce-sync-settings}

## Protokollieren von E-Mail-Aktivitäten in Salesforce über API {#logging-email-activity-to-salesforce-via-api}

Für diese Funktion müssen Sie die Enterprise/Unlimited Edition von Salesforce oder die Professional Edition verwenden, wenn Sie die Integration über die Web Services-API erworben haben.

>[!PREREQUISITES]
>
>Salesforce und Sales Connect müssen verbunden sein.

1. Klicken Sie [!DNL Sales Connect] oben rechts auf das Zahnradsymbol und dann auf **[!UICONTROL Einstellungen]**.

   ![](assets/one-2.png)

1. Klicken Sie unter [!UICONTROL Mein Konto] ([!UICONTROL Admin-Einstellungen] wenn Sie Administrator sind) auf **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Klicken Sie auf die **[!UICONTROL Synchronisierungseinstellungen]**.

   ![](assets/three-1.png)

1. Klicken Sie auf den Pfeil neben E-Mail-Aktivität in [!DNL Salesforce] protokollieren.

   ![](assets/four-1.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Salesforce]** API. Auf dieser Karte können Sie festlegen, wie Sie Informationen in [!DNL Salesforce] protokollieren möchten. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/five.png)

## Protokollieren von E-Mail-Aktivitäten in Salesforce per E-Mail an Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Sobald Sie „E-Mail an Salesforce (BCC)“ aktiviert haben, erhalten Sie eine BCC Ihrer Verkaufs-E-Mails und Ihre E-Mails werden als Aktivitäten zu Opportunitys, Leads und Kontakten protokolliert.

>[!PREREQUISITES]
>
>[!DNL Salesforce] und [!DNL Sales Connect] müssen verbunden sein.

**So protokollieren Sie Ihre E-Mails in Salesforce per E-Mail (BCC)**

1. Klicken Sie [!UICONTROL Sales Connect] oben rechts auf das Zahnradsymbol und wählen Sie &quot;**[!UICONTROL &quot;]**.

   ![](assets/one-3.png)

1. Klicken Sie unter [!UICONTROL Mein Konto] ([!UICONTROL Admin-Einstellungen] wenn Sie Administrator sind) auf **[!UICONTROL Salesforce]**.

   ![](assets/two-3.png)

1. Klicken Sie auf die **[!UICONTROL Synchronisierungseinstellungen]**.

   ![](assets/three-1.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte E-Mail an Salesforce (BCC]** und klicken Sie auf **[!UICONTROL Aktivieren]**.

   ![](assets/six-2.png)

Wenn Ihre E-Mail-Adresse aus irgendeinem Grund nicht [!DNL Salesforce] wird, führen Sie die folgenden Schritte aus, um die BCC-Funktion in Ihrem [!DNL Salesforce]-Konto zu aktivieren:

1. Melden Sie sich bei Ihrer [!DNL Salesforce] an.
1. Suchen Sie Ihren Benutzernamen in der oberen rechten Ecke und wählen Sie die Dropdown-Leiste aus.
1. Wählen Sie **[!UICONTROL Meine Einstellungen]** aus.
1. Wählen Sie **[!UICONTROL E-Mail]** aus.
1. Wählen Sie **[!UICONTROL Meine E-Mail an Salesforce]** aus.
1. Auf dieser Seite wird ein Feld mit der Bezeichnung „E-Mail an Salesforce-Adresse“ angezeigt. Wenn daneben nichts ausgefüllt ist, scrollen Sie nach unten zu „Meine akzeptablen E-Mail-Adressen“.
1. Geben Sie die E-Mail-Adresse(n) ein, die BCC speichern soll(en).
1. Klicken Sie **[!UICONTROL Änderungen speichern]**.

**Meine zu [!DNL Salesforce] E-Mail kann in meinen Einstellungen nicht gefunden werden**

Wenn Meine E-Mail an Salesforce in Ihren Einstellungen nicht angezeigt wird, hat Ihr Administrator sie möglicherweise nicht aktiviert. Dies kann vorkommen, wenn Ihr Team mit [!DNL Salesforce] noch nicht vertraut ist oder Ihr Team die von [!DNL Salesforce] bereitgestellte BCC-Adresse noch nie verwendet hat.

>[!NOTE]
>
>Sie benötigen Administratorrechte, um dies einzurichten.

1. Klicken Sie **[!UICONTROL Setup]**.
1. Klicken Sie auf **[!UICONTROL E-Mail-Administration]**.
1. Klicken Sie **[!UICONTROL E-Mail an Salesforce]**.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Aktivieren Sie das Kontrollkästchen neben &quot;[!UICONTROL Aktiv].
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Aufgaben/Erinnerungen mit [!DNL Salesforce] Aufgaben synchronisieren {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Klicken Sie oben rechts auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/one-3.png)

1. Klicken Sie unter [!UICONTROL Mein Konto] ([!UICONTROL Admin-Einstellungen] wenn Sie Administrator sind) auf **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Klicken Sie auf die **[!UICONTROL Synchronisierungseinstellungen]**.

   ![](assets/three-1.png)

1. Klicken Sie auf den Pfeil neben [!UICONTROL Aufgaben/Erinnerungen von Vertriebsmitarbeitern mit Salesforce-Aufgaben synchronisieren].

   ![](assets/seven-2.png)

1. Wählen Sie die gewünschte Option aus ([!UICONTROL Mit Salesforce-Aufgaben nicht synchronisieren] ist standardmäßig ausgewählt).

   ![](assets/eight.png)
