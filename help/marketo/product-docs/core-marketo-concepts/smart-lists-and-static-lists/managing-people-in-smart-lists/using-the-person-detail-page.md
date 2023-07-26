---
unique-page-id: 2953415
description: Verwenden der Personendetailseite - Marketo-Dokumente - Produktdokumentation
title: Verwenden der Seite "Personendetails"
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 50%

---

# Verwenden der Seite &quot;Personendetails&quot; {#using-the-person-detail-page}

Die Personendetailseite enthält alle Informationen, die Marketo über eine Person kennt. Sie können Daten direkt auf dieser Seite bearbeiten.

## Zur Seite &quot;Personendetails&quot; {#getting-to-person-detail-page}

Es gibt viele Möglichkeiten, bestimmte Personen zu öffnen. Beispiele:

* Aus dem **Datenbank**, können Sie in der Schnellsuche suchen.
* Alle intelligenten **Liste** oder Liste
* **Mitglieder** Programmregisterkarte
* **Anzeigen von Campaign-Mitgliedern** in einer Smart-Kampagne
* Einige **Berichte**
  <br> 

1. Doppelklicken Sie auf eine beliebige Person oder klicken Sie mit einem Klick auf die ID auf der linken Seite.

   ![](assets/one-1.png)

1. Dadurch wird der Bildschirm mit den Personendetails geöffnet.

   ![](assets/two-5.png)

## Seitenorganisation - Salesforce {#page-organization-salesforce}

Personeninformationen werden in die folgenden Registerkarten kategorisiert:

| Registerkarte | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Unternehmensinfo | Unternehmensinformationen und -adresse der Person. |
| Opportunity-Info | Aus Salesforce synchronisierte Opportunity-Informationen. |
| SFDC-Lead-Feld | Integrierte Salesforce-Felder. |
| SFDC Benutzerdefiniertes Feld | Benutzerdefinierte Salesforce-Felder. |
| Aktivitätsprotokoll | Alle Aktivitäten, die mit der Person verbunden sind. |

## Seitenorganisation - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Registerkarte | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Unternehmensinfo | Unternehmensinformationen und -adresse der Person. |
| Opportunity-Info | Aus Microsoft synchronisierte Opportunity-Informationen. |
| Benutzerdefinierte Microsoft-Felder | Benutzerdefinierte Microsoft-Felder. |
| Microsoft-Lead-Feld | Integrierte Microsoft-Felder. |
| Aktivitätsprotokoll | Alle Aktivitäten, die mit der Person verbunden sind. |

>[!NOTE]
>
>Sie können auch Opportunity-Informationen anzeigen [über API eingefügt](https://developers.marketo.com/rest-api/lead-database/opportunities/) für Instanzen, die nicht mit einem CRM synchronisiert werden.

## Bearbeiten eines Felds {#editing-a-field}

Viele Felder können bearbeitet werden. Um die Informationen einer Person zu aktualisieren, geben Sie einen neuen Wert ein und klicken Sie außerhalb des zu speichernden Felds auf .

![](assets/image2015-2-27-11-3a14-3a2.png)

## Marketo-Standardfelder vor der CRM-Synchronisierung {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| Adresse | Jahresumsatz | Anonyme IP | Rechnungsadresse | Abrechnungsort |
| Rechnungsland | Postleitzahl für Rechnung | Bundesland für Rechnung | Ort | Firmenname |
| Land | Erstellt am | Geburtsdatum | Abteilung | Nicht aufrufen |
| Nicht aufrufen – Grund | Nicht aufrufen – Ursache | E-Mail-Adresse | E-Mail-Adresse ungültig | Grund für ungültige E-Mail |
| Externe Unternehmens-ID | Externe Vertriebsmitarbeiter-ID | Faxnummer | Vorname | Vollständiger Name |
| Branche | Abgeleiteter Ort | Abgeleitetes Unternehmen | Abgeleitetes Land | Abgeleiteter Stadtbereich |
| Abgeleitete Vorwahl | Abgeleitete Postleitzahl | Abgeleitetes Bundesland/abgeleitete Region | Ist anonym | Ist Kunde |
| Ist Partner | Jobtitel | Nachname | Bewertung | Bewertung |
| Personen-Quelle | Status | Haupttelefonnummer | Marketo Social – Facebook-Anzeigename | Marketo Social – Facebook-ID |
| Marketo Social – Facebook-Foto-URL | Marketo Social – Facebook-Profil-URL | Marketo Social – Facebook-Reichweite | Marketo Social – bezeichnete Registrierungen bei Facebook | Marketo Social – bezeichnete Besuche bei Facebook |
| Marketo Social – Geschlecht | Marketo Social – letzte bezeichnete Registrierung | Marketo Social – letzter bezeichneter Besuch | Marketo Social – LinkedIn-Anzeigename | Marketo Social – LinkedIn-ID |
| Marketo Social – LinkedIn-Foto-URL | Marketo Social – LinkedIn-Profil-URL | Marketo Social – LinkedIn-Reichweite | Marketo Social – bezeichnete Registrierungen bei LinkedIn | Marketo Social – bezeichnete Besuche bei LinkedIn |
| Marketo Social Syndication-ID | Marketo Social – bezeichnete Registrierungen insgesamt | Marketo Social – bezeichnete Besuche insgesamt | Marketo Social – Twitter-Anzeigename | Marketo Social – Twitter-ID |
| Marketo Social – Twitter-Foto-URL | Marketo Social – Twitter-Profil-URL | Marketo Social – Twitter-Reichweite | Marketo Social – bezeichnete Registrierungen bei Twitter | Marketo Social – bezeichnete Besuche bei Twitter |
| Zweiter Vorname | Mobiltelefonnummer | Anzahl Mitarbeiter | Telefonnummer | Postleitzahl |
| Priorität | Relative Bewertung | Rolle | Anrede | SIC-Code |
| Seite | Status | Abgemeldet | Ursache für Abbestellung | Aktualisiert am |
| Dringlichkeit | Website |  |  |  |

>[!NOTE]
>
>Einige Felder sind _not_ editable:
>
>* Aktivitätsprotokoll
>* Unternehmensinformationen
>* Möglichkeiten für SFDC-Kontakte
>* Bestimmte Marketo-spezifische Felder, z. B. Erstellungsdatum und Ursprünglicher Quelltyp.
>
>Weitere Informationen [Systemverwaltete Felder](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Erstellen einer benutzerdefinierten Registerkarte für die Seite &quot;Personendetails&quot;](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
