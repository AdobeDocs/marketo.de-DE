---
description: Anmeldeverwaltungseinstellungen - Marketo-Dokumente - Produktdokumentation
title: Einstellungen der Anmeldeverwaltung
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Einstellungen der Anmeldeverwaltung {#login-management-settings}

Mit den Einstellungen der Anmeldeverwaltung können Administratoren die Authentifizierungseinstellungen für Benutzer von Sales Insight-Aktionen global festlegen.

>[!NOTE]
>
>Standardmäßig ist die Option Nur Salesforce für Instanzen von Sales Insight-Aktionen aktiviert. Wir empfehlen diese Einstellung, damit Benutzer sich [ Salesforce ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) können.

## Aktualisieren der Einstellungen für die Anmeldeverwaltung {#update-login-management-settings}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Führen Sie die folgenden Schritte aus, um Ihre Einstellungen für die Anmeldeverwaltung zu aktualisieren.

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/login-management-settings-1.png)

1. Klicken Sie unter „Admin Settings“ auf **General**.

   ![](assets/login-management-settings-2.png)

1. Scrollen Sie nach unten zur Karte Anmeldeverwaltung und wählen Sie die gewünschte Einstellung aus (in diesem Beispiel wählen wir Nur Salesforce aus). Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/login-management-settings-3.png)

## Häufig gestellte Fragen (FAQ) zu Salesforce {#salesforce-only-faq}

Nur Salesforce bedeutet, dass sich Benutzende nur authentifizieren können, um Sales Insight-Aktionen mit Salesforce zu verwenden. Es ist die Standardauswahl für Sales Insight-Aktionsinstanzen und wird empfohlen, da sich Benutzende nahtlos authentifizieren können, ohne einen Benutzernamen und ein Kennwort verwalten zu müssen.

### Wie aktiviert ein neuer Benutzer in meiner Instanz sein Konto, wenn „Nur Salesforce&quot; ausgewählt ist? {#activate-when-salesforce-only-is-selected}

Nach dem Klicken auf **Erste Schritte** in der Einladungs-E-Mail werden neue Benutzende zu einem Bildschirm zur Kontoaktivierung gesendet, wo sie aufgefordert werden, ihre Salesforce-Instanz zu verbinden, um ihr Sales Insight Actions-Konto zu aktivieren.

![](assets/login-management-settings-4.png)

### Mit welchen Authentifizierungsmethoden dürfen sich meine Benutzerinnen und Benutzer authentifizieren, wenn „Nur Salesforce&quot; ausgewählt ist? {#what-authentication-methods}

Beim Navigieren zu unserem Anmeldebildschirm geben Benutzer zunächst ihre E-Mail-Adresse ein. Anschließend klicken sie auf die Schaltfläche Salesforce One Click Login , über die sie sich mit dem Salesforce-Konto authentifizieren können, bei dem sie angemeldet sind.

>[!NOTE]
>
>Dies betrifft nur Benutzende, die direkt zum Anmeldebildschirm navigieren. Benutzende, die über Salesforce auf Aktionen zugreifen, werden mit [Auto-login](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) angemeldet.

![](assets/login-management-settings-5.png)

### Wie wird die Benutzerauthentifizierung für Aktionen gehandhabt, wenn ein Benutzer über Salesforce auf eine Aktionsfunktion zugreift und „Nur Salesforce&quot; ausgewählt ist? {#how-is-user-authentication-handled}

Wenn ein(e) Benutzende(r) auf eine der Aktionen klickt (Anruf, E-Mail, Kampagne, Aufgaben, Kampagnenliste usw.), verwenden wir seine SFDC-Authentifizierung, um ihn/sie automatisch bei seinem Sales Insight Actions-Konto anzumelden. Wir nennen diese Authentifizierung [automatische Anmeldung](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Häufig gestellte Fragen zu allen Anmeldemethoden {#all-login-methods-faq}

### Wie aktiviert ein neuer Benutzer in meiner Instanz sein Konto, wenn „Alle Anmeldemethoden“ ausgewählt ist? {#activate-when-all-login-methods-is-selected}

Wenn ein neuer Benutzer zu einer -Instanz eingeladen wird, erhält er eine E-Mail zur Kontoaktivierung. Er klickt auf die Schaltfläche „Erste Schritte“, um zu einer Seite zu gelangen, auf der er aufgefordert wird, ein Kennwort zu erstellen und zu bestätigen. Nach der Erstellung wird ihr Konto aktiviert und über den Onboarding-Workflow weitergeleitet.

![](assets/login-management-settings-6.png)

### Mit welchen Benutzern meiner Instanz darf ich mich anmelden, wenn „Alle Anmeldemethoden“ ausgewählt ist? {#what-are-users-allowed-to-log-in-with-all-login}

Bei der Nutzung unserer Anmeldeseite geben Benutzer zunächst ihre E-Mail-Adresse ein. Dann werden sie auf eine Seite weitergeleitet, die ihnen alle Anmeldeoptionen (Benutzername/Kennwort, SFDC, Gmail, SSO) zur Authentifizierung bietet.
