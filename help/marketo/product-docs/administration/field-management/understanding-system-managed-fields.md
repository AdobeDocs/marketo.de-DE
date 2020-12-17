---
unique-page-id: 5472615
description: Die systemverwalteten Felder - Marketing-Dokumente - Produktdokumentation
title: Die systemverwalteten Felder
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Die systemverwalteten Felder {#understanding-system-managed-fields}

Möglicherweise haben Sie bemerkt, dass die [Personendaten-Seite](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) eine Reihe nicht bearbeitbarer Felder enthält, die von Marketo erstellt wurden. Diese Daten stammen aus verschiedenen Quellen, und es gibt unzählige Werte, die angezeigt werden könnten.

## Feldtypen {#field-types}

| **Feldname** | **Definition** |
|---|---|
| Originalquellentyp | Der Ort, an dem ein Besucher einer Person oder Website zuerst gefunden wurde (Beispiel: Liste importieren, Webseitenbesuch) |
| Ursprüngliche Quellinformationen | Details zu diesem Ort (Beispiel: Name der Liste, URL der Webseite) |
| Ursprüngliche Suchmaschine | Falls zutreffend, die Suchmaschine, die die Person an die ursprüngliche Einstiegsquelle verwiesen hat |
| Ursprünglicher Suchbegriff | Falls zutreffend, der verwendete Suchbegriff, der die Person an die ursprüngliche Einstiegsquelle verwiesen hat |
| Ursprünglicher Werber | URL, die die ursprüngliche Einstiegsquelle gehostet hat |
| Registrierungsquellen-Typ | Der Ort, an dem eine Aktivität zuerst eine Person wurde (Beispiel: Liste importieren, Webseitenbesuch) |
| Informationen zur Registrierungsquelle | Details zu diesem Ort (Beispiel: Name der Liste, URL der Webseite) |
| Anonyme IP | Gibt die IP-Adresse einer Person an |
| Vorgestellte Firma | Marketo&#39;s beste Schätzung (basierend auf IP) der Firma der Person |
| Inferated City | Marketo&#39;s beste Schätzung (basierend auf IP) der Stadt der Person |
| Inferierte Staatsregion | Marketo&#39;s beste Schätzung (basierend auf IP) des Staates oder der Region der Person |
| Postleitzahl | Marketo&#39;s beste Schätzung (basierend auf IP) der Postleitzahl der Person |
| Inferiertes Land | Marketo&#39;s beste Schätzung (basierend auf IP) des Landes der Person |
| Großraum | Marketo&#39;s beste Schätzung (basierend auf IP) der Metropolregion der Person |
| Abgeleiteter Telefonbereichscode | Marketo&#39;s beste Schätzung (basierend auf IP) des Bereichscodes der Person |

## Mögliche Werte für Original- und Registrierungsquelle-Typ {#possible-values-for-original-and-registration-source-type}

Unten sind einige mögliche Werte und was sie meinen.

| **Originalquellentyp** | **Definition** |
|---|---|
| Salesforce.com | Person wurde aus einer Salesforce-Synchronisierung entdeckt |
| Webseitenbesuche | Person wurde auf einer Webseite entdeckt |
| Ausfüllen von Webformularen | Person wurde nach dem Ausfüllen eines Formulars entdeckt |
| Liste importieren | Person wurde bei einem Listen-Import entdeckt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| Weblink-Klick | Person wurde nach dem Klicken auf einen Link entdeckt |
| Verkaufsemail | Person wurde per E-Mail über Sales Insight-E-Mail-Hinzufügen gesendet |
| Person | Person wurde von Salesforce als Person synchronisiert |
| Kontakt | Person wurde von Salesforce als Kontakt synchronisiert |
| Munchkin-API | Person wurde von Marketo&#39;s Munchkin API entdeckt |
| Social-App | Person wurde von einem sozialen Widget entdeckt |
| Web Service API | Person wurde von einer Webdienst-API entdeckt |
| Ereignis-Partner | Person wurde durch einen synchronisierten Webinar-Dienst entdeckt |
| Associate Lead | Person, die über den Associate Lead API-Aufruf zusammengeführt wurde |

| **Registrierungsquellen-Typ** | **Definition** |
|---|---|
| Liste importieren | Persönlichkeit durch Import einer Liste |
| Salesforce.com | Werden Sie eine Person durch eine Salesforce-Synchronisierung |
| Ausfüllen von Webformularen | Persönlichkeit nach dem Ausfüllen eines Formulars |
| Verkaufsemail | Person wurde per E-Mail über Sales Insight-E-Mail-Hinzufügen gesendet |
| Web Service API | Person wurde über die SOAP/REST-API erstellt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| Munchkin-API | Werden Sie eine Person durch Marketo&#39;s Munchkin API |
| Social-App | Persönlichkeit durch ein soziales Widget |
| Ereignis-Partner | Persönlichkeit über einen verknüpften Webinar-Dienst |

