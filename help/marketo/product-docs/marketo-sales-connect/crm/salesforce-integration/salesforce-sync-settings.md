---
unique-page-id: 18317669
description: Salesforce-Synchronisierungseinstellungen - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisationseinstellungen
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 5%

---

# Salesforce-Synchronisationseinstellungen {#salesforce-sync-settings}

## Protokollieren von E-Mail-Aktivitäten in Salesforce über API {#logging-email-activity-to-salesforce-via-api}

Für diese Funktion müssen Sie die Enterprise/Unlimited Edition von Salesforce oder die Professional Edition verwenden, wenn Sie die Integration über die Web Services-API erworben haben.

>[!PREREQUISITES]
>
>Salesforce und Sales Connect müssen verbunden sein.

1. Klicken Sie in Sales Connect oben rechts auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one-2.png)

1. Klicken Sie unter Mein Konto (Administratoreinstellungen, wenn Sie Administrator sind) auf **Salesforce**.

   ![](assets/two-2.png)

1. Klicken Sie auf die **Synchronisierungseinstellungen**.

   ![](assets/three-1.png)

1. Klicken Sie auf den Pfeil neben E-Mail-Aktivität in Salesforce protokollieren .

   ![](assets/four-1.png)

1. Klicken Sie auf die Registerkarte **Salesforce** API. Auf dieser Karte können Sie Ihre Voreinstellungen für die Protokollierung von Informationen in Salesforce festlegen. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/five.png)

## Protokollieren von E-Mail-Aktivitäten in Salesforce per E-Mail an Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Sobald Sie „E-Mail an Salesforce (BCC)“ aktiviert haben, erhalten Sie eine BCC Ihrer Verkaufs-E-Mails und Ihre E-Mails werden als Aktivitäten zu Opportunitys, Leads und Kontakten protokolliert.

>[!PREREQUISITES]
>
>Salesforce und Sales Connect müssen verbunden sein.

**So protokollieren Sie Ihre E-Mails in Salesforce per E-Mail (BCC)**

1. Klicken Sie in Sales Connect oben rechts auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one-3.png)

1. Klicken Sie unter Mein Konto (Administratoreinstellungen, wenn Sie Administrator sind) auf **Salesforce**.

   ![](assets/two-3.png)

1. Klicken Sie auf die **Synchronisierungseinstellungen**.

   ![](assets/three-1.png)

1. Klicken Sie auf **Registerkarte E-Mail an Salesforce (BCC** und klicken Sie auf **Aktivieren**.

   ![](assets/six-2.png)

Wenn Ihre E-Mail-Adresse an Salesforce aus irgendeinem Grund nicht abgerufen werden kann, führen Sie die folgenden Schritte aus, um die BCC-Funktion in Ihrem Salesforce-Konto zu aktivieren:

1. Melden Sie sich bei Ihrer Salesforce-Instanz an.
1. Suchen Sie Ihren Benutzernamen in der oberen rechten Ecke und wählen Sie die Dropdown-Leiste aus.
1. Wählen Sie **Meine Einstellungen** aus.
1. Wählen Sie **E-Mail** aus.
1. Wählen Sie **Meine E-Mail an Salesforce** aus.
1. Auf dieser Seite wird ein Feld mit der Bezeichnung „E-Mail an Salesforce-Adresse“ angezeigt. Wenn daneben nichts ausgefüllt ist, scrollen Sie nach unten zu „Meine akzeptablen E-Mail-Adressen“.
1. Geben Sie die E-Mail-Adresse(n) ein, die BCC speichern soll(en).
1. Klicken Sie **Änderungen speichern**.

**Meine E-Mail an Salesforce kann in meinen Einstellungen nicht gefunden werden**

Wenn Meine E-Mail an Salesforce in Ihren Einstellungen nicht angezeigt wird, hat Ihr Administrator sie möglicherweise nicht aktiviert. Dies kann vorkommen, wenn Ihr Team mit Salesforce noch nicht vertraut ist oder die von Salesforce bereitgestellte BCC-Adresse noch nie verwendet hat.

>[!NOTE]
>
>Sie benötigen Administratorrechte, um dies einzurichten.

1. Klicken Sie **Setup**.
1. Klicken Sie auf **E-Mail-Administration**.
1. Klicken Sie **E-Mail an Salesforce**.
1. Klicken Sie auf **Bearbeiten**.
1. Aktivieren Sie das Kontrollkästchen neben „Aktiv“.
1. Klicken Sie auf **Speichern**.

## Aufgaben von Sales Connect/Wiedervorlagen für Salesforce-Aufgaben synchronisieren {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Klicken Sie oben rechts auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/one-3.png)

1. Klicken Sie unter Mein Konto (Administratoreinstellungen, wenn Sie Administrator sind) auf **Salesforce**.

   ![](assets/two-2.png)

1. Klicken Sie auf die **Synchronisierungseinstellungen**.

   ![](assets/three-1.png)

1. Klicken Sie auf den Pfeil neben Aufgaben/Erinnerungen mit Salesforce synchronisieren .

   ![](assets/seven-2.png)

1. Wählen Sie die gewünschte Option aus (standardmäßig „Mit Salesforce-Aufgaben nicht synchronisieren“ ausgewählt).

   ![](assets/eight.png)
