---
description: Admin-Setup-Handbuch für Sales Insight-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Admin-Einrichtungshandbuch für Sales Insight-Aktionen
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Admin-Einrichtungshandbuch für Sales Insight-Aktionen {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions ist eine Web-basierte Anwendung, die über das [Marketo Sales Insight Package} ausschließlich mit Salesforce CRM integriert ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Dies wird manchmal als &quot;Marketo-Vertrieb“ oder einfach als „Aktionen“ bezeichnet.

>[!PREREQUISITES]
>
>* Bestätigen Sie mit dem Adobe-Account-Team (Ihrem Account Manager), dass MSI Actions für Ihr Marketo Engage-Account aktiviert wurde (wenn Sie keinen Account Manager haben, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
>* Die Synchronisierung von Marketo und Salesforce muss eingerichtet sein.

<table>
 <tr>
  <th>Persona</th>
  <th>Schritt</th>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Marketo-Kundenkonto einrichten</td>
 </tr>
 <tr>
  <td>Marketo Admin oder <br/>Salesforce Admin</td>
  <td>Marketo-Kundenkonto mit Salesforce verbinden</td>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Marketo-Kundenkonto mit Marketo verbinden</td>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Initiieren der Datensynchronisation von Marketo mit dem Marketo-Kundenkonto</td>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Benutzer zu MSI-Aktionen einladen</td>
 </tr>
 <tr>
  <td>Salesforce Admin</td>
  <td>Installieren/Aktualisieren des MSI-Pakets in Salesforce</td>
 </tr>
 <tr>
  <td>Salesforce Admin</td>
  <td>Konfigurieren von MSI-Aktionen in Salesforce</td>
 </tr>
</table>

## Marketo-Kundenkonto einrichten {#set-up-marketo-sales-account}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Wenn auf der Karte „Integrationsinformationen“ keine Client-ID und kein Client-Geheimnis angezeigt werden, aktivieren Sie Ihre Actions-Instanz, indem Sie den ersten Benutzer einladen. Daraufhin werden die Client-ID und das Client-Geheimnis angezeigt.

1. Klicken Sie **Sales Insight**, dann **Actions Config**. Wählen Sie aus einer Liste von Marketo-Administratoren aus, die eingeladen werden sollen, und klicken Sie auf **Einladen senden**.

   ![](assets/msi-actions-admin-guide-2.png)

Der Benutzer erhält eine E-Mail mit Schritten, um Zugriff auf das Konto zu erhalten.

>[!NOTE]
>
>Zusätzliche Benutzende werden nicht über Marketo hinzugefügt, sondern über die Seite „Kundenverwaltung“ des Kundenkontos. [Klicken Sie hier](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} um mehr über das Hinzufügen zusätzlicher Benutzer zu erfahren.

## Marketo-Kundenkonto mit Salesforce verbinden {#connect-marketo-sales-account-to-salesforce}

1. Klicken Sie in Ihrem Marketo-Kundenkonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-3.png)

1. Klicken Sie unter „Admin Settings“ auf **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Klicken Sie auf der Registerkarte Verbindungen und Anpassungen auf **Verbinden**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Klicken Sie auf **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Wenn Sie bereits bei Salesforce angemeldet sind, sind Sie angemeldet. Wenn nicht, werden Sie aufgefordert, sich anzumelden.

## Verbinden von Marketo mit Ihrem Sales Apps-Konto {#connect-marketo-to-your-sales-apps-account}

1. Klicken Sie in Ihrem Marketo-Kundenkonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-7.png)

1. Klicken Sie unter „Admin Settings“ auf **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Klicken Sie auf **Verbinden**. Ihr Konto wird dann verbunden.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Wenn keine Verbindung hergestellt werden kann, kopieren Sie die Anmeldeinformationen aus der Registerkarte „Aktionskonfiguration“ von Marketo Sales Insight und fügen Sie sie in die Registerkarte „Einrichten“ ein.

## Initiieren der Datensynchronisation {#initiate-data-sync}

Mit der Feldsynchronisierung zur Datenvereinheitlichung für Sales Insight-Aktionen kann das System Personeninformationen aus Ihrer Marketo Engage-Datenbank in Ihre Sales Insight-Aktionsdatenbank abrufen, Ihre Personendaten auf dem neuesten Stand halten und sicherstellen, dass Aktivitäten in Marketo und Salesforce auf den richtigen Datensätzen protokolliert werden.

>[!CAUTION]
>
>Nachdem Sie die Datensynchronisation initiiert haben, sollten Sie **nicht** den ursprünglichen Benutzer aus Ihrer Sales Insight Actions-Instanz entfernen. Dies ist der Benutzer, an den die erste Einladung gesendet wurde.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Klicken Sie **Sales Insight**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Klicken Sie auf **Registerkarte** Aktionskonfiguration“. Klicken Sie auf der Karte Aktion Feldsynchronisierung auf **Synchronisieren**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Sie sehen eine Vorschau der Felder, die synchronisiert werden. Klicken Sie **Synchronisierung starten**.

   ![](assets/msi-actions-admin-guide-13.png)

Personendatensätze, die in Marketo und Salesforce vorhanden sind, werden mit Ihrem Marketo Sales Apps-Konto synchronisiert.

>[!NOTE]
>
>Weitere Informationen dazu, wie Personen- und Aktivitätsdaten zwischen Sales Insight-Aktionen, Marketo und Salesforce synchronisiert werden, finden [ hier ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Einzelne Benutzer zu MSI-Aktionen einladen {#invite-individual-users-to-msi-actions}

1. Klicken Sie in Ihrem Marketo-Kundenkonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-14.png)

1. Wählen Sie unter „Admin-Einstellungen **die Option „Benutzerverwaltung** aus.

   ![](assets/msi-actions-admin-guide-15.png)

1. Klicken Sie auf **Aktionen** und wählen Sie **Benutzer einladen** aus.

   ![](assets/msi-actions-admin-guide-16.png)

1. Geben Sie die E-Mail-Adresse(n) ein und klicken Sie auf **Einladen**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Standardmäßig werden alle neuen Mitglieder dem Team Alle hinzugefügt.

Sie erhalten eine Bestätigungsnachricht.

## Benutzer über CSV zu MSI-Aktionen einladen {#invite-users-via-csv-to-msi-actions}

1. Klicken Sie in Ihrem Marketo-Kundenkonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-18.png)

1. Wählen Sie unter „Admin-Einstellungen **die Option „Benutzerverwaltung** aus.

   ![](assets/msi-actions-admin-guide-19.png)

1. Klicken Sie auf **Aktionen** und wählen Sie **Benutzer über CSV einladen** aus.

   ![](assets/msi-actions-admin-guide-20.png)

1. Suchen Sie die CSV-Datei auf Ihrem Computer, wählen Sie sie aus und klicken Sie auf **Weiter**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Vergewissern Sie sich, dass die Felder ordnungsgemäß zugeordnet sind, und klicken Sie auf **Einladen**.

   ![](assets/msi-actions-admin-guide-22.png)

Sie erhalten eine Bestätigungsnachricht, sobald die Einladungen gesendet wurden.

>[!NOTE]
>
>Sobald dies geschehen ist, können Sie entweder Ihr bestehendes MSI-Paket aktualisieren oder ein neues installieren und mit &quot;[ von MSI-Aktionen in Salesforce&quot; ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
