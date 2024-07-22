---
description: Vertriebsaktivitäten mit Salesforce synchronisieren - Marketo Docs - Produktdokumentation
title: Vertriebsaktivitäten mit Salesforce synchronisieren
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# Vertriebsaktivitäten mit Salesforce synchronisieren {#sync-sales-activities-to-salesforce}

Sie können die Salesforce-Synchronisierungseinstellungen für Aktionen konfigurieren, um E-Mails zu protokollieren und Aktivitäten in Salesforce aufzurufen. Dadurch erhalten Teams, die aus Ihrem CRM-System arbeiten, eine bessere Sichtbarkeit und Manager können diese Aktivitäten verwenden, um benutzerspezifische Salesforce-Berichte zu erstellen, um die Leistung Ihrer Teams zu verfolgen.

## Protokollieren von E-Mail-Aktivitäten bei Salesforce über API {#logging-email-activity-to-salesforce-via-api}

Für diese Funktion müssen Sie die Salesforce-Edition (Enterprise/Unlimited Edition) oder die Professional Edition verwenden, wenn Sie die Integration über Web Services API erworben haben.

>[!PREREQUISITES]
>
>Salesforce- und Sales Insight-Aktionen müssen verknüpft sein.

1. Klicken Sie in Sales Insight-Aktionen auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/sync-sales-activities-to-salesforce-1.png)

1. Klicken Sie unter &quot;Admin Settings&quot;(oder &quot;My Account&quot;, wenn Sie kein Administrator sind) auf **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-2.png)

1. Klicken Sie auf die Registerkarte **Einstellungen synchronisieren** .

   ![](assets/sync-sales-activities-to-salesforce-3.png)

1. Klicken Sie auf den Pfeil neben Protokoll-E-Mail-Aktivität zu Salesforce.

   ![](assets/sync-sales-activities-to-salesforce-4.png)

1. Klicken Sie auf die Registerkarte **Salesforce API** . Auf dieser Karte können Sie Ihre Voreinstellung für die Protokollierung von Informationen in Salesforce einrichten. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/sync-sales-activities-to-salesforce-5.png)

## Protokollieren von E-Mail-Aktivitäten bei Salesforce per E-Mail an Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Sobald Sie &quot;E-Mail an Salesforce (BCC)&quot; aktivieren, erhalten Sie einen BCC Ihrer E-Mails, und Ihre E-Mails werden als Aktivitäten zu Chancen, Leads und Kontakten protokolliert.

>[!PREREQUISITES]
>
>Salesforce- und Sales Insight-Aktionen müssen verknüpft sein.

**So protokollieren Sie Ihre E-Mails in Salesforce per E-Mail (BCC)**

1. Klicken Sie in Marketo Sales auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/sync-sales-activities-to-salesforce-6.png)

1. Klicken Sie unter &quot;Admin Settings&quot;(oder &quot;My Account&quot;, wenn Sie kein Administrator sind) auf **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-7.png)

1. Klicken Sie auf die Registerkarte **Einstellungen synchronisieren** .

   ![](assets/sync-sales-activities-to-salesforce-8.png)

1. Klicken Sie auf die Registerkarte **E-Mail an Salesforce (BCC)** und dann auf **Aktivieren**.

   ![](assets/sync-sales-activities-to-salesforce-9.png)

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

## Synchronisieren von Sales Insight-Aktionsaufgaben/-Erinnerungen mit Salesforce-Aufgaben {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Klicken Sie in Sales Insight-Aktionen auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/sync-sales-activities-to-salesforce-10.png)

1. Klicken Sie unter &quot;Admin Settings&quot;(oder &quot;My Account&quot;, wenn Sie kein Administrator sind) auf **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-11.png)

1. Klicken Sie auf die Registerkarte **Einstellungen synchronisieren** .

   ![](assets/sync-sales-activities-to-salesforce-12.png)

1. Klicken Sie auf den Pfeil neben Marketo Sales Tasks/Reminders zu Salesforce Tasks synchronisieren.

   ![](assets/sync-sales-activities-to-salesforce-13.png)

1. Wählen Sie die gewünschte Option aus (&quot;Synchronisieren Sie nicht mit Salesforce-Aufgaben&quot; ist standardmäßig ausgewählt).

   ![](assets/sync-sales-activities-to-salesforce-14.png)

## Synchronisieren von Sales Insight-Aktionsaufgaben mit Salesforce zum ersten Mal {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Insight-Aktionen und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden keine aktuellen Aufgaben, die Sie in Sales Insight-Aktionen haben, an Salesforce übergeben. Um Übersichtlichkeit und Duplikate zu reduzieren, sind die einzigen Aufgaben, die aus Sales Insight-Aktionen in Salesforce synchronisiert werden, Aufgaben, die nach der Synchronisierung von Sales Insight-Aktionen mit SFDC erstellt wurden.

Folgendes passiert, wenn Sie Sales Insight-Aktionen und SFDC-Aufgaben synchronisieren:

* Sobald Sie auf Bei der Aufgabensynchronisierung speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC zu Sales Insight-Aktionen abgerufen. Die Synchronisation basiert auf dem Fälligkeitsdatum und alle diese Aufgaben werden im Backend synchronisiert, aber im Command Center werden nur noch Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle Elemente, die in den letzten 15 Tagen gelöscht wurden, aus Command Center gelöscht.

* Solange die Synchronisierung aktiviert ist, synchronisieren wir ständig Aufgaben zwischen Sales Insight Actions und SFDC.

* Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Insight-Aktionen erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wurde, aktualisiert Ihre Aufgabenliste in Sales Insight-Aktionen.

* Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Synchronisierungsfeld auf Ihrer Einstellungsseite in der Webanwendung.
