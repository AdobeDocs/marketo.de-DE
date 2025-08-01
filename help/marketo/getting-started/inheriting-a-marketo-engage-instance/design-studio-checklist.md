---
description: Checkliste für das Design von geerbten Instanzen - Marketo-Dokumente - Produktdokumentation
title: Checkliste für das Design Studio der geerbten Instanz
feature: Getting Started
exl-id: 41e89120-4ac0-4e70-bed0-da4e5c5542ff
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 4%

---

# Vererbte Instanz: Design Studio-Checkliste {#inherited-instance-design-studio-checklist}

Das Strukturieren von Vorlagen und das Erstellen globaler Formulare, Snippets sowie Bilder und Dateien trägt dazu bei, Datenfehler zu minimieren und den Workflow für die Erstellung Ihres Programms zu optimieren. Denken Sie daran[ die Checklisten herunterzuladen ](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) Ihren Fortschritt zu verfolgen.

## Landingpages {#landing-pages}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Globale Landing Pages</td>
   <td><li>Wie viele globale <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages.md" target="_blank">Landingpages</a> gibt es? Werden sie von Programmen verwendet?</li>
   <li>Haben Sie ein <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-learn.html?lang=de" target="_blank">Abonnementzentrum</a> eingerichtet?
   <br/>     Wenn nicht, sollten Sie eine erstellen.</li></td>
  </tr>
  <tr>
   <td>Vorlagen</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.md" target="_blank">Landingpage-Vorlagen</a> gibt es? Werden sie wirksam eingesetzt?</li></td>
  </tr>
  <tr>
   <td>Testgruppen</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups.md" target="_blank">Landingpage-Testgruppen</a> sind das? Sind sie alle noch relevant?</li></td>
  </tr>
   <tr>
   <td>Datenschutz und Compliance</td>
   <td><li>Verfügen alle Landingpages über die entsprechenden Fußzeilen?</li></td>
  </tr>
 </tbody>
</table>

## Bilder und Dateien {#images-and-files}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Benennungskonventionen</td>
   <td><li>Haben <a href="/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md" target="_blank">Bilder und Dateien</a> konsistente Benennungskonventionen?</li></td>
  </tr>
  <tr>
   <td>Ordnerstruktur</td>
   <td><li>Sind Bilder und Dateien <a href="/help/marketo/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders.md" target="_blank">angemessen organisiert</a> und leicht zu durchsuchen?</li></td>
  </tr>
  <tr>
   <td>Bilder und Dateien</td>
   <td><li>Müssen Bilder oder Dateien <a href="/help/marketo/product-docs/demand-generation/images-and-files/find-the-url-of-an-uploaded-image-or-file.md" target="_blank">auf Webseiten referenziert</a> aktualisiert werden?
   <p>Beispiel: Die hartcodierte URL<a href="https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632#_Toc54870361" target="_blank">Struktur muss möglicherweise aktualisiert werden</a> z. B. <code>http://na-sj01.marketo.com/rs/123-ABC-456/images/puppy.png</code>.
   <p>Bitte wenden Sie sich an Ihren Web-Entwickler, um zu ermitteln, wo Sie möglicherweise Aktualisierungen vornehmen müssen.</li></td>
  </tr>
 </tbody>
</table>

## Formulare {#forms}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Globale Formulare</td>
   <td><li>Wie viele globale <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md" target="_blank">Formulare</a> gibt es?</li>
<li>Verwenden die meisten Programme globale oder lokale Formulare?</li>
<li>Sammeln alle Formulare die richtigen Daten für Marketing und Vertrieb?</li>
<li>Werden ausgeblendete Werte angemessen genutzt?</li>
<li>Werden Marketo Engage-Formulare auf Landingpages von anderen Anbietern als Marketo Engage verwendet? Wie wird auf sie verwiesen?</li>
<p><img src="assets/tip-icon.png" alt="Tipp-Symbol">TIPP: Aktualisieren Sie die Seiten, auf denen Sie Marketo Engage-Formulare einbetten, mit dem neuen Einbettungs-Code, der eingeführt wurde (sichere Landingpages sind erforderlich).
<p><a href="/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/design-studio-checklist-2.png" target="_blank"><img src="assets/design-studio-checklist-1.png" alt="Codeminiatur"></a>
</td>
  </tr>
  <tr>
   <td>Datenstandardisierung</td>
   <td><li>Sind Ihre <a href="/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md" target="_blank">Formularfelder</a> in erster Linie Auswahllisten oder offene Textfelder?</li>
