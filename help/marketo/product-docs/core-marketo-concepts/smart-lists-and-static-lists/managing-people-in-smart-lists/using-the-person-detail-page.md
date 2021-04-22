---
unique-page-id: 2953415
description: Verwenden der Seite "Personendetails"- Marketo Dokumente - Produktdokumentation
title: Verwenden der Seite "Personendetails"
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 50%

---

# Verwenden der Seite mit den Personendetails {#using-the-person-detail-page}

Die Personendetailseite enthält alle Informationen, die Marketo über eine Person kennt. Sie können Daten direkt auf dieser Seite bearbeiten.

## Seite &quot;Zu Personendaten&quot; {#getting-to-person-detail-page}

Es gibt viele Möglichkeiten, bestimmte Leute zu öffnen. Beispiele:

* In der **Datenbank** können Sie in der Schnellsuche suchen
* Eine Smart **Liste** oder Liste
* **Programm-** Memberstab
* **Ansicht Kampagne** Mitglied einer intelligenten Kampagne
* Einige **Berichte**

   <br> 

1. Klicken Sie entweder mit der Dublette auf eine beliebige Person oder klicken Sie mit der Maus auf die ID auf der linken Seite.

   ![](assets/one-1.png)

1. Dadurch wird der Bildschirm mit den Personendetails geöffnet.

   ![](assets/two-5.png)

## Seitenorganisation - Salesforce {#page-organization-salesforce}

Personeninformationen werden in die folgenden Registerkarten kategorisiert:

| Registerkarte | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Unternehmensinfo | Angaben und Anschrift der Person zur Firma. |
| Opportunity-Info | Aus Salesforce synchronisierte Opportunity-Informationen. |
| SFDC-Lead-Feld | Integrierte Salesforce-Felder. |
| Benutzerdefiniertes SFDC-Feld | Benutzerdefinierte Salesforce-Felder. |
| Aktivitätsprotokoll | Alle Aktivitäten, die mit der Person zusammenhängen. |

## Seitenorganisation - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Registerkarte | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Unternehmensinfo | Angaben und Anschrift der Person zur Firma. |
| Opportunity-Info | Von Microsoft synchronisierte Opportunity-Informationen. |
| Benutzerdefinierte Microsoft-Felder | Benutzerdefinierte Microsoft-Felder. |
| Microsoft-Lead-Feld | Integrierte Microsoft-Felder. |
| Aktivitätsprotokoll | Alle Aktivitäten, die mit der Person zusammenhängen. |

>[!NOTE]
>
>Außerdem können Sie Opportunity info [sehen, die über API](http://developers.marketo.com/rest-api/lead-database/opportunities/) eingefügt wird, wenn Instanzen nicht mit einem CRM synchronisiert werden.

## Bearbeiten eines Felds {#editing-a-field}

Viele Felder können bearbeitet werden. Um die Informationen einer Person zu aktualisieren, geben Sie einen neuen Wert ein und klicken Sie zum Speichern auf eine Stelle außerhalb des Felds.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Marketo-Standardfelder vor CRM-Synchronisierung {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Adresse | Jahresumsatz | Anonyme IP | Rechnungsadresse | Abrechnungsort |
| Abrechnungsland | Postleitzahl für Abrechnung | Bundesland für Abrechnung | Ort | Unternehmensname |
| Land | Erstellt am | Geburtsdatum | Abteilung | Nicht aufrufen |
| Nicht aufrufen – Grund | Nicht aufrufen – Ursache | E-Mail-Adresse | E-Mail-Adresse ungültig | Grund für ungültige E-Mail |
| Externe Unternehmens-ID | Externe Vertriebsmitarbeiter-ID | Faxnummer | Vorname | Vollständiger Name |
| Branche | Abgeleiteter Ort | Abgeleitetes Unternehmen | Abgeleitetes Land | Abgeleiteter Stadtbereich |
| Abgeleitete Vorwahl | Abgeleitete Postleitzahl | Abgeleitetes Bundesland/abgeleitete Region | Ist anonym | Ist Kunde |
| Ist Partner | Jobtitel | Nachname | Bewertung | Bewertung |
| Person – Quelle | Status | Haupttelefonnummer | Marketo Social – Facebook-Anzeigename | Marketo Social Facebook-ID |
| Marketo Social – Facebook-Foto-URL | Marketo Social – Facebook-Profil-URL | Marketo Social – Facebook-Reichweite | Marketo Social – bezeichnete Registrierungen bei Facebook | Marketo Social – bezeichnete Besuche bei Facebook |
| Marketo Social – Geschlecht | Marketo Social – letzte bezeichnete Registrierung | Marketo Social – letzter bezeichneter Besuch | Marketo Social – LinkedIn-Anzeigename | Marketo Social LinkedIn-ID |
| Marketo Social – LinkedIn-Foto-URL | Marketo Social – LinkedIn-Profil-URL | Marketo Social – LinkedIn-Reichweite | Marketo Social – bezeichnete Registrierungen bei LinkedIn | Marketo Social – bezeichnete Besuche bei LinkedIn |
| Marketo Social Syndication-ID | Marketo Social – bezeichnete Registrierungen insgesamt | Marketo Social – bezeichnete Besuche insgesamt | Marketo Social – Twitter-Anzeigename | Marketo Social Twitter-ID |
| Marketo Social – Twitter-Foto-URL | Marketo Social – Twitter-Profil-URL | Marketo Social – Twitter-Reichweite | Marketo Social – bezeichnete Registrierungen bei Twitter | Marketo Social – bezeichnete Besuche bei Twitter |
| Zweiter Vorname | Mobiltelefonnummer | Anzahl Mitarbeiter | Telefonnummer | Postleitzahl |
| Priorität | Relative Bewertung | Stellenbeschreibung | Anrede | SIC-Code |
| Seite | Bundesland | Abgemeldet | Ursache für Abbestellung | Aktualisiert am |
| Dringlichkeit | Website |  |  |  |

>[!NOTE]
>
>Einige Felder sind bearbeitbar:__
>
>* Aktivitätsprotokoll
>* Informationen zur Firma
>* Möglichkeiten für die Kontakte zum SFDC
>* Bestimmte Marketo-spezifische Felder, wie &quot;Erstellungsdatum&quot;und &quot;Ursprünglicher Quelltyp&quot;.

>
>
Erfahren Sie mehr über [Systemverwaltete Felder](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Erstellen eines benutzerspezifischen Registers für die Seite mit den Benutzerdetails](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
