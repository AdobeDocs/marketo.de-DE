---
unique-page-id: 6094890
description: Versionshinweise - Februar 2015 - Marketo-Dokumentation - Produktdokumentation
title: Versionshinweise - Februar 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 15%

---

# Versionshinweise – Februar 2015 {#release-notes-february}

Die folgenden Funktionen sind in der Version vom Februar 2015 enthalten. Bitte überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit. Vergewissern Sie sich, dass Sie nach der Veröffentlichung zurückkehren, um Links zu detaillierten Artikeln für jede Funktion zu finden. Trommelwirbel…

## Verbesserungen bei der Marketing-Automatisierung {#marketing-automation-enhancements}

**[Intelligente Kampagne verschieben](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Viel Spaß! Sie können jetzt intelligente Kampagnen per Drag-and-drop oder mit der Verschieben-Funktion in der Baumstruktur in Programme verschieben und daraus entfernen.

**[[!DNL Dynamics] 2015 (Online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - Unterstützt!

**HTTPS-Zertifikatänderungen**

Zum Schutz der Vertraulichkeit und Integrität von Kundendaten und SaaS-Services befolgt Marketo die Best Practices der SaaS-Branche

und wird die derzeit verwendeten Sicherheitsprotokolle (SHA-1 und SSL) durch sicherere Versionen (SHA-2 (auch bekannt als SHA-256) und TLS) für die folgenden Domains ersetzen:

* marketo.net (verschlüsselter [!DNL Munchkin] Traffic)

* [marketo.com](https://marketo.com) (SaaS-Hauptanwendungen)

Dies geschieht kurz nach dieser Version. Das SHA-1-Protokoll wird bis Dezember 2015 vorübergehend auf der [mktoapi.com](https://mktoapi.com)-Domain unterstützt, damit Besitzer älterer Systeme und Anwendungen ihre Systeme mit SHA-2-Kompatibilität aktualisieren können.

**Sichere[!DNL Munchkin]**

Wir entfernen unsere Unterstützung für SSL3. Bisher haben wir SSL3 beibehalten, um Unterstützung für alte Webbrowser zu erhalten, aber 2015 sehen wir keinen signifikanten Webtraffic mehr von diesen Browsern. Dies würde sich nur auf [!DNL Munchkin] auswirken, wenn es auf sicheren Seiten verwendet wird, und wird nach der Februarversion langsam eingeführt.

## Verbesserungen bei Real-Time Personalization {#real-time-personalization-enhancements}

**[Target-URL für Kampagnen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Wählen Sie mithilfe von „Ziel-URL hinzufügen“ die Seiten aus, die Ihre Echtzeit-Kampagne anzeigen soll. Diese Funktion funktioniert bei allen Kampagnentypen (Dialogfeld, In-Zone, Widgets), ist aber besonders für In-Zone-Kampagnen nützlich, bei denen eine Kampagne nur für die ausgewählte Ziel-URL in der Zonen-ID gerendert wird. Es unterstützt das Hinzufügen mehrerer URLs zu verschiedenen Web-Seiten.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Land und Bundesland zum kontobasierten Targeting hinzugefügt**

Jetzt können Land und Bundesland zu Ihren Named-Accounts-Listen hinzugefügt werden. Zielen Sie auf wichtigste potenzielle Kunden an bestimmten Standorten ab.
