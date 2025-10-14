---
unique-page-id: 4720758
description: Versionshinweise - Januar 2015 - Marketo-Dokumentation - Produktdokumentation
title: Januar 2015 - Versionshinweise
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 5%

---

# Versionshinweise – Januar 2015 {#release-notes-january}

Die folgenden Funktionen sind in der Version vom Januar 2015 enthalten. Bitte überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit. Nach der Veröffentlichung sollten Sie unbedingt zurückkommen, um Links zu detaillierten Artikeln für jede Funktion zu finden!

## Aktualisierungen der Marketing-Automatisierung {#marketing-automation-updates}

**Handy-freundliche Landingpages**

Sie können [im Landingpage-Editor &#x200B;](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) mobile Ansichten für Landingpages erstellen). Stellen Sie Ihre Nachricht unabhängig vom Gerät effektiv bereit und steigern Sie die Interaktion, indem Sie Ihre Inhalte für den einfachen Gebrauch unterwegs anpassen. Diese Funktion wird in der Woche nach der Veröffentlichung schrittweise eingeführt.

Video-[&#x200B; zur schrittweisen Anleitung für &#x200B;](https://youtu.be/aPQHlG2X6c0)-Landingpages

**Neue REST API-Aufrufe**

Drei neue Aufrufe für die Lead &amp; Activity REST-API:

* Lead löschen
* Leads nach Programm-ID abrufen
* Gelöschte Leads abrufen

Außerdem gibt es eine neue Option für Lead synchronisieren , um die Lead-Änderung für einen schnelleren API-Aufruf asynchron zu schreiben. Alle Details werden nach der Veröffentlichung unter [https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/home verfügbar sein](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/home)

**E-Mail-Skriptfunktionen: Support für benutzerdefinierte Objekte**

Greifen Sie jetzt über E-Mail-Skripte auf benutzerdefinierte Objekte zu, die mit dem Kontoobjekt verknüpft sind!

## Echtzeit-Personalisierung {#real-time-personalization}

**Personalisiertes Remarketing für Google und[!DNL Facebook]**

Remarketing zeigt Anzeigen an Personen, die Ihre Website besucht haben. Sie können jetzt Ihre Remarketing-Kampagnen auf [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) personalisieren und mit Daten aus Real-Time Personalization [[!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md). Remarketing für Zielgruppen aus verschiedenen Branchen, benannte Kontolisten, Unternehmensgrößen oder Daten von bekannten Leads.

[Modul der Liste benannter Konten](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Verbesserungen am Modul Benannte Konten verbessern die Übereinstimmungsraten und Validierungen für Benutzer. Zu den Ergänzungen gehören:

* Abgleichen von Organisationen aus Ihrer Liste benannter Konten mithilfe der E-Mail-Adresse des Leads (auch für Kunden, die nur RTP verwenden)
* Unterstützung von bis zu 100.000 Datensätzen pro Konto
* CSV-Dateivorlage zum Anzeigen und Herunterladen

![](assets/image2015-1-14-11-3a12-3a16.png)

**Aktualisierte RTP-Tag-Optionen**

Die RTP-Tag-Optionen unter „Kontoeinstellungen“ wurden aktualisiert, um Folgendes einzuschließen:

1. CDN und Asynchron (Empfohlenes Tag)
1. CDN und synchron (hohe Geschwindigkeit)
1. Asynchrones Tag ohne CDN
1. Synchrones Tag ohne CDN

Um eine optimale Leistung zu erzielen, wird empfohlen, das -Tag nach dem `<head>` oben in der Kopfzeile Ihrer Web-Seite zu platzieren. Alle Tags ermöglichen die Verwendung der [RTP-](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation). Informationen zur Bereitstellung des RTP-Tags finden Sie unter [hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
