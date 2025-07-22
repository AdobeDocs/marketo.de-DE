---
unique-page-id: 2953415
description: Verwenden der Seite „Personendetails“ - Marketo-Dokumente - Produktdokumentation
title: Verwenden der Seite „Personendetails“
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 33%

---

# Verwenden der Seite „Personendetails“ {#using-the-person-detail-page}

Die Seite „Personendetails“ enthält alle Informationen, die Marketo über eine Person kennt. Daten können direkt von dieser Seite aus bearbeitet werden.

## Seite „Personendetails“ aufrufen {#getting-to-person-detail-page}

Es gibt viele Möglichkeiten, bestimmte Leute zu öffnen. Beispiele:

* In der **Datenbank** können Sie in der Schnellsuche suchen
* Beliebige **Smart-Liste** oder Liste
* **Mitglieder** Registerkarte eines Programms
* **Anzeigen von Kampagnenmitgliedern** in einer intelligenten Kampagne
* Einige **Berichte**
  <br> 

1. Doppelklicken Sie entweder auf eine beliebige Person oder klicken Sie einfach auf die ID auf der linken Seite.

   ![](assets/one-1.png)

1. Dadurch wird der Bildschirm mit den Personendetails geöffnet.

   ![](assets/two-5.png)

## Seitenorganisation - Salesforce {#page-organization-salesforce}

Personeninformationen werden in die folgenden Registerkarten kategorisiert:

| Tab | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Unternehmensinfo | Unternehmensinformationen und -adresse der Person. |
| Opportunity-Info | Opportunity-Informationen aus Salesforce synchronisiert. |
| SFDC-Lead-Feld | Integrierte Salesforce-Felder. |
| Benutzerdefiniertes SFDC-Feld | Benutzerdefinierte Salesforce-Felder. |
| Aktivitätsprotokoll | Alle mit der Person verbundenen Aktivitäten. |

## Seitenorganisation - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tab | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Unternehmensinfo | Unternehmensinformationen und -adresse der Person. |
| Opportunity-Info | Opportunity-Informationen aus Microsoft synchronisiert. |
| Benutzerdefinierte Microsoft-Felder | Benutzerdefinierte Microsoft-Felder. |
| Microsoft-Lead-Feld | Integrierte Microsoft-Felder. |
| Aktivitätsprotokoll | Alle mit der Person verbundenen Aktivitäten. |

>[!NOTE]
>
>Sie können auch Opportunity-[ (über API eingefügt) für ](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/opportunities) sehen, die nicht mit einem CRM synchronisiert wurden.

## Bearbeiten eines Felds {#editing-a-field}

Viele Felder können bearbeitet werden. Um die Informationen einer Person zu aktualisieren, geben Sie einen neuen Wert ein und klicken Sie zum Speichern auf eine Stelle außerhalb des Felds.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Marketo-Standardfelder vor der CRM-Synchronisierung {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| Adresse | Jahresumsatz | Anonyme IP | Rechnungsadresse | Abrechnungsort |
| Abrechnungsland | Postleitzahl für Abrechnung | Bundesland für Abrechnung | Stadt | Firmenname |
| Land | Erstellt um | Geburtsdatum | Abteilung | Nicht aufrufen |
| Nicht aufrufen – Grund | Nicht aufrufen – Ursache | E-Mail-Adresse | E-Mail-Adresse ungültig | Grund für ungültige E-Mail |
| Externe Unternehmens-ID | Externe Vertriebsmitarbeiter-ID | Faxnummer | Vorname | Vollständiger Name |
| Branche | Abgeleiteter Ort | Abgeleitetes Unternehmen | Abgeleitetes Land | Abgeleiteter Stadtbereich |
| Abgeleitete Vorwahl | Abgeleitete Postleitzahl | Abgeleitetes Bundesland/abgeleitete Region | Ist anonym | Ist Kunde |
| Ist Partner | Jobtitel | Nachname | Rating | Ergebnis |
| Person – Quelle | Status | Haupttelefonnummer | Anzeigename des Marketo Social-[!DNL Facebook] | Marketo Social [!DNL Facebook] ID |
| Foto-URL für Marketo Social [!DNL Facebook] | Profil-URL von Marketo Social [!DNL Facebook] | Marketo Social [!DNL Facebook] Reach | An Marketo Social [!DNL Facebook] weitergeleitete Registrierungen | Verwiesene Besuche bei Marketo Social [!DNL Facebook] |
| Marketo Social – Geschlecht | Marketo Social – letzte bezeichnete Registrierung | Marketo Social – letzter bezeichneter Besuch | Anzeigename des Marketo Social-[!DNL LinkedIn] | Marketo Social [!DNL LinkedIn] ID |
| Foto-URL für Marketo Social [!DNL LinkedIn] | Profil-URL von Marketo Social [!DNL LinkedIn] | Marketo Social [!DNL LinkedIn] Reach | An Marketo Social [!DNL LinkedIn] weitergeleitete Registrierungen | Verwiesene Besuche bei Marketo Social [!DNL LinkedIn] |
| Marketo Social Syndication-ID | Marketo Social – bezeichnete Registrierungen insgesamt | Marketo Social – bezeichnete Besuche insgesamt | Anzeigename des Marketo Social-[!DNL Twitter] | Marketo Social [!DNL Twitter] ID |
| Foto-URL für Marketo Social [!DNL Twitter] | Profil-URL von Marketo Social [!DNL Twitter] | Marketo Social [!DNL Twitter] Reach | An Marketo Social [!DNL Twitter] weitergeleitete Registrierungen | Verwiesene Besuche bei Marketo Social [!DNL Twitter] |
| Zweiter Vorname | Mobiltelefonnummer | Anzahl Mitarbeiter | Telefonnummer | Postleitzahl |
| Priorität | Relative Bewertung | Rolle | Anrede | SIC-Code |
| Seite | Land | Abgemeldet | Ursache für Abbestellung | Aktualisiert um |
| Dringlichkeit | Website |  |  |  |

>[!NOTE]
>
>Einige Felder können _nicht_ bearbeitet werden:
>
>* Aktivitätsprotokoll
>* Unternehmensinformationen
>* Möglichkeiten für SFDC-Kontakte
>* Bestimmte Marketo-spezifische Felder, z. B. Erstellungsdatum und ursprünglicher Source-Typ.
>
>Weitere Informationen zu [Systemverwalteten Feldern](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Erstellen einer benutzerdefinierten Registerkarte für die Personendetailseite](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
