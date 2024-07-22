---
description: Verwaltungsanleitung für Sales Insight-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Admin-Setup-Anleitung für Sales Insight-Aktionen
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Admin-Setup-Anleitung für Sales Insight-Aktionen {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions ist eine webbasierte Anwendung, die über das [Marketo Sales Insight-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} in die Salesforce-Benutzeroberfläche integriert wird. Dies wird manchmal als &quot;Marketo-Verkäufe&quot;oder einfach als &quot;Aktionen&quot;bezeichnet.

>[!PREREQUISITES]
>
>* Vergewissern Sie sich beim Adobe Account Team (Ihrem Kundenbetreuer), dass MSI-Aktionen für Ihr Marketo Engage-Konto aktiviert wurden (wenn Sie keinen Kundenbetreuer haben, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
>* Ihre Marketo/Salesforce-Synchronisation muss eingerichtet sein.

<table>
 <tr>
  <th>Persona</th>
  <th>Schritt</th>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Einrichten des Marketo-Verkaufskontos</td>
 </tr>
 <tr>
  <td>Marketo Admin oder <br/>Salesforce Admin</td>
  <td>Marketo-Verkaufskonto mit Salesforce verbinden</td>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Marketo-Verkaufskonto mit Marketo verbinden</td>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Initiieren der Datensynchronisation von Marketo zu Marketo-Verkaufskonto</td>
 </tr>
 <tr>
  <td>Marketo-Administrator</td>
  <td>Benutzer zu MSI-Aktionen einladen</td>
 </tr>
 <tr>
  <td>Salesforce Admin</td>
  <td>MSI-Paket installieren/aktualisieren in Salesforce</td>
 </tr>
 <tr>
  <td>Salesforce Admin</td>
  <td>Konfigurieren von MSI-Aktionen in Salesforce</td>
 </tr>
</table>

## Einrichten des Marketo-Verkaufskontos {#set-up-marketo-sales-account}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Wenn auf der Karte &quot;Integrationsinformationen&quot;keine Client-ID und kein Client-Geheimnis angezeigt werden, aktivieren Sie Ihre Aktionsinstanz, indem Sie den ersten Benutzer einladen. Daraufhin werden die Client-ID und das Client-Geheimnis angezeigt.

1. Klicken Sie auf **Sales Insight** und dann auf **Aktionskonfiguration**. Wählen Sie aus einer Liste von Marketo-Administratoren aus, die Sie einladen möchten, und klicken Sie auf **Einladung senden**.

   ![](assets/msi-actions-admin-guide-2.png)

Der Benutzer erhält eine E-Mail mit Schritten, um Zugriff auf das Konto zu erhalten.

>[!NOTE]
>
>Zusätzliche Benutzer werden nicht über Marketo hinzugefügt und stattdessen über die Seite &quot;Benutzerverwaltung für Verkaufskonten&quot;hinzugefügt. [Klicken Sie hier](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} , um mehr über das Hinzufügen zusätzlicher Benutzer zu erfahren.

## Marketo-Verkaufskonto mit Salesforce verbinden {#connect-marketo-sales-account-to-salesforce}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-3.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Klicken Sie auf der Registerkarte Verbindungen und Anpassungen auf **Verbinden**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Klicken Sie auf **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Wenn Sie bereits bei Salesforce angemeldet sind, werden Sie angemeldet sein. Ist dies nicht der Fall, werden Sie aufgefordert, sich anzumelden.

## Verbinden von Marketo mit Ihrem App-Konto für Vertrieb {#connect-marketo-to-your-sales-apps-account}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-7.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Klicken Sie auf **connect**. Ihr Konto wird dann verbunden.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Wenn keine Verbindung hergestellt wird, kopieren Sie die Anmeldeinformationen aus der Registerkarte &quot;Aktionskonfiguration&quot;von Marketo Sales Insight und fügen Sie sie auf der Registerkarte &quot;Einrichtung&quot;ein.

## Datensynchronisation starten {#initiate-data-sync}

Die Datenzusammenführungsfeldsynchronisierung für Sales Insight-Aktionen ermöglicht es dem System, personenbezogene Daten aus Ihrer Marketo Engage-Datenbank in Ihre Sales Insight-Aktionsdatenbank zu übertragen, Ihre Personendaten auf dem neuesten Stand zu halten und sicherzustellen, dass Aktivitäten in Marketo und Salesforce in den richtigen Datensätzen protokolliert werden.

>[!CAUTION]
>
>Nachdem Sie die Datensynchronisation initiiert haben, sollten Sie den ursprünglichen Benutzer **nicht** in Ihrer Instanz von Sales Insight Actions entfernen. Dies ist der Benutzer, an den die erste Einladung gesendet wurde.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Klicken Sie auf **Sales Insight**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Klicken Sie auf die Registerkarte **Aktionskonfiguration** . Klicken Sie auf der Karte &quot;Synchronisierung von Aktionsfeldern&quot;auf **Synchronisieren**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Sie sehen eine Vorschau der zu synchronisierenden Felder. Klicken Sie auf **Synchronisation starten**.

   ![](assets/msi-actions-admin-guide-13.png)

Personendatensätze, die in Marketo und Salesforce vorhanden sind, werden mit Ihrem Marketo Sales Apps-Konto synchronisiert.

>[!NOTE]
>
>Um mehr darüber zu erfahren, wie Personen und Aktivitätsdaten zwischen Sales Insight-Aktionen, Marketo und Salesforce synchronisiert werden, klicken Sie hier [hier](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Einladen einzelner Benutzer zu MSI-Aktionen {#invite-individual-users-to-msi-actions}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-14.png)

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **User Management**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Klicken Sie auf **Aktionen** und wählen Sie **Benutzer einladen** aus.

   ![](assets/msi-actions-admin-guide-16.png)

1. Geben Sie die E-Mail-Adresse(n) ein und klicken Sie auf **Einladen**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Standardmäßig werden alle neuen Mitglieder zum Team Alle hinzugefügt.

Sie erhalten eine Bestätigungsnachricht.

## Benutzer über CSV zu MSI-Aktionen einladen {#invite-users-via-csv-to-msi-actions}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/msi-actions-admin-guide-18.png)

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **User Management**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Klicken Sie auf **Aktionen** und wählen Sie **Benutzer über CSV einladen** aus.

   ![](assets/msi-actions-admin-guide-20.png)

1. Suchen Sie auf Ihrem Computer nach der CSV-Datei, wählen Sie sie aus und klicken Sie auf **Weiter**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Vergewissern Sie sich, dass die Felder ordnungsgemäß zugeordnet sind, und klicken Sie auf **Einladen**.

   ![](assets/msi-actions-admin-guide-22.png)

Sie erhalten eine Bestätigungsnachricht, sobald die Einladungen gesendet wurden.

>[!NOTE]
>
>Danach können Sie entweder Ihr vorhandenes MSI-Paket aktualisieren oder ein neues installieren und mit [Konfigurieren von MSI-Aktionen in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"} fortfahren.
