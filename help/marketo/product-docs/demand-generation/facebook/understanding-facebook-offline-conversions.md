---
unique-page-id: 11383945
description: Grundlegendes zu Facebook-Offline-Konversionen - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Offline-Konversionen in Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Grundlegendes zu Offline-Konversionen in Facebook {#understanding-facebook-offline-conversions}

Facebook Lead Ads-Kampagnen generieren Leads und senden sie zur Verwendung in Marketingkampagnen an Marketo. Ohne die Sichtbarkeit von Offline-Konversionen kann der Facebook-Advertiser jedoch nicht wissen, welche Anzeigen am effektivsten sind. Hier ist ein Beispiel.

>[!NOTE]
>
>**Beispiel**
>
>Facebook Lead Ads führt drei Anzeigen aus.
>
>* Anzeige 1 generiert 20 Leads
>* Anzeige 2 generiert 30 Leads
>* Anzeige 3 generiert 50 Leads
>
>Basierend auf diesen Zahlen erscheint allein Anzeige 3 als die effektivste.
>
>Bei der Betrachtung von Daten auf der Marketo-Seite entwickelt sich jedoch eine andere Geschichte.
>
>* Anzeige 1 generiert 10 Verkäufe
>* Ad 3 generiert 2 Verkäufe
>
>Das bedeutet, dass Anzeige 1, obwohl sie weniger Leads generiert hat, eine Erfolgsrate von 50 Prozent aufwies, während Anzeige 3 überhaupt nicht wirksam war.
>
>Ohne Offline-Konversionen würde der Werbetreibende wahrscheinlich mehr Geld in Ad 3 investieren. Mit Offline-Konversionsdaten investiert der Werbetreibende wahrscheinlich eher in Anzeige 1.

Sie können [ Facebook-Offline-Konversionen einrichten](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md), um die Offline-Anzeigenleistung an Facebook zu senden.

1. Stellen Sie sicher, dass Ihre [Facebook LaunchPoint-Integration](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) auf dem neuesten Stand ist.
1. Ordnen Sie Phasen in Ihrem Umsatzzyklusmodell Offline-Konversionsphasen in Facebook zu.
1. Wenn ein Facebook-Lead aus einer Lead-Anzeige von Facebook generiert wird und eine zugeordnete Phase erreicht, sendet Marketo Offline-Konversionsdaten mehrmals täglich über eine sichere, automatisierte API an Facebook. Die Daten werden im Facebook Ads Manager-Bericht angezeigt.

>[!MORELIKETHIS]
>
>[Einrichten von Facebook-Offline-Konversionen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
