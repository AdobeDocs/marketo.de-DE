---
unique-page-id: 11380218
description: Versionshinweise - sommer '16 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - sommer '16
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
feature: Release Information
source-git-commit: 5e2d1979abcafd8e4a37e55b843be932125c954e
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 3%

---

# Versionshinweise: Sommer &#39;16 {#release-notes-summer}

Die folgenden Funktionen sind in der Sommerversion 16 enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit. Klicken Sie auf die Titel-Links, um detaillierte Artikel zu den einzelnen Funktionen anzuzeigen.

## [Account-based Marketing](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo Account-basiertes Marketing bietet alle wesentlichen Funktionen einer einheitlichen Plattform:

* **Target** - Kontoermittlung, Übereinstimmung von Interessenten mit Konten und Namenskontenlisten
* **Engage** - Kontobasierte Personalisierung, kanalübergreifende Interaktion und kontospezifische Workflows
* **Maßnahme** - Insights auf Konto- und Listenebene, Interaktionsbewertung des Kontos und Auswirkungen auf Pipeline und Umsatz

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM ist als Add-on für Ihr Marketo-Abonnement verfügbar. Wenden Sie sich daher an Ihren Vertriebsmitarbeiter, um es implementieren zu lassen.

## [Audit-Trail](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

Das Audit-Protokoll bietet einen umfassenden Verlauf der Änderungen, die innerhalb Ihres Marketo-Abonnements vorgenommen wurden. Es wird eine Rechenschaftspflicht unter Benutzern und Administratoren schaffen, dazu beitragen, die Ursache für unerwartetes Verhalten zu identifizieren, und die Sicherheit bieten, zu wissen, wer was und wann tut. Diese Informationen sind jederzeit verfügbar und können zur Beantwortung von Fragen wie:

* Was ist mit diesem Asset oder dieser Einstellung passiert und wer hat es zuletzt aktualisiert?
* Was hat Benutzer X so gemacht?
* Wer meldet sich bei unserem Konto an?

![](assets/audit-trail.png)

## [Integration von Marketo mit Vibes SMS LaunchPoint](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Erstellen Sie einfach SMS-Nachrichten direkt in Marketo. Personalisieren und zielen Sie Ihre Nachricht mit Ihren umfangreichen Marketo-Daten ab und überwachen Sie sie einfach über das Dashboard für SMS-Nachrichten.

>[!NOTE]
>
>Für diese Funktion ist es erforderlich, dass Sie über ein vorhandenes Konto für Vibes SMS verfügen.

![](assets/vibes-sms2.png)

## [Verbesserungen in Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variablen auf Modulebene**

Zuvor waren alle in E-Mail 2.0-Vorlagen spezifizierten Variablen im Umfang &quot;global&quot;. Bei Verwendung von Variablen in Modulen ist dies nicht immer wünschenswert, wenn Sie mehrere Instanzen des Moduls verwenden möchten. Mit dieser Version können Variablen jetzt als &quot;Modulebene&quot;angegeben werden, sodass Sie angeben können, dass der Benutzer eindeutige Werte für jedes Modul festlegen kann, in dem er verwendet wird.

![](assets/module-level-variables.png)

**Syntaxaktualisierung**

* Sie können jetzt &quot;mktoAddByDefault&quot;für Module verwenden, die in E-Mail 2.0-Vorlagen angegeben sind, um anzugeben, welche Module standardmäßig in neuen E-Mails angezeigt werden sollen. Dies ist viel bequemer, wenn Sie eine E-Mail-Vorlage mit einer großen Anzahl von Modulen erstellen.
* Bei Bildelementen können Sie jetzt angeben, ob das zugrunde liegende `<img>` Die Eigenschaften &quot;height&quot;und &quot;width&quot;des HTML-Elements sollten für den Endbenutzer gesperrt oder bearbeitbar sein. mktoLockImgSize=&quot;true&quot; bewirkt, dass Höhe/Breite gesperrt wird (auch wenn das Bild geändert wird). Auf ähnliche Weise bewirkt mktoLockImgStyle=&quot;true&quot;, dass die Eigenschaft &quot;style&quot;gesperrt wird.

