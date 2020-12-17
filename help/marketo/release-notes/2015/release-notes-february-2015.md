---
unique-page-id: 6094890
description: Versionshinweise - Februar 2015 - Marketing Docs - Produktdokumentation
title: Versionshinweise - Februar 2015
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# Versionshinweise: Februar 2015 {#release-notes-february}

Die folgenden Funktionen sind in der Version vom Februar 2015 enthalten. Überprüfen Sie Ihre Marketing Edition auf Verfügbarkeit der Funktionen. Stellen Sie nach der Veröffentlichung sicher, dass Sie zu den einzelnen Funktionen nach Links zu detaillierten Artikeln suchen. Trommelwalzen...

## Verbesserungen der Marketing-Automatisierung {#marketing-automation-enhancements}

** [Intelligente Kampagne verschieben](../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Freut euch! Jetzt können Sie intelligente Kampagnen per Drag &amp; Drop oder mit der Funktion Verschieben in der Struktur in Programme verschieben.

** [Dynamics 2015 (Online)](http://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises) **- unterstützt!

**Änderungen am HTTPS-Zertifikat**

Zur Wahrung der Vertraulichkeit und Integrität von Kundendaten und SaaS-Diensten folgt Marketo den Best Practices der SaaS-Branche

und ersetzt derzeit verwendete Sicherheitsprotokolle (SHA-1 und SSL) durch sicherere Versionen (SHA-2 (alias). SHA-256) und TLS) für die folgenden Domänen:

`·` [marketo.net](http://marketo.net) (verschlüsselter Munchkin-Traffic)

`·` [marketo.com](http://marketo.com) (Hauptanwendungen von SaaS)

Dies wird kurz nach dieser Version passieren. Das SHA-1-Protokoll wird bis Dezember 2015 unter der Domäne [mktoapi.com](http://mktoapi.com) vorübergehend unterstützt, damit Eigentümer von älteren Systemen und Anwendungen ihre Systeme mit SHA-2-Kompatibilität aktualisieren können.

**Sicherer Munchkin**

Wir entfernen unsere Unterstützung für SSL3. Wir haben SSL3 bisher beibehalten, um die Unterstützung alter Webbrowser zu erhalten, aber 2015 wird kein signifikanter Web-Traffic von diesen Browsern mehr festgestellt. Dies würde sich nur auf Munchkin auswirken, wenn es auf sicheren Seiten verwendet wird, und wird nach der Februar-Version langsam eingeführt.

## Verbesserungen der Echtzeit-Personalisierung {#real-time-personalization-enhancements}

** [Zielgruppen-URL für Kampagnen](../../product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Wählen Sie die Seiten aus, auf denen Ihre Echtzeit-Kampagne angezeigt werden soll, indem Sie &quot;Hinzufügen eine Zielgruppen-URL&quot;verwenden. Diese Funktion funktioniert mit allen Typen von Kampagnen (Dialog, In Zone, Widgets), ist jedoch besonders nützlich für In-Zone-Kampagnen, bei denen eine Kampagne in der Zone-ID nur für die ausgewählte Zielgruppen-URL gerendert wird. Es unterstützt das Hinzufügen mehrerer URLs zur Zielgruppe verschiedener Webseiten.

![](assets/image2015-2-19-11-3a0-3a30.png)

** [Land und Bundesland zum kontobasierten Targeting hinzugefügt](https://docs.marketo.com/display/DOCS/View+a+Named+Account+List)**

Land und Bundesland können jetzt zu Ihren Listen mit Ihrem benannten Konto hinzugefügt werden. Zielgruppe wichtiger Konto-Potenzieller Kunde von bestimmten Orten.
