---
unique-page-id: 18317669
description: Salesforce-Synchronisierungseinstellungen - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisationseinstellungen
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 4%

---

# Salesforce-Synchronisationseinstellungen {#salesforce-sync-settings}

## Protokollieren von E-Mail-Aktivitäten bei Salesforce über API {#logging-email-activity-to-salesforce-via-api}

Für diese Funktion müssen Sie die Salesforce-Edition (Enterprise/Unlimited Edition) oder die Professional Edition verwenden, wenn Sie die Integration über Web Services API erworben haben.

>[!PREREQUISITES]
>
>Salesforce und Sales Connect müssen verbunden sein.

1. Klicken Sie in Sales Connect auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen** aus.

   ![](assets/one-2.png)

1. Klicken Sie unter &quot;Mein Konto&quot;(Admin-Einstellungen, wenn Sie Administrator sind) auf **Salesforce**.

   ![](assets/two-2.png)

1. Klicken Sie auf die Registerkarte **Einstellungen synchronisieren** .

   ![](assets/three-1.png)

1. Klicken Sie auf den Pfeil neben Protokoll-E-Mail-Aktivität zu Salesforce.

   ![](assets/four-1.png)

1. Klicken Sie auf die Registerkarte **Salesforce API** . Auf dieser Karte können Sie Ihre Voreinstellung für die Protokollierung von Informationen in Salesforce einrichten. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/five.png)

## Protokollieren von E-Mail-Aktivitäten bei Salesforce per E-Mail an Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Sobald Sie &quot;E-Mail an Salesforce (BCC)&quot; aktivieren, erhalten Sie einen BCC Ihrer E-Mails, und Ihre E-Mails werden als Aktivitäten zu Chancen, Leads und Kontakten protokolliert.

>[!PREREQUISITES]
>
>Salesforce und Sales Connect müssen verbunden sein.

**So protokollieren Sie Ihre E-Mails in Salesforce per E-Mail (BCC)**

1. Klicken Sie in Sales Connect auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen** aus.

   ![](assets/one-3.png)

1. Klicken Sie unter &quot;Mein Konto&quot;(Admin-Einstellungen, wenn Sie Administrator sind) auf **Salesforce**.

   ![](assets/two-3.png)

1. Klicken Sie auf die Registerkarte **Einstellungen synchronisieren** .

   ![](assets/three-1.png)

1. Klicken Sie auf die Registerkarte **E-Mail an Salesforce (BCC)** und dann auf **Aktivieren**.

   ![](assets/six-2.png)

Wenn Ihre E-Mail-an-Salesforce-Adresse aus irgendeinem Grund nicht erfasst wird, führen Sie die folgenden Schritte aus, um die BCC-Funktion in Ihrem Salesforce-Konto zu aktivieren:

1. Melden Sie sich bei Ihrer Salesforce-Instanz an.
1. Suchen Sie Ihren Benutzernamen in der oberen rechten Ecke und wählen Sie die Dropdown-Leiste aus.
1. Wählen Sie **Meine Einstellungen** aus.
1. Wählen Sie **E-Mail** aus.
1. Wählen Sie **Meine E-Mail an Salesforce** aus.
1. Auf dieser Seite sehen Sie ein Feld mit der Bezeichnung &quot;E-Mail an Salesforce-Adresse&quot;. Wenn daneben nichts eingetragen ist, scrollen Sie nach unten zu &quot;Meine akzeptablen E-Mail-Adressen&quot;.
1. Geben Sie die E-Mail-Adresse(n) ein, die BCC verwenden soll.
1. Klicken Sie auf **Änderungen speichern**.

**Kann meine E-Mail an Salesforce nicht in meinen Einstellungen finden**

Wenn Sie Meine E-Mail an Salesforce unter Ihren Einstellungen nicht sehen, hat Ihr Administrator sie möglicherweise nicht aktiviert. Dies kann passieren, wenn Ihr Team neu bei Salesforce ist oder Ihr Team noch nie die BCC-Adresse verwendet hat, die Salesforce bereitstellt.

>[!NOTE]
>
>Sie benötigen Administratorrechte, um dies einzurichten.

1. Klicken Sie auf **Einrichten**.
1. Klicken Sie auf **E-Mail-Administration**.
1. Klicken Sie auf **E-Mail an Salesforce**.
1. Klicken Sie auf **Bearbeiten**.
1. Aktivieren Sie das Kästchen neben &quot;Aktiv&quot;.
1. Klicken Sie auf **Speichern**.

## Aufgaben von Sales Connect/Wiedervorlagen für Salesforce-Aufgaben synchronisieren {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Klicken Sie auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen** aus.

   ![](assets/one-3.png)

1. Klicken Sie unter &quot;Mein Konto&quot;(Admin-Einstellungen, wenn Sie Administrator sind) auf **Salesforce**.

   ![](assets/two-2.png)

1. Klicken Sie auf die Registerkarte **Einstellungen synchronisieren** .

   ![](assets/three-1.png)

1. Klicken Sie auf den Pfeil neben Synchronisieren von Sales Connect-Aufgaben/Erinnerungen mit Salesforce-Aufgaben.

   ![](assets/seven-2.png)

1. Wählen Sie die gewünschte Option aus (&quot;Synchronisieren Sie nicht mit Salesforce-Aufgaben&quot; ist standardmäßig ausgewählt).

   ![](assets/eight.png)
