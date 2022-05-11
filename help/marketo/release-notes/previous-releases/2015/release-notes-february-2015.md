---
unique-page-id: 6094890
description: Versionshinweise - Februar 2015 - Marketo-Dokumente - Produktdokumentation
title: Februar 2015 - Versionshinweise
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 19%

---

# Versionshinweise: Februar 2015 {#release-notes-february}

Die folgenden Funktionen sind in der Version vom Februar 2015 enthalten. Informationen zur Verfügbarkeit von Funktionen finden Sie in Ihrer Marketo Edition. Stellen Sie nach der Veröffentlichung sicher, dass Sie zu den einzelnen Funktionen Links zu detaillierten Artikeln finden. Trommelrollen...

## Verbesserungen bei der Marketing-Automatisierung {#marketing-automation-enhancements}

**[Intelligente Kampagne verschieben](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Viel Spaß! Sie können jetzt intelligente Kampagnen per Drag-and-drop oder mit der Verschieben-Funktion in der Baumstruktur in Programme verschieben und daraus entfernen.

**[Dynamics 2015 (online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - unterstützt!

**HTTPS-Zertifikatänderungen**

Zum Schutz der Vertraulichkeit und Integrität von Kundendaten und SaaS-Diensten folgt Marketo den Best Practices der SaaS-Branche

und ersetzt die derzeit verwendeten Sicherheitsprotokolle (SHA-1 und SSL) durch sicherere Versionen (SHA-2 (alias SHA-256) und TLS) für die folgenden Domänen:

* marketo.net (verschlüsselter Munchkin-Traffic)

* [marketo.com](https://marketo.com) (Hauptanwendungen von SaaS)

Dies geschieht kurz nach dieser Version. SHA-1-Protokoll wird temporär von [mktoapi.com](https://mktoapi.com) -Domain bis Dezember 2015, damit Eigentümer von Legacy-Systemen und -Anwendungen ihre Systeme mit SHA-2-Kompatibilität aktualisieren können.

**Sicheres Munchkin**

Wir entfernen unsere Unterstützung für SSL3. Bis jetzt haben wir SSL3 gepflegt, um die Unterstützung alter Webbrowser zu erhalten. Im Jahr 2015 wird jedoch von diesen Browsern kein signifikanter Web-Traffic mehr beobachtet. Dies würde sich nur auf Munchkin auswirken, wenn es auf sicheren Seiten verwendet wird, und wird nach der Februar-Version langsam eingeführt.

## Verbesserungen bei der Echtzeit-Personalisierung {#real-time-personalization-enhancements}

**[Target-URL für Kampagnen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Wählen Sie mit &#39;Ziel-URL hinzufügen&#39; die Seiten aus, die in Ihrer Echtzeitkampagne angezeigt werden sollen. Diese Funktion funktioniert mit allen Kampagnentypen (Dialog, In Zone, Widgets), ist jedoch besonders nützlich für In-Zone-Kampagnen, bei denen eine Kampagne in der Zone-ID nur für die ausgewählte Ziel-URL gerendert wird. Es unterstützt das Hinzufügen mehrerer URLs zum Targeting verschiedener Webseiten.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Land und Bundesland für kontobasiertes Targeting hinzugefügt**

Jetzt können Land und Bundesland zu Ihren Named-Accounts-Listen hinzugefügt werden. Zielen Sie auf wichtigste potenzielle Kunden an bestimmten Standorten ab.
