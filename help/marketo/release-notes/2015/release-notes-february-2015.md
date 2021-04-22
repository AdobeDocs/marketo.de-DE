---
unique-page-id: 6094890
description: Versionshinweise - Februar 2015 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Februar 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 18%

---

# Versionshinweise: Februar 2015 {#release-notes-february}

Die folgenden Funktionen sind in der Version vom Februar 2015 enthalten. Überprüfen Sie Ihre Marketo Edition auf Verfügbarkeit der Funktionen. Stellen Sie nach der Veröffentlichung sicher, dass Sie zu den einzelnen Funktionen nach Links zu detaillierten Artikeln suchen. Trommelwalzen...

## Verbesserungen der Marketing-Automatisierung {#marketing-automation-enhancements}

**[Intelligente Kampagne verschieben](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Viel Spaß! Sie können jetzt intelligente Kampagnen per Drag-and-drop oder mit der Verschieben-Funktion in der Baumstruktur in Programme verschieben und daraus entfernen.

**[Dynamics 2015 (Online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  - unterstützt!

**Änderungen am HTTPS-Zertifikat**

Zum Schutz der Vertraulichkeit und Integrität von Kundendaten und SaaS-Diensten befolgt Marketo die Best Practices der SaaS-Branche

und ersetzt derzeit verwendete Sicherheitsprotokolle (SHA-1 und SSL) durch sicherere Versionen (SHA-2 (alias). SHA-256) und TLS) für die folgenden Domänen:

* [marketo.net](https://marketo.net) (verschlüsselter Munchkin-Traffic)

* [marketo.com](https://marketo.com) (Hauptanwendungen von SaaS)

Dies wird kurz nach dieser Version passieren. Das SHA-1-Protokoll wird bis Dezember 2015 unter der Domäne [mktoapi.com](https://mktoapi.com) vorübergehend unterstützt, damit Eigentümer von älteren Systemen und Anwendungen ihre Systeme mit SHA-2-Kompatibilität aktualisieren können.

**Sicherer Munchkin**

Wir entfernen unsere Unterstützung für SSL3. Wir haben SSL3 bisher beibehalten, um die Unterstützung alter Webbrowser zu erhalten, aber 2015 wird kein signifikanter Web-Traffic von diesen Browsern mehr festgestellt. Dies würde sich nur auf Munchkin auswirken, wenn es auf sicheren Seiten verwendet wird, und wird nach der Februar-Version langsam eingeführt.

## Verbesserungen der Echtzeit-Personalisierung {#real-time-personalization-enhancements}

**[Zielgruppen-URL für Kampagnen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Wählen Sie mit &#39;Ziel-URL hinzufügen&#39; die Seiten aus, die in Ihrer Echtzeitkampagne angezeigt werden sollen. Diese Funktion funktioniert mit allen Typen von Kampagnen (Dialog, In Zone, Widgets), ist jedoch besonders nützlich für In-Zone-Kampagnen, bei denen eine Kampagne in der Zone-ID nur für die ausgewählte Zielgruppen-URL gerendert wird. Es unterstützt das Hinzufügen mehrerer URLs zur Zielgruppe verschiedener Webseiten.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Land und Bundesland zum kontobasierten Targeting hinzugefügt**

Jetzt können Land und Bundesland zu Ihren Named-Accounts-Listen hinzugefügt werden. Zielen Sie auf wichtigste potenzielle Kunden an bestimmten Standorten ab.