**Codesuche**

Verwenden Sie neue Suchfunktionen, um effizient Inhalte im Code Ihrer E-Mail zu finden und zu ersetzen. Diese Funktion ist auch im E-Mail-Vorlageneditor verfügbar.

![](assets/2nd-screenshot.png)

**Token-Unterstützung in Bildelementen**

Token können jetzt im Bereich &quot;Externe URL&quot;des Einfügebild-Erlebnisses verwendet werden! Wenn Sie Bilder mit `{{my.tokens}}`können Sie diese Token jetzt in Email Editor 2.0 referenzieren. Beachten Sie, dass das Bild auf der Arbeitsfläche des E-Mail-Editors 2.0 weiterhin fehlerhaft angezeigt wird. Sie werden jedoch vor dem Versand Ihrer E-Mail in der Vorschau und im Beispiel gerendert.

## Mehrmarken-Domainen {#multiple-branding-domains}

Vorbei sind die Tage, an denen E-Mail-Tracking-Links nur mit einer einzigen Branding-Domäne versehen werden konnten. Sie können jetzt mehrere Branding-Domänen hinzufügen, um das Vertrauen der Verbraucher zu wecken, ein optimiertes Erscheinungsbild zu schaffen, das sich auf die Marke konzentriert, die Zustellbarkeit von E-Mails zu verbessern und anhand von E-Mails zu entscheiden, welche Branding-Domäne für die Tracking-Links jeder E-Mail verwendet werden soll.

![](assets/multiple-branding-domains.png)

## [Programm-Token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Wir haben einen neuen Token-Typ für Programme erstellt. Sie können jetzt Programmname, Beschreibung und ID in Assets und Schritten zum intelligenten Kampagnenfluss rendern.

![](assets/program-tokens.png)

## [Konzernschlüssel](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Es kann mühsam sein, jede Person in Ihrem Verkaufsteam zu verpflichten, unser Sales Insight-Plugin für Outlook zu installieren. Wir haben eine neue Möglichkeit eingeführt, das Plug-in für Outlook remote mithilfe eines Unternehmensschlüssels zu installieren. Senden Sie Ihrem IT-Team Ihren eindeutigen Schlüssel im Marketo Sales Insight -Abschnitt von Admin und lassen Sie ihn den Rest erledigen.

![](assets/enterprise-key.png)

## [Kampagnen zur Web-Personalisierung](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Geben Sie eine Zeitverzögerung für Webkampagnen an, die auf Ihrer Website reagieren sollen.

![](assets/dialog-campaign-delay.png)

## [Export von Content Analytics und Recommendations](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Inhaltsanalysen und Empfehlungsdaten offline anzeigen.

## [API-Support für Email Editor 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Vorhandene Asset-APIs, die zuvor nur mit E-Mails und Vorlagen der Version 1.0 kompatibel waren, sind jetzt für E-Mail-Assets der Version 2.0 aktiviert.

## [Marketo-Entwicklersite](https://developers.marketo.com/) {#marketo-developers-site}

Neu und noch besser!

## [Datenschutzeinstellungen](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Marketingexperten können Datenschutzeinstellungen verwenden, um zu entscheiden, ob Besucher mit Munchkin- und Web-Personalisierungsfunktionen verfolgt werden. Die Tracking-Ebene wird mithilfe der Einstellung Nicht verfolgen des Browsers, eines Opt-out-Cookies oder einer nicht spezifischen IP-Adresse gesteuert. Diese Methoden können sich auf den Wert und die Funktionalität von Marketo in bestimmten Bereichen auswirken. Wenn der Marketing-Experte jedoch nichts ändert, bleiben die Marketo-Funktionen unverändert.

Diese Funktion wird Kunden über einen Zeitraum von sechs Wochen schrittweise zur Verfügung gestellt. Wenn Sie es sofort benötigen, wenden Sie sich an den Marketo-Support.
