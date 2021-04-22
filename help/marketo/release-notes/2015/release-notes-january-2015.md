---
unique-page-id: 4720758
description: Versionshinweise - Januar 2015 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Januar 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 4%

---

# Versionshinweise: Januar 2015 {#release-notes-january}

Die folgenden Funktionen sind in der Version vom Januar 2015 enthalten. Überprüfen Sie Ihre Marketo Edition auf Verfügbarkeit der Funktionen. Stellen Sie nach der Veröffentlichung sicher, dass Sie wieder zu finden Links zu detaillierten Artikeln für jede Funktion!

## Aktualisierungen der Marketing-Automatisierung {#marketing-automation-updates}

**Mobil-freundliche Landingpages**

Sie können jetzt [Mobilgeräte-Ansichten für Landingpages](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) aus dem Landingpages-Editor erstellen. Stellen Sie Ihre Nachricht unabhängig vom Gerät effektiv bereit und erhöhen Sie die Interaktion, indem Sie Ihre Inhalte für eine einfache Nutzung unterwegs anpassen. Diese Funktion wird schrittweise in der Woche nach der Veröffentlichung eingeführt.

[- Landingpage-exemplarisch](https://youtu.be/aPQHlG2X6c0)

**Neue Rest-API-Aufrufe**

Drei neue Aufrufe für die Lead &amp; Aktivität ReST-API:

* Lead löschen
* Interessenten nach Programm-ID abrufen
* Gelöschte Interessenten abrufen

Außerdem gibt es eine neue Option für &quot;Lead synchronisieren&quot;, um die Interessentenänderung asynchron für einen schnelleren API-Aufruf zu schreiben. Vollständige Details sind nach der Veröffentlichung unter [developer.marketo.com](https://developers.marketo.com) verfügbar.

**E-Mail-Skriptfunktionen: Support für benutzerdefinierte Objekte**

Greifen Sie nun über E-Mail-Skripte auf benutzerdefinierte Objekte zu, die mit dem Kontoobjekt verknüpft sind!

## Echtzeit-Personalisierung {#real-time-personalization}

**Individuelles Remarketing für Google und Facebook**

Remarketing zeigt Anzeigen für Personen, die Ihre Website besucht haben. Sie können Ihre Remarketing-Kampagnen jetzt unter [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) und [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) mithilfe von Daten aus der Echtzeit-Personalisierung personalisieren. Erfahren Sie mehr zu Audiencen aus verschiedenen Branchen, namentlich Kontoangaben, Listen der Firma oder Daten bekannter Interessenten.

[Modul zur Liste benannter Konten](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Verbesserungen am Modul Benannte Konten verbessern die Übereinstimmungsraten und Überprüfungen für Benutzer. Zu den Ergänzungen gehören:

* Übereinstimmungen von Organisationen aus Ihrer Liste mit Ihrem benannten Konto mithilfe der E-Mail-Adresse des Interessenten (auch für RTP-Kunden)
* Unterstützung von bis zu 100 K Datensätzen pro Konto
* CSV-Dateivorlage zur Ansicht und zum Herunterladen

![](assets/image2015-1-14-11-3a12-3a16.png)

**Aktualisierte RTP-Tag-Optionen**

Die RTP-Tag-Optionen unter &quot;Kontoeinstellungen&quot;wurden aktualisiert und umfassen Folgendes:

1. CDN und Asynchron (Recommended-Tag)
1. CDN und synchron (hohe Geschwindigkeit)
1. Asynchrones Tag ohne CDN
1. Synchrones Tag ohne CDN

Für eine optimale Leistung wird empfohlen, das Tag nach `<head>` oben in der Kopfzeile Ihrer Webseite zu platzieren. Alle Tags ermöglichen die Verwendung der [RTP-API](https://developers.marketo.com/documentation/websites/rtp-js-api/). Informationen zum Bereitstellen des RTP-Tags finden Sie unter [hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
