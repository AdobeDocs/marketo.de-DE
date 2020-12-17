---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Kontosynchronisierung - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Kontosynchronisierung
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Kontosynchronisierung {#microsoft-dynamics-sync-account-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit Dynamics synchronisiert? Es synchronisiert, wartet dann 5 Minuten und synchronisiert dann den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Dynamics Accounts speziell behandelt.

## Auf welche Weise werden die Informationen synchronisiert? {#which-way-does-the-information-sync}

Nur eine Möglichkeit: von Dynamics bis Marketo.

## Wie funktionieren die Updates? {#how-do-the-updates-work}

Wenn Sie ein Feld für ein Konto für einen Kontakt in Marketo aktualisieren, ändert es die Werte aller Kontakte, die zu diesem Konto in Marketo gehören. Es wird nicht mit Dynamics synchronisiert. Bei der nächsten Aktualisierung dieses Kontos in Dynamics werden jedoch alle Kontoinformationen in Marketo durch die Änderungen außer Kraft gesetzt.

## Kann ich mit Marketo ein Konto erstellen? {#can-i-create-an-account-using-marketo}

Anzahl Marketo kann keine Konten in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können die zu synchronisierenden Felder [während des Setups auswählen. ](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) Marketo synchronisiert jedoch nur die Felder, auf die Ihr Dynamics Sync-Benutzer Zugriff hat.

## Führt eine Änderung in einem Kontofeld in Dynamik zu einem Änderungs-Datenwert-Aktivität-Protokoll für jeden Kontakt?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Meistens ja. Wenn jedoch ein Konto mehr als 5.000 Kontakte hat und ein Feld auf diesem Konto sich in Dynamics ändert, synchronisieren wir die Änderung, aber protokollieren Sie nicht die Aktivität für die 5.000+ Kontakte.
