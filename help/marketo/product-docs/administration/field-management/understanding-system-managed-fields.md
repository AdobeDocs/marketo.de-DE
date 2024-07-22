---
unique-page-id: 5472615
description: Grundlegendes zu systemverwalteten Feldern - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu systemverwalteten Feldern
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 13%

---

# Grundlegendes zu systemverwalteten Feldern {#understanding-system-managed-fields}

Möglicherweise haben Sie bemerkt, dass die [Personen-Detailseite](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} eine Reihe von nicht bearbeitbaren Feldern enthält, die von Marketo erstellt wurden. Diese Daten stammen aus verschiedenen Quellen, und es gibt unzählige Werte, die angezeigt werden können.

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
| Abgleitete Vorwahl | Die beste Schätzung von Marketo (basierend auf IP) des Gebietscodes der Person |

## Mögliche Werte für den Source-Typ Original und Registrierung {#possible-values-for-original-and-registration-source-type}

Im Folgenden finden Sie einige mögliche Werte und deren Bedeutung.

| **Ursprünglicher Source-Typ** | **Definition** |
|---|---|
| Salesforce.com | Person wurde bei einer [!DNL Webhook] -Synchronisierung entdeckt |
| Webseitenbesuche | Person wurde auf einer Webseite entdeckt |
| Webformularausfüllung | Person wurde nach dem Ausfüllen eines Formulars entdeckt |
| Listenimport | Person wurde beim Listenimport entdeckt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| Weblink-Klick | Person wurde nach dem Klicken auf einen Link erkannt |
| Sales Email | Person wurde eine E-Mail über [!DNL Sales Insight] E-Mail-Add-In gesendet |
| Person | Person wurde von [!DNL Salesforce] als Person synchronisiert |
| Kontakt | Person wurde von [!DNL Webhook] als Kontakt synchronisiert |
| [!DNL Munchkin] API | Person wurde von der Marketo Engage [!DNL Munchkin]-API entdeckt |
| Social App | Person wurde von einem Social-Widget entdeckt |
| Webdienst-API | Person wurde von einer Web-Service-API entdeckt |
| Veranstaltungspartner | Person wurde über einen synchronisierten Webinardienst entdeckt |
| Lead zuordnen | Person, die über den API-Aufruf &quot;Associate Lead&quot;zusammengeführt wurde |

| **Source-Registrierungstyp** | **Definition** |
|---|---|
| Listenimport | Person durch Listenimport werden |
| Salesforce.com | Person durch eine [!DNL Webhook]-Synchronisation werden |
| Webformularausfüllung | Person werden, nachdem ein Formular ausgefüllt wurde |
| Sales Email | Person wurde eine E-Mail über [!DNL Webhook] E-Mail-Add-In gesendet |
| Webdienst-API | Person wurde über die SOAP/REST-API erstellt |
| Neue Person | Person wurde manuell in die Datenbank eingegeben |
| [!DNL Munchkin] API | Person durch die [!DNL Munchkin]-API von Marketo werden |
| Social App | Person über ein Social Widget werden |
| Veranstaltungspartner | Person über einen verknüpften Webinar-Dienst werden |
