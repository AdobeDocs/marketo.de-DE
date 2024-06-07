---
unique-page-id: 1147114
description: Grundlegendes zu meinen Token in einem Programm - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zu meinen Token in einem Programm
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 3%

---

# Grundlagen zu meinen Token in einem Programm {#understanding-my-tokens-in-a-program}

Ein Token ist eine Variable, die Sie in E-Mails, Landingpages und Smart-Kampagnen verwenden können, um Ihr Leben zu vereinfachen.

Neben My Tokens können Sie auch beliebige der integrierten Token in Ihren Programmen verwenden. Sehen Sie sich die [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

## Meine Token  {#my-tokens}

Meine Token sind benutzerdefinierte Variablen, die jeder erstellen kann. Sie sind [created](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} in Kampagnenordnern oder -programmen.

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
   <td>Verwenden Sie dieses Token zum <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">Hinzufügen einer Kalenderereignisdatei (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> auf Ihre E-Mails und Landingpages.</td> 
  </tr> 
  <tr> 
   <td><p>Datum <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Dieses Token enthält einen Datumswert. Das Datum wird als Jahr-Monat-Tag angezeigt (z. B. 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>E-Mail-Script <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token, um ein Velocity-Skript in Ihren E-Mails auszuführen. Weitere Infos <a href="https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting" title="Link folgen" rel="nofollow">here</a>. </td> 
  </tr> 
  <tr> 
   <td>Zahl<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Beliebige Ganzzahlen. Es kann sogar negativ sein.</td> 
  </tr> 
  <tr> 
   <td>RTF <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Das ist HTML. Verwenden Sie sie in E-Mails und Landingpages.</td> 
  </tr> 
  <tr> 
   <td>Bewertung <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Verwenden Sie dieses Token im <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">Schritt zum Wechseln des Punktflusses</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC-Kampagne <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">Verwenden Sie dieses Token, damit Leads, die Teil eines Marketo-Programms werden, auch zu jeder SFDC-Kampagne hinzugefügt werden können.</td> 
  </tr> 
  <tr> 
   <td>Text <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Nur etwas Text. Verwenden Sie es, wenn HTML übertötet ist. Die maximale Größe für Text-Token beträgt 524.288 Zeichen (UTF-8) oder 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Meine Token werden beim Senden einer E-Mail aus Sales Insight auf Microsoft Dynamics oder Salesforce nicht aufgelöst. Es werden nur Standard-Token (Lead, Unternehmen usw.) ausgefüllt. Standardwerte für Token _will_ funktioniert.

## Verschachtelungstoken {#nesting-tokens}

Wenn Sie ein neues Token erstellen, kann es von anderen Objekten in der Struktur referenziert werden. Es gibt eine Namensstruktur, in der das Token zur einfachen Verwaltung erstellt wurde.

* **Lokaler Token:** Das Token wurde direkt in diesem Programm oder Ordner erstellt.
* **Vererbter Token:** Das Token wurde im Baum irgendwo in einem Programm oder Ordner mit höherer Ebene erstellt.
* **Überschriebenes Token:** Das Token wurde vererbt und dann hat jemand in diesem Programm oder Ordner eine Ausnahme gemacht.

Sie können globale Variablen erstellen und diese dann auf niedrigeren Ebenen im Baum überschreiben.

Das Verschieben von Programmen und Ordnern wirkt sich auch auf Token aus. Vergewissern Sie sich stets, dass die Verweise während des Verschiebevorgangs nicht beschädigt werden.

>[!NOTE]
>
>Wenn es sich bei der von einem Interaktionsprogramm gesendeten E-Mail um eine untergeordnete E-Mail eines Standardprogramms handelt (nicht lokal für Ihr Interaktionsprogramm), werden alle in der E-Mail verwendeten My Tokens aus dem Standardprogramm aufgelöst, in dem sich die untergeordnete E-Mail befindet.

>[!MORELIKETHIS]
>
>* [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Verwalten von My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
