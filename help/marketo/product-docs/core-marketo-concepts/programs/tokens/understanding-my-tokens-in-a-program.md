---
unique-page-id: 1147114
description: Grundlegendes zu meinen Token in einem Programm - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu meinen Token in einem Programm
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# Grundlegendes zu meinen Token in einem Programm {#understanding-my-tokens-in-a-program}

Ein Token ist eine Variable, die Sie in E-Mails, Landingpages und Smart-Kampagnen verwenden können, um Ihr Leben zu vereinfachen.

Zusätzlich zu „Meine Token“ können Sie auch eines der integrierten Token in Ihren Programmen verwenden. Sehen Sie sich die [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} an.

## Meine Token  {#my-tokens}

Meine Token sind benutzerdefinierte Variablen, die jeder erstellen kann. Lokal werden sie [ Kampagnenordnern ](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} Programmen erstellt.

Meine Token werden wie folgt angezeigt: `{{my.Name Of Token}}`

Beispiele:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>Token-Typ</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kalenderdatei <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token, um <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">eine Kalenderereignisdatei (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs) </a> Ihren E-Mails und Landingpages hinzuzufügen.</td> 
  </tr> 
  <tr> 
   <td><p>Datum <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Dieses Token enthält einen Datumswert. Das Datum wird als Jahr-Monat-Tag angezeigt (z. B. 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>E-Mail-Script <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token, um ein Velocity-Skript in Ihren E-Mails auszuführen. <a href="https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/email-scripting" title="Link folgen" rel="nofollow">Weitere Informationen</a>. </td> 
  </tr> 
  <tr> 
   <td>Zahl<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Beliebige Ganzzahl. Es kann sogar negativ sein.</td> 
  </tr> 
  <tr> 
   <td>RTF <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Das ist HTML. Verwenden Sie ihn in E-Mails und Landingpages.</td> 
  </tr> 
  <tr> 
   <td>Ergebnis <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token im Schritt <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">Score-Fluss ändern</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC-Kampagne <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">Verwenden Sie dieses Token, damit Leads, die Teil eines Marketo-Programms werden, auch zu dem hinzugefügt werden können, was SFDC Campaign hinzugefügt wird.</td> 
  </tr> 
  <tr> 
   <td>Text <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Nur Text. Verwenden Sie es, wenn HTML zu viel Arbeit erfordert. Die Größenbeschränkung für Text-Token beträgt 524.288 Zeichen (UTF-8) oder 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Meine Token werden beim Senden einer E-Mail von Sales Insight auf [!DNL Microsoft Dynamics] oder [!DNL Salesforce] nicht aufgelöst. Nur Standard-Token werden ausgefüllt (Lead, Unternehmen usw.). Die Standardwerte für Token _werden_ funktionieren jedoch.

## Verschachteln von Token {#nesting-tokens}

Wenn Sie ein neues Token erstellen, kann es von anderen Objekten in der Struktur referenziert werden. Es gibt eine Benennungsstruktur, bei der das Token für eine einfache Verwaltung erstellt wurde.

* **Lokales Token:** Das Token wurde direkt in diesem Programm oder Ordner erstellt.
* **Vererbtes Token:** Das Token wurde in der Baumstruktur an einer Stelle in einem Programm oder Ordner einer höheren Ebene erstellt.
* **Überschriebenes Token:** Das Token wurde vererbt und dann machte jemand eine Ausnahme in diesem Programm oder Ordner.

Sie können globale Variablen erstellen und sie dann auf niedrigeren Ebenen in der Struktur überschreiben.

Das Verschieben von Programmen und Ordnern wirkt sich auch auf Token aus. Stellen Sie immer sicher, dass Verweise beim Verschieben nicht beschädigt werden.

>[!NOTE]
>
>Wenn die von einem Interaktionsprogramm gesendete E-Mail eine untergeordnete E-Mail eines Standardprogramms ist (nicht lokal in Ihrem Interaktionsprogramm), werden alle in der E-Mail verwendeten Token aus dem Standardprogramm aufgelöst, in dem sich die untergeordnete E-Mail befindet.

>[!MORELIKETHIS]
>
>* [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Meine Token verwalten](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
