---
unique-page-id: 4720758
description: Versionshinweise - Januar 2015 - Marketo-Dokumente - Produktdokumentation
title: Januar 2015 - Versionshinweise
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 4%

---

# Versionshinweise: Januar 2015 {#release-notes-january}

Die folgenden Funktionen sind in der Version vom Januar 2015 enthalten. Informationen zur Verfügbarkeit von Funktionen finden Sie in Ihrer Marketo Edition. Stellen Sie nach der Veröffentlichung sicher, dass Sie zu den einzelnen Funktionen Links zu detaillierten Artikeln finden!

## Aktualisierungen der Marketing-Automatisierung {#marketing-automation-updates}

**Mobilgerätefreundliche Einstiegsseiten**

Sie können jetzt [mobile Ansichten für Landingpages](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) im Landingpage-Editor erstellen. Stellen Sie Ihre Nachricht unabhängig vom Gerät effektiv bereit und erhöhen Sie die Interaktion, indem Sie Ihre Inhalte für den einfachen Verbrauch unterwegs anpassen. Diese Funktion wird während der Woche nach der Veröffentlichung schrittweise eingeführt.

[- Anleitung zur Landingpage - Video-](https://youtu.be/aPQHlG2X6c0)

**Neue REST-API-Aufrufe**

Drei neue Aufrufe für die Lead- und Aktivitäts-ReST-API:

* Lead löschen
* Abrufen von Leads nach Programm-ID
* Gelöschte Leads abrufen

Außerdem gibt es eine neue Option für &quot;Lead synchronisieren&quot;, um die Lead-Änderung asynchron zu schreiben, um einen schnelleren API-Aufruf zu ermöglichen. Vollständige Details sind nach der Veröffentlichung unter [developers.marketo.com](https://developers.marketo.com) verfügbar.

**E-Mail-Skriptfunktionen: Support für benutzerdefinierte Objekte**

Greifen Sie jetzt in E-Mail-Skripten auf benutzerdefinierte Objekte zu, die mit dem Konto-Objekt verknüpft sind!

## Echtzeit-Personalisierung {#real-time-personalization}

**Individuelles Remarketing für Google und Facebook**

Remarketing zeigt Anzeigen für Personen, die Ihre Website besucht haben. Sie können Ihre Remarketing-Kampagnen jetzt auf [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) und [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) mithilfe von Daten aus der Echtzeit-Personalisierung personalisieren. Remarketing für Zielgruppen aus verschiedenen Branchen, spezifische Kontolisten, Unternehmensgrößen oder Daten bekannter Leads.

[Namenskontenlisten-Modul](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Verbesserungen am Modul &quot;Spezifische Konten&quot;verbessern die Übereinstimmungsraten und Überprüfungen für Benutzer. Zu den Hinweisen gehören:

* Abgleichen von Organisationen aus Ihrer Liste mit Ihrem spezifischen Konto mithilfe der E-Mail-Adresse des Leads (auch für RTP-Kunden)
* Unterstützung für bis zu 100.000 Datensätze pro Konto
* CSV-Dateivorlage zum Anzeigen und Herunterladen

![](assets/image2015-1-14-11-3a12-3a16.png)

**Aktualisierte RTP-Tag-Optionen**

Die RTP-Tag-Optionen unter &quot;Kontoeinstellungen&quot;wurden aktualisiert und umfassen nun Folgendes:

1. CDN und Asynchron (empfohlenes Tag)
1. CDN und synchron (hohe Geschwindigkeit)
1. Asynchrones Tag ohne CDN
1. Synchrone Tags ohne CDN

Für eine optimale Leistung wird empfohlen, das Tag nach `<head>` oben in der Kopfzeile Ihrer Web-Seite zu platzieren. Alle Tags ermöglichen die Verwendung der [RTP-API](https://developers.marketo.com/documentation/websites/rtp-js-api/). Informationen zur Bereitstellung des RTP-Tags finden Sie unter [hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
