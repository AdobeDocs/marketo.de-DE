---
description: Salesforce-Synchronisierungseinstellungen - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Synchronisationseinstellungen
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 2%

---

# Synchronisierungseinstellungen [!DNL Salesforce] {#salesforce-sync-settings}

## Protokollieren von E-Mail-Aktivitäten in [!DNL Salesforce] über API {#logging-email-activity-to-salesforce-via-api}

Für diese Funktion müssen Sie die Enterprise/Unlimited Edition von [!DNL Salesforce] verwenden oder die Professional Edition, wenn Sie Integration über die Web Services-API erworben haben.

>[!PREREQUISITES]
>
>[!DNL Salesforce] und [!DNL Sales Insight Actions] müssen verbunden sein.

1. Klicken Sie [!DNL Sales Insight Actions] auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/salesforce-sync-settings-1.png)

1. Klicken [!UICONTROL &#x200B; unter &quot;]&quot; (oder &quot;[!UICONTROL Mein Konto], wenn Sie kein Administrator sind) auf **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-2.png)

1. Klicken Sie auf die **[!UICONTROL Synchronisierungseinstellungen]**.

   ![](assets/salesforce-sync-settings-3.png)

1. Klicken Sie auf den Pfeil neben [!UICONTROL E-Mail-Aktivität protokollieren], um [!DNL Salesforce].

   ![](assets/salesforce-sync-settings-4.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Salesforce]** API. Auf dieser Karte können Sie festlegen, wie Sie Informationen in [!DNL Salesforce] protokollieren möchten. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/salesforce-sync-settings-5.png)

## Protokollieren der E-Mail-Aktivität für [!DNL Salesforce] per E-Mail an [!DNL Salesforce] (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Sobald Sie &quot;[!UICONTROL E-Mail an Salesforce (BCC)]&quot; aktiviert haben, erhalten Sie eine BCC Ihrer Verkaufs-E-Mails und Ihre E-Mails werden als Aktivitäten zu Opportunitys, Leads und Kontakten protokolliert.

>[!PREREQUISITES]
>
>[!DNL Salesforce] und [!DNL Sales Insight Actions] müssen verbunden sein.

**So melden Sie Ihre E-Mails [!DNL Salesforce] über E-Mail (BCC) an**

1. Klicken Sie in Marketo Sales auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/salesforce-sync-settings-6.png)

1. Klicken [!UICONTROL &#x200B; unter &quot;]&quot; (oder &quot;[!UICONTROL Mein Konto], wenn Sie kein Administrator sind) auf **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-7.png)

1. Klicken Sie auf die **[!UICONTROL Synchronisierungseinstellungen]**.

   ![](assets/salesforce-sync-settings-8.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte E-Mail an Salesforce (BCC]** und klicken Sie auf **[!UICONTROL Aktivieren]**.

   ![](assets/salesforce-sync-settings-9.png)

Wenn Ihre E-Mail-Adresse aus irgendeinem Grund nicht [!DNL Salesforce] wird, führen Sie die folgenden Schritte aus, um die BCC-Funktion in Ihrem [!DNL Salesforce]-Konto zu aktivieren:

1. Melden Sie sich bei Ihrer [!DNL Salesforce] an.
1. Suchen Sie Ihren Benutzernamen in der oberen rechten Ecke und wählen Sie die Dropdown-Leiste aus.
1. Wählen Sie **[!UICONTROL Meine Einstellungen]** aus.
1. Wählen Sie **[!UICONTROL E-Mail]** aus.
1. Wählen Sie **[!UICONTROL Meine E-Mail an Salesforce]** aus.
1. Auf dieser Seite wird ein Feld mit der Bezeichnung „E[!UICONTROL Mail an Salesforce-Adresse] angezeigt. Wenn daneben nichts ausgefüllt ist, scrollen Sie nach unten zu &quot;[!UICONTROL Meine akzeptablen E-Mail-Adressen].
1. Geben Sie die E-Mail-Adresse(n) ein, die BCC speichern soll(en).
1. Klicken Sie **[!UICONTROL Änderungen speichern]**.

**Meine zu [!DNL Salesforce] E-Mail kann in meinen Einstellungen nicht gefunden werden**

Wenn Meine E-Mail an [!DNL Salesforce] in Ihren Einstellungen nicht angezeigt wird, hat Ihr Administrator sie möglicherweise nicht aktiviert. Dies kann vorkommen, wenn Ihr Team mit [!DNL Salesforce] noch nicht vertraut ist oder Ihr Team die von [!DNL Salesforce] bereitgestellte BCC-Adresse noch nie verwendet hat.

>[!NOTE]
>
>Sie benötigen Administratorrechte, um dies einzurichten.

1. Klicken Sie **[!UICONTROL Setup]**.
1. Klicken Sie auf **[!UICONTROL E-Mail-Administration]**.
1. Klicken Sie **[!UICONTROL E-Mail an Salesforce]**.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Aktivieren Sie das Kontrollkästchen neben „Aktiv“.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## [!DNL Sales Insight Actions] Aufgaben/Erinnerungen mit [!DNL Salesforce] Aufgaben synchronisieren {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Klicken Sie [!DNL Sales Insight Actions] auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/salesforce-sync-settings-10.png)

1. Klicken [!UICONTROL &#x200B; unter &quot;]&quot; (oder &quot;[!UICONTROL Mein Konto], wenn Sie kein Administrator sind) auf **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-11.png)

1. Klicken Sie auf die **[!UICONTROL Synchronisierungseinstellungen]**.

   ![](assets/salesforce-sync-settings-12.png)

1. Klicken Sie auf den Pfeil neben Marketo-Verkaufsaufgaben/-erinnerungen mit [!DNL Salesforce] Aufgaben synchronisieren.

   ![](assets/salesforce-sync-settings-13.png)

1. Wählen Sie die gewünschte Option aus (standardmäßig „Mit [!DNL Salesforce] Aufgaben nicht synchronisieren“ ausgewählt).

   ![](assets/salesforce-sync-settings-14.png)

## Erstmaliges Synchronisieren [!DNL Sales Insight Actions] Aufgaben mit [!DNL Salesforce] {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen [!DNL Sales Insight Actions] und [!DNL Salesforce] Aufgaben zum ersten Mal aktivieren, importieren wir Ihre [!DNL Salesforce] Aufgaben. Wir werden keine aktuellen Aufgaben, die Sie [!DNL Sales Insight Actions] zu [!DNL Salesforce] haben, überspringen. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von [!DNL Sales Insight Actions] in [!DNL Salesforce] nach der Synchronisierung von [!DNL Sales Insight Actions] mit SFDC erstellt.

Folgendes passiert, wenn Sie [!DNL Sales Insight Actions]- und SFDC-Aufgaben synchronisieren:

Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC nach [!DNL Sales Insight Actions] übertragen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

Wir synchronisieren Aufgaben zwischen [!DNL Sales Insight Actions] und SFDC kontinuierlich, solange die Synchronisierung aktiviert ist.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in [!DNL Sales Insight Actions] erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in [!DNL Salesforce] synchronisiert. Und alles, was in [!DNL Salesforce] erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in [!DNL Sales Insight Actions].

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf der Seite [!UICONTROL Einstellungen] in der Web-Anwendung.
