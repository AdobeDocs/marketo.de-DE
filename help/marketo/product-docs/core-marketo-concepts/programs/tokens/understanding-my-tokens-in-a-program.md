---
unique-page-id: 1147114
description: Einführung zu meinen Token in einem Programm - Marketing Docs - Produktdokumentation
title: Meine Token in einem Programm
translation-type: tm+mt
source-git-commit: e5050328cbddaf072dd60ddd8d7363a704e720b5
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# My Tokens in einem Programm {#understanding-my-tokens-in-a-program}

Ein Token ist eine Variable, die Sie in E-Mails, Landingpages und intelligenten Kampagnen verwenden können, um Ihr Leben zu vereinfachen.

Zusätzlich zu &quot;Meine Token&quot;können Sie auch beliebige der integrierten Token in Ihren Programmen verwenden. Sehen Sie sich die [Tokens-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) an.

## Meine Tokens {#my-tokens}

Meine Tokens sind benutzerspezifische Variablen, die jeder erstellen kann. Sie sind [created](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) in Kampagnen- oder Programmen.

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
   <td>Verwenden Sie dieses Token, um <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">eine Kalenderdatei (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> zu Ihren E-Mails und Landingpages hinzuzufügen.</td> 
  </tr> 
  <tr> 
   <td><p>Datum <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Dieses Token enthält einen Datumswert. Das Datum wird als Jahr-Monat-Tag angezeigt (z. B. 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Email-Skript <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token, um ein Velocity-Skript in Ihren E-Mails auszuführen. Weitere Informationen <a href="http://developers.marketo.com/documentation/email-scripting/" title="Link" rel="nofollow">hier</a>. </td> 
  </tr> 
  <tr> 
   <td>Number<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Jede Ganzzahl. Es kann sogar negativ sein.</td> 
  </tr> 
  <tr> 
   <td>Rich Text <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Das ist HTML. Verwenden Sie es in E-Mails und Landingpages.</td> 
  </tr> 
  <tr> 
   <td>Ergebnis <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token im Schritt <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">zum Ändern des Ergebnisablaufs</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC-Kampagne <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">Verwenden Sie dieses Token, um zu ermöglichen, dass Interessenten, die Teil eines Marketo-Programms werden, auch zu jeder SFDC-Kampagne hinzugefügt werden.</td> 
  </tr> 
  <tr> 
   <td>Text <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Nur etwas Text. Verwenden Sie sie, wenn HTML übertönen ist. Die maximale Textgröße beträgt 524.288 Zeichen (UTF-8) oder 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Meine Tokens werden nicht aufgelöst, wenn eine E-Mail von Sales Insight auf Microsoft Dynamics oder Salesforce gesendet wird. Es werden nur Standard-Token ausgefüllt (Interessent, Firma usw.). Die Standardwerte für Token _funktionieren jedoch_.

## Verschachtelungstoken {#nesting-tokens}

Wenn Sie ein neues Token erstellen, kann es von anderen Objekten in der Struktur referenziert werden. Es gibt eine Benennungsstruktur, bei der das Token zur einfachen Verwaltung erstellt wurde.

* **Lokales Token:** Das Token wurde direkt in diesem Programm oder Ordner erstellt.
* **Vererbtes Token:** Das Token wurde in einem Programm oder Ordner mit einer höheren Ebene in der Struktur erstellt.
* **Überschriebenes Token:** Das Token wurde geerbt und dann hat jemand in diesem Programm oder Ordner eine Ausnahme gemacht.

Sie können globale Variablen erstellen und diese dann auf niedrigeren Ebenen in der Struktur überschreiben.

Das Verschieben von Programmen und Ordnern wirkt sich auch auf Token aus. Vergewissern Sie sich stets, dass Verweise während des Verschiebevorgangs nicht beschädigt werden.

>[!NOTE]
>
>Wenn es sich bei der E-Mail, die Sie von einem Interaktions-Programm senden, um eine untergeordnete E-Mail eines standardmäßigen Programms handelt (nicht lokal zu Ihrem Interaktions-Programm), werden alle in der E-Mail verwendeten &quot;Meine Token&quot;aus dem Programm gelöst, in dem sich die untergeordnete E-Mail befindet.

>[!MORELIKETHIS]
>
>* [Tokens - Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [Verwalten von My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

