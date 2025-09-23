---
unique-page-id: 11383945
description: Grundlegendes zu Facebook-Offline-Konversionen - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Offline-Konversionen in Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 2%

---

# Grundlagen [!DNL Facebook] Offline-Konversionen {#understanding-facebook-offline-conversions}

Facebook-Lead-Werbekampagnen generieren Leads und senden sie zur Verwendung in Marketing-Kampagnen an Marketo. Ohne Einblick in Offline-Konversionen kann der [!DNL Facebook] Advertiser jedoch nicht wissen, welche Anzeigen am effektivsten sind. Hier ein Beispiel.

>[!NOTE]
>
>**Beispiel**
>
>[!UICONTROL Facebook Lead Ads] führt drei Anzeigen aus.
>
>* Anzeige 1 generiert 20 Leads
>* Anzeige 2 generiert 30 Leads
>* Anzeige 3 generiert 50 Leads
>
>Allein auf Grundlage dieser Zahlen scheint Ad 3 die effektivste zu sein.
>
>Wenn man jedoch Daten auf der Marketo-Seite betrachtet, entwickelt sich eine andere Geschichte.
>
>* Anzeige 1 generiert 10 Verkäufe
>* Anzeige 3 generiert 2 Umsätze
>
>Das bedeutet, dass die Erfolgsrate von Ad 1 trotz der Generierung weniger Leads 50 Prozent betrug, während Ad 3 überhaupt nicht effektiv war.
>
>Ohne Offline-Konversionen würde der Werbetreibende wahrscheinlich mehr Geld in Ad 3 investieren. Bei Offline-Konversionsdaten wird der Werbetreibende mit größerer Wahrscheinlichkeit in Anzeige 1 investieren.

Sie können [Facebook-Offline-Konversionen einrichten](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) um die Offline-Anzeigenleistung an [!DNL Facebook] zu senden.

1. Stellen Sie sicher[[!DNL Facebook] [!UICONTROL &#x200B; dass Ihre &#x200B;]LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md)-Integration auf dem neuesten Stand ist.
1. Ordnen Sie die Stadien in Ihrem Umsatzzyklusmodell den Offline-Konversionsstadien in [!DNL Facebook] zu.
1. Wenn ein [!DNL Facebook] Lead aus einer [!DNL Facebook] Lead-Anzeige generiert wird und eine zugeordnete Phase erreicht, sendet Marketo Offline-Konversionsdaten über eine sichere, automatisierte API mehrmals täglich an [!DNL Facebook] zurück. Die Daten werden im Bericht &quot;[!DNL Facebook] Ads Manager“ angezeigt.

>[!MORELIKETHIS]
>
>[Einrichten [!DNL Facebook] Offline-Konvertierungen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
