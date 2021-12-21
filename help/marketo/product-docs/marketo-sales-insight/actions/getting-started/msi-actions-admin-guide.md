---
description: MSI Actions Admin Guide - Marketo Docs - Produktdokumentation
title: Administratorhandbuch für MSI-Aktionen
hide: true
hidefromtoc: true
source-git-commit: 9ee07611ffae25fea4bffa3124927083bf187ddd
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 1%

---

# Administratorhandbuch für MSI-Aktionen {#msi-actions-admin-guide}

>[!PREREQUISITES]
>
>* Vergewissern Sie sich bei Ihrem Customer Success Manager, dass MSI-Aktionen für Ihr Marketo-Konto aktiviert wurden (Wenn Sie kein CSM haben, geben Sie bitte an, [Support kontaktieren](https://nation.marketo.com/t5/support/ct-p/Support)).
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

PICC

1. Klicken **Sales Insight**, dann **Aktionskonfiguration**. Wählen Sie aus einer Liste von Marketo-Administratoren aus, die Sie einladen möchten, und klicken Sie auf **Einladung senden**.

PICC

Der Benutzer erhält eine E-Mail mit Schritten, um Zugriff auf das Konto zu erhalten.

>[!NOTE]
>
>Zusätzliche Benutzer werden nicht über Marketo hinzugefügt und stattdessen über die Seite &quot;Benutzerverwaltung für Verkaufskonten&quot;hinzugefügt. [Hier klicken](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) , um mehr über das Hinzufügen zusätzlicher Benutzer zu erfahren.

## Marketo-Verkaufskonto mit Salesforce verbinden {#connect-marketo-sales-account-to-salesforce}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen**.

PICC

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Salesforce**.

PICC

1. Klicken Sie auf der Registerkarte Verbindungen und Anpassungen auf **Verbinden**.

PICC

1. Klicken **OK**.

PICC

Wenn Sie bereits bei Salesforce angemeldet sind, werden Sie angemeldet sein. Ist dies nicht der Fall, werden Sie aufgefordert, sich anzumelden.

## Verbinden von Marketo mit Ihrem App-Konto für Vertrieb {#connect-marketo-to-your-sales-apps-account}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen**.

PICC

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Marketo**.

PICC

1. Klicken **connect**. Ihr Konto wird dann verbunden.

>[!NOTE]
>
>Wenn keine Verbindung hergestellt wird, kopieren Sie die Anmeldeinformationen aus der Registerkarte &quot;Aktionskonfiguration&quot;von Marketo Sales Insight und fügen Sie sie auf der Registerkarte &quot;Einrichtung&quot;ein.

## Datensynchronisation starten {#initiate-data-sync}

1. Klicken Sie in Marketo auf &quot;Admin&quot;.

PICC

1. Klicken Sie auf Sales Insight und dann auf Aktionskonfiguration.

PICC

1. Klicken Sie auf der Karte Aktionsfeld-Synchronisierung auf **Synchronisieren**.

PICC

1. Sie sehen eine Vorschau der zu synchronisierenden Felder. Klicken **Synchronisierung starten**.

PICC

Personendatensätze, die in Marketo und Salesforce vorhanden sind, werden mit Ihrem Marketo Sales Apps-Konto synchronisiert.

## Einladen einzelner Benutzer zu MSI-Aktionen {#invite-individual-users-to-msi-actions}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen**.

PICC

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **Benutzerverwaltung**.

PICC

1. Klicken **Aktionen** und wählen Sie **Benutzer einladen**.

PICC

1. Geben Sie die E-Mail-Adresse(n) ein und klicken Sie auf **Einladen**.

>[!NOTE]
>
>Standardmäßig werden alle neuen Mitglieder zum Team Alle hinzugefügt.

Sie erhalten eine Bestätigungsnachricht.

## Benutzer über CSV zu MSI-Aktionen einladen {#invite-users-via-csv-to-msi-actions}

1. Klicken Sie in Ihrem Marketo-Verkaufskonto auf das Zahnradsymbol und wählen Sie **Einstellungen**.

PICC

1. Wählen Sie unter &quot;Admin Settings&quot;die Option **Benutzerverwaltung**.

PICC

1. Klicken **Aktionen** und wählen Sie **Benutzer über CSV einladen**.

PICC

1. Suchen Sie auf Ihrem Computer nach der CSV-Datei, wählen Sie sie aus und klicken Sie auf **Nächste**.

PICC

1. Überprüfen Sie, ob die Felder korrekt zugeordnet sind, und klicken Sie auf **Einladen**.

PICC

Sie erhalten eine Bestätigungsnachricht, sobald die Einladungen gesendet wurden.

>[!NOTE]
>
>Danach können Sie entweder Ihr vorhandenes MSI-Paket aktualisieren oder ein neues installieren und zu [Konfigurieren von MSI-Aktionen in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/salesforce-configuration/msi-actions-configuration-in-salesforce.md).