<p><img src="assets/tip-icon.png" alt="Tipp-Symbol">TIPP: Wenn es sich um offene Textfelder handelt, sollten Sie diese ggf. auf Auswahllisten umstellen, um unübersichtliche Daten zu verhindern.</td>
  </tr>
  <tr>
   <td>Datenschutz und Compliance</td>
   <td><li>Entspricht Ihre Formularstrategie den Datenschutz- und Opt-in-Anforderungen Ihres Unternehmens?
   <br/>     Man betrachte etwa <a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">Datenschutz-Grundverordnung (DSGVO)</a>, das kanadische Anti-Spam-Gesetz (CASL), den Controlling the Assault of Non-Solicited Pornografy and Marketing Act von 2003 (CAN-SPAM), den California Consumer Privacy Act (CCPA) usw., um die Einhaltung der Vorschriften zu gewährleisten.</li>
<p><img src="assets/tip-icon.png" alt="Tipp-Symbol">TIPP: Vergessen Sie nicht, sich in diesen Fragen immer an Ihre Rechtsabteilung zu wenden. Fragen Sie Ihr Team nach früheren Initiativen, um die Compliance aufrechtzuerhalten, bevor Sie Änderungen vornehmen.</td>
  </tr>
 </tbody>
</table>

## E-Mails {#emails}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Globale E-Mails</td>
   <td><li>Wie viele globale <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md" target="_blank">E</a>Mails gibt es? Werden sie von Programmen verwendet?</li></td>
  </tr>
  <tr>
   <td>Vorlagen</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md" target="_blank">E-Mail</a>Vorlagen gibt es? Werden sie wirksam eingesetzt?</li></td>
  </tr>
  <tr>
   <td>E-Mail-Tests</td>
   <td><li>Wie verwenden Sie <a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/understanding-email-testing-options.md" target="_blank">E-Mail-Tests</a>? Ist Ihre Methode noch wirksam?</li></td>
  </tr>
  </tr>
  <tr>
   <td>Datenschutz und Compliance</td>
   <td><li>Haben alle E-Mails die entsprechenden Fußzeilen? Berücksichtigen Sie die DSGVO, CASL, CAN-SPAM, CCPA usw. Auswirkungen auf die Compliance.</li>
<p><img src="assets/tip-icon.png" alt="Tipp-Symbol">TIPP: Vergessen Sie nicht, sich bezüglich dieser Compliance-Fragen immer an Ihre Rechtsabteilung zu wenden. Fragen Sie Ihr Team nach früheren Initiativen, um die Compliance aufrechtzuerhalten, bevor Sie Änderungen vornehmen.</td>
  </tr>
 </tbody>
</table>

## Snippets {#snippets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Snippets</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md" target="_blank">Snippets</a> gibt es? Werden sie verwendet?
   <br/>     Wenn nicht, sollten Sie sie für <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md" target="_blank">E-Mail</a> und <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page.md" target="_blank">Landingpage</a> Fußzeileninhalte, Logos und mehr verwenden.</li></td>
  </tr>
 </tbody>
</table>

## Alle Assets {#all-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Asset-Status</td>
   <td><li>Wie viele Assets befinden sich im Status <i>Entwurf</i> und <i>Genehmigt mit Entwurf</i> (z. B. <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md" target="_blank">E-Mails</a>, <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md#approve-a-landing-page" target="_blank">Landingpages</a>, <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/approve-a-form.md" target="_blank">Formulare</a>, <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/approve-a-snippet.md" target="_blank"></a>)?
   <br/>     Wenn viele vorhanden sind, sollten Sie sie löschen oder genehmigen.</li></td>
  </tr>
  <tr>
   <td>Asset-Freigabe</td>
   <td><li>Welche Assets werden <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md#sharing-across-workspaces" target="_blank">über Arbeitsbereiche hinweg freigegeben</a>?</li>
   <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Es ist wichtig zu wissen, dass Aktionen, die in einer Workspace durchgeführt werden, dazu führen können, dass ein Asset in einer anderen Workspace für einen anderen Benutzer nicht zugänglich ist.</td>
  </tr>
 </tbody>
</table>
