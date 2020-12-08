---
unique-page-id: 2953415
description: Verwenden der Seite "Personendetails"- "Marketing-Dokumente - Produktdokumentation"
title: Verwenden der Seite "Personendetails"
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---


# Verwenden der Seite &quot;Personendetails&quot; {#using-the-person-detail-page}

Die Personendetailseite enthält alle Informationen, die Marketo über eine Person kennt. Sie können Daten direkt auf dieser Seite bearbeiten.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Seite &quot;Zu Personendaten&quot; {#getting-to-person-detail-page}

Es gibt viele Möglichkeiten, bestimmte Leute zu öffnen. Nachfolgend sind einige Beispiele aufgeführt.

>[!NOTE]
>
>**Beispiel**
>
>* In der **Datenbank** können Sie in der Schnellsuche suchen
>* Jede intelligente **Liste** oder Liste
>* **Registerkarte &quot;Mitglieder** &quot;eines Programms
>* **Ansicht Kampagne Mitglieder** in einer intelligenten Kampagne
>* Einige **Berichte**

>



1. Klicken Sie entweder mit der Dublette auf eine beliebige Person oder klicken Sie mit der Maus auf die ID auf der linken Seite.

   ![](assets/one-1.png)

1. Dadurch wird der Bildschirm mit den Personendetails geöffnet.

   ![](assets/two-5.png)

## Seitenorganisation - Salesforce {#page-organization-salesforce}

Personeninformationen werden in die folgenden Registerkarten kategorisiert:

| Registerkarte | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Firma | Angaben und Anschrift der Person zur Firma. |
| Opportunity Info | Aus Salesforce synchronisierte Opportunity-Informationen. |
| SFDC-Interessentenfeld | Integrierte Salesforce-Felder. |
| Benutzerdefiniertes SFDC-Feld | Benutzerdefinierte Salesforce-Felder. |
| Aktivitäten-Protokoll | Alle Aktivitäten, die mit der Person zusammenhängen. |

## Seitenorganisation - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Registerkarte | Beschreibung |
|---|---|
| Info | Kontaktinformationen und benutzerdefinierte Felder zu einer Person. |
| Firma | Angaben und Anschrift der Person zur Firma. |
| Opportunity Info | Von Microsoft synchronisierte Opportunity-Informationen. |
| Microsoft Benutzerdefinierte Felder | Benutzerdefinierte Microsoft-Felder. |
| Microsoft-Interessentenfeld | Integrierte Microsoft-Felder. |
| Aktivitäten-Protokoll | Alle Aktivitäten, die mit der Person zusammenhängen. |

## Bearbeiten eines Felds {#editing-a-field}

Viele Felder können bearbeitet werden. Um die Informationen einer Person zu aktualisieren, geben Sie einen neuen Wert ein und klicken Sie zum Speichern auf eine Stelle außerhalb des Felds.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Markieren in Standardfelder vor der CRM-Synchronisierung {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Adresse | Jahresumsatz | Anonyme IP | Rechnungsadresse | Rechnungsstadt |
| Rechnungsland | Postleitzahl der Rechnungsstellung | Rechnungsstaat | Ort | Name der Firma |
| Land | Erstellt am | Geburtsdatum | Abteilung | Nicht aufrufen |
| Ursache nicht aufrufen | Grund nicht aufrufen | Email-Adresse | Email ungültig | Email-Fehler |
| Externe Firmen-ID | Externe Vertriebskennung | Faxnummer | Vorname | Vollständiger Name |
| Branche | Inferated City | Vorgestellte Firma | Inferiertes Land | Großraum |
| Abgeleiteter Telefonbereichscode | Postleitzahl | Inferierte Staatsregion | Ist anonym | Ist Kunde |
| Ist Partner | Auftragstitel | Nachname | Beurteilung | Ergebnis |
| Personalquelle | Status | Hauptfach | Anzeigename von &quot;Social Facebook&quot; | Marketing-zu-Social-Facebook-ID |
| Marketing-zu-Social-Facebook-Foto-URL | Marketing-zu-Social-Facebook-Profil-URL | Marketing-zu-Social-Facebook-Reichweite | Auf Facebook verwiesene &quot;Social Marketing&quot;-Registrierungen | Von Social Facebook verwiesene Besuche |
| Marketing für soziales Geschlecht | Anmeldung für &quot;Social zuletzt referenziert&quot; | Marketing zu Social - Letzter verwiesener Besuch | Markieren in Social LinkedIn-Anzeigename | MarketingIn Social LinkedIn-ID |
| Marketing-zu-Social LinkedIn-Foto-URL | Marketing-zu-Social-LinkedIn-Profil-URL | Marketing-Social LinkedIn-Reichweite | Von &quot;Social&quot;verwiesene LinkedIn-Registrierungen | Von Marketing zu Social verwiesene LinkedIn-Besuche |
| Marketing-Social-Syndikations-ID | In Social verwiesene Registrierungen gesamt | Marketing in Social insgesamt verwiesene Besuche | Anzeigename von Marketing in Social Twitter | Marketing-zu-Social-Twitter-ID |
| Marketing-zu-Social-Twitter-Foto-URL | Marketing-zu-Social-Twitter-Profil-URL | Marketing in Social - Twitter-Reichweite | Von Marketing zu Social verwiesene Twitter-Registrierungen | Von Marketing zu Social verwiesene Twitter-Besuche |
| Mittlerer Name | Mobiltelefonnummer | Anzahl Arbeitnehmer | Telefonnummer | Postleitzahl |
| Priorität | Relative Bewertung | Rolle | Anrede | SIC-Code |
| Site | state | Nicht abonniert | Grund für nicht abonnierte Benutzer | Aktualisiert am |
| Dringlichkeit | Webseite |  |  |  |

>[!NOTE]
>
>**Tieftauchen**
>
>Einige Felder können *nicht* bearbeitet werden:
>
>* Informationen zur Firma
>* Möglichkeiten für die Kontakte zum SFDC
>* Bestimmte marketingspezifische Felder, wie &quot;Erstellungsdatum&quot;und &quot;Ursprünglicher Quelltyp&quot;.
>* Aktivitäten-Protokoll

>
>
Weitere Informationen zu [systemverwalteten Feldern](../../../../product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Erstellen eines benutzerspezifischen Registers für die Seite mit den Benutzerdetails](../../../../product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)

>



