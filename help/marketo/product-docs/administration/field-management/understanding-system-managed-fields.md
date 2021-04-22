---
unique-page-id: 5472615
description: Erläuterungen zu systemverwalteten Feldern - Marketo Docs - Produktdokumentation
title: Die systemverwalteten Felder
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 14%

---

# Die systemverwalteten Felder {#understanding-system-managed-fields}

Möglicherweise haben Sie bemerkt, dass die [Personendaten-Seite](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) eine Reihe von nicht bearbeitbaren Feldern enthält, die von Marketo erstellt wurden. Diese Daten stammen aus verschiedenen Quellen, und es gibt unzählige Werte, die angezeigt werden könnten.

## Feldtypen {#field-types}

| **Feldname** | **Definition** |
|---|---|
| Ursprünglicher Quellentyp | Der Ort, an dem ein Besucher einer Person oder Website zuerst gefunden wurde (Beispiel: Liste importieren, Webseitenbesuch) |
| Ursprüngliche Quelleninfo | Details zu diesem Ort (Beispiel: Name der Liste, URL der Webseite) |
| Ursprüngliche Such-Engine | Falls zutreffend, die Suchmaschine, die die Person an die ursprüngliche Einstiegsquelle verwiesen hat |
| Ursprünglicher Suchausdruck | Falls zutreffend, der verwendete Suchbegriff, der die Person an die ursprüngliche Einstiegsquelle verwiesen hat |
| Ursprünglicher Verweis | URL, die die ursprüngliche Einstiegsquelle gehostet hat |
| Registrierungsquellentyp | Der Ort, an dem eine Aktivität zuerst eine Person wurde (Beispiel: Liste importieren, Webseitenbesuch) |
| Registrierungsquelleninfo | Details zu diesem Ort (Beispiel: Name der Liste, URL der Webseite) |
| Anonyme IP | Gibt die IP-Adresse einer Person an |
| Abgeleitetes Unternehmen | Marketos beste Einschätzung (basierend auf IP) der Firma der Person |
| Abgeleiteter Ort | Marketos beste Schätzung (basierend auf IP) der Stadt |
| Abgeleitetes Bundesland/abgeleitete Region | Marketos beste Schätzung (basierend auf IP) des Bundesstaates oder der Region der Person |
| Abgeleitete Postleitzahl | Marketos beste Schätzung (nach IP) der Postleitzahl der Person |
| Abgeleitetes Land | Marketos beste Schätzung (basierend auf IP) des Landes des Benutzers |
| Abgeleiteter Stadtbereich | Marketos beste Schätzung (basierend auf IP) der Metropolregion der Person |
| Abgeleitete Vorwahl | Marketos beste Schätzung (basierend auf IP) des Gebietscodes der Person |

## Mögliche Werte für Original- und Registrierungsquelle-Typ {#possible-values-for-original-and-registration-source-type}

Unten sind einige mögliche Werte und was sie meinen.

| **Ursprünglicher Quellentyp** | **Definition** |
|---|---|
| Salesforce.com | Person wurde aus einer Salesforce-Synchronisierung entdeckt |
| Webseitenbesuche | Person wurde auf einer Webseite entdeckt |
| Ausfüllen von Webformularen | Person wurde nach dem Ausfüllen eines Formulars entdeckt |
| Listenimport | Person wurde bei einem Listen-Import entdeckt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| Weblink-Klick | Person wurde nach dem Klicken auf einen Link entdeckt |
| Verkaufsemail | Person wurde per E-Mail über Sales Insight-E-Mail-Hinzufügen gesendet |
| Person | Person wurde von Salesforce als Person synchronisiert |
| Kontakt | Person wurde von Salesforce als Kontakt synchronisiert |
| Munchkin-API | Person wurde von der Marketo Munchkin API entdeckt |
| Social App | Person wurde von einem sozialen Widget entdeckt |
| Web Service API | Person wurde von einer Webdienst-API entdeckt |
| Veranstaltungspartner | Person wurde durch einen synchronisierten Webinar-Dienst entdeckt |
| Lead zuordnen | Person, die über den Associate Lead API-Aufruf zusammengeführt wurde |

| **Registrierungsquellentyp** | **Definition** |
|---|---|
| Listenimport | Persönlichkeit durch Import einer Liste |
| Salesforce.com | Werden Sie eine Person durch eine Salesforce-Synchronisierung |
| Ausfüllen von Webformularen | Persönlichkeit nach dem Ausfüllen eines Formulars |
| Verkaufsemail | Person wurde per E-Mail über Sales Insight-E-Mail-Hinzufügen gesendet |
| Web Service API | Person wurde über die SOAP/REST-API erstellt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| Munchkin-API | Persönlich durch die Marketo Munchkin API |
| Social-App | Persönlichkeit durch ein soziales Widget |
| Veranstaltungspartner | Persönlichkeit über einen verknüpften Webinar-Dienst |
