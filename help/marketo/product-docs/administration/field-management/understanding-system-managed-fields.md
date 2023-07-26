---
unique-page-id: 5472615
description: Grundlegendes zu systemverwalteten Feldern - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu systemverwalteten Feldern
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 16%

---

# Grundlegendes zu systemverwalteten Feldern {#understanding-system-managed-fields}

Vielleicht haben Sie bemerkt, dass die Variable [Personendetailseite](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} verfügt über eine Reihe von nicht bearbeitbaren Feldern, die von Marketo erstellt wurden. Diese Daten stammen aus verschiedenen Quellen, und es gibt unzählige Werte, die angezeigt werden können.

## Feldtypen {#field-types}

| **Feldname** | **Definition** |
|---|---|
| Ursprünglicher Quellentyp | Der Ort, an dem eine Person oder ein Website-Besucher zuerst entdeckt wurde (Beispiel: Listenimport, Webseitenbesuch) |
| Ursprüngliche Quelleninfo | Details zu dieser Position (Beispiel: Name der Liste, URL der Webseite) |
| Ursprüngliche Such-Engine | Gegebenenfalls die Suchmaschine, die die Person an die ursprüngliche Einstiegsquelle verwiesen hat |
| Ursprünglicher Suchausdruck | Falls zutreffend, der verwendete Suchbegriff, der die Person an die ursprüngliche Quelle der Einsendung verwiesen hat |
| Ursprünglicher Verweis | URL, die die ursprüngliche Einstiegsquelle hostet |
| Registrierungsquellentyp | Der Ort, an dem eine Aktivität zuerst zu einer Person wurde (Beispiel: Listenimport, Webseitenbesuch) |
| Registrierungsquelleninfo | Details zu dieser Position (Beispiel: Name der Liste, URL der Webseite) |
| Anonyme IP | Gibt die IP-Adresse einer Person an |
| Abgeleitetes Unternehmen | Die beste Schätzung von Marketo (basierend auf IP) für das Unternehmen der Person |
| Abgeleiteter Ort | Die beste Schätzung von Marketo (basierend auf IP) für die Stadt der Person |
| Abgeleitetes Bundesland/abgeleitete Region | Die beste Schätzung von Marketo (basierend auf IP) des Bundesstaates oder der Region der Person |
| Abgeleitete Postleitzahl | Die beste Schätzung von Marketo (basierend auf IP) für die Postleitzahl der Person |
| Abgeleitetes Land | Die beste Schätzung von Marketo (basierend auf IP) für das Land der Person |
| Abgeleiteter Stadtbereich | Die beste Schätzung (basierend auf IP) der Metropolregion der Person durch Marketo |
| Abgeleitete Vorwahl | Die beste Schätzung von Marketo (basierend auf IP) des Gebietscodes der Person |

## Mögliche Werte für Ursprünge- und Registrierungsquellentyp {#possible-values-for-original-and-registration-source-type}

Im Folgenden finden Sie einige mögliche Werte und deren Bedeutung.

| **Ursprünglicher Quellentyp** | **Definition** |
|---|---|
| Salesforce.com | Person wurde aus einem [!DNL Webhook] Synchronisieren |
| Webseitenbesuche | Person wurde auf einer Webseite entdeckt |
| Webformularausfüllung | Person wurde nach dem Ausfüllen eines Formulars entdeckt |
| Listenimport | Person wurde beim Listenimport entdeckt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| Weblink-Klick | Person wurde nach dem Klicken auf einen Link erkannt |
| Sales Email | Person wurde eine E-Mail gesendet über [!DNL Sales Insight] E-Mail-Add-In |
| Person | Person wurde synchronisiert von [!DNL Salesforce] als Person |
| Kontakt | Person wurde synchronisiert von [!DNL Webhook] als Ansprechpartner |
| [!DNL Munchkin] API | Person wurde vom Marketo Engage entdeckt [!DNL Munchkin] API |
| Social App | Person wurde von einem Social-Widget entdeckt |
| Webservice-API | Person wurde von einer Web-Service-API entdeckt |
| Veranstaltungspartner | Person wurde über einen synchronisierten Webinardienst entdeckt |
| Lead zuordnen | Person, die über den API-Aufruf &quot;Associate Lead&quot;zusammengeführt wurde |

| **Registrierungsquellentyp** | **Definition** |
|---|---|
| Listenimport | Person durch Listenimport werden |
| Salesforce.com | Werden Sie ein Mensch durch eine [!DNL Webhook] Synchronisieren |
| Webformularausfüllung | Person werden, nachdem ein Formular ausgefüllt wurde |
| Sales Email | Person wurde eine E-Mail gesendet über [!DNL Webhook] E-Mail-Add-In |
| Webservice-API | Person wurde über die SOAP-/REST-API erstellt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| [!DNL Munchkin] API | Werden Sie durch Marketo zu einer Person [!DNL Munchkin] API |
| Social App | Person über ein Social Widget werden |
| Veranstaltungspartner | Person über einen verknüpften Webinar-Dienst werden |
