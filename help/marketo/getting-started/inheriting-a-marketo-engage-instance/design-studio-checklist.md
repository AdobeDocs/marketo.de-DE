---
description: Checkliste für geerbtes Instanzdesign Studio - Marketo Docs - Produktdokumentation
title: Checkliste für geerbtes Instanzdesign Studio
feature: Getting Started
exl-id: 41e89120-4ac0-4e70-bed0-da4e5c5542ff
source-git-commit: 2c74c71c9311312f7e0991ed5598ccb09a9b1f15
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 4%

---

# Vererbte Instanz: Design Studio Checkliste {#inherited-instance-design-studio-checklist}

Die Strukturierung von Vorlagen und das Erstellen globaler Formulare, Snippets sowie Bilder und Dateien tragen dazu bei, Datenfehler zu minimieren und den Arbeitsablauf für Ihren Programmaufbau zu optimieren. Denken Sie daran, [die Checklisten herunterzuladen](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) und Ihren Fortschritt zu verfolgen.

## Landing Page {#landing-pages}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Globale Landing Pages</td> 
   <td><li>Wie viele globale <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages.md" target="_blank">Einstiegsseiten</a> gibt es? Werden sie von Programmen genutzt?</li>
   <li>Ist ein <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-learn.html" target="_blank">Abonnement-Center</a> eingerichtet?
   <br/>     Ist dies nicht der Fall, können Sie eine erstellen.</li></td>
  </tr>
  <tr> 
   <td>Vorlagen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.md" target="_blank">Landingpage-Vorlagen</a> gibt es? Werden sie genutzt?</li></td>
  </tr>
  <tr> 
   <td>Testgruppen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups.md" target="_blank">Einstiegsseitentestgruppen</a> sind sie? Sind sie alle noch relevant?</li></td>
  </tr>
   <tr> 
   <td>Datenschutz und Compliance</td> 
   <td><li>Haben alle Ihre Landingpages die entsprechenden Fußzeilen?</li></td>
  </tr>
 </tbody> 
</table>

## Bilder und Dateien {#images-and-files}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Benennungskonventionen</td> 
   <td><li>Verfügen <a href="/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md" target="_blank">Bilder und Dateien</a> über konsistente Namenskonventionen?</li></td>
  </tr>
  <tr> 
   <td>Ordnerstruktur</td> 
   <td><li>Sind Bilder und Dateien <a href="/help/marketo/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders.md" target="_blank">angemessen organisiert</a> und leicht zu durchsuchen?</li></td>
  </tr>
  <tr> 
   <td>Bilder und Dateien</td> 
   <td><li>Müssen Bilder oder Dateien, auf die <a href="/help/marketo/product-docs/demand-generation/images-and-files/find-the-url-of-an-uploaded-image-or-file.md" target="_blank">auf Webseiten verwiesen wird</a>, aktualisiert werden? 
   <p>Beispiel: Die hartcodierte URL-Struktur <a href="https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632#_Toc54870361" target="_blank"> muss möglicherweise aktualisiert werden</a>, z. B. <code>http://na-sj01.marketo.com/rs/123-ABC-456/images/puppy.png</code>. 
   <p>Arbeiten Sie mit Ihrem Web-Entwickler zusammen, um festzustellen, wo Sie möglicherweise Updates vornehmen müssen.</li></td>
  </tr>
 </tbody> 
</table>

## Formulare {#forms}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Globale Formulare</td> 
   <td><li>Wie viele globale <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md" target="_blank">Formulare</a> gibt es?</li>
<li>Verwenden die meisten Programme globale oder lokale Formulare?</li>
<li>Sammeln alle Formulare die richtigen Daten für Marketing und Vertrieb?</li>
<li>Werden versteckte Werte entsprechend genutzt?</li>
<li>Werden Marketo Engage-Formulare auf Nicht-Marketo Engage-Landingpages verwendet? Wie werden sie referenziert?</li>
<p><img src="assets/tip-icon.png" alt="Tippsymbol">TIPP: Aktualisieren Sie Seiten, auf denen Sie Marketo Engage-Formulare einbetten, mit dem neuen Einbettungscode (gesicherte Landingpages sind erforderlich).
<p><a href="/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/design-studio-checklist-2.png" target="_blank"><img src="assets/design-studio-checklist-1.png" alt="Code-Miniatur"></a>
</td>
  </tr>
  <tr> 
   <td>Datenstandardisierung</td> 
   <td><li>Sind Ihre <a href="/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md" target="_blank">Formularfelder</a> hauptsächlich Auswahllisten oder geöffnete Textfelder?</li>
<p><img src="assets/tip-icon.png" alt="Tippsymbol">TIPP: Wenn es sich um offene Textfelder handelt, sollten Sie sie zu Auswahllisten wechseln, um unsaubere Daten zu verhindern.</td>
  </tr>
  <tr> 
   <td>Datenschutz und Compliance</td> 
   <td><li>Entspricht Ihre Formularstrategie Ihren Anforderungen an den Datenschutz und die Anmeldung von Unternehmensdaten? 
   <br/>     Zur Einhaltung der Vorschriften sollten Sie die <a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">Datenschutz-Grundverordnung (DSGVO)</a>, das kanadische Anti-Spam-Gesetz (CASL), den Controlling the Assault of Non-Solicited Pornography and Marketing Act von 2003 (CAN-SPAM), den California Consumer Privacy Act (CCPA) usw. beachten.</li>
<p><img src="assets/tip-icon.png" alt="Tippsymbol">Tipp: Denken Sie daran, sich zu diesen Fragen immer an Ihr Rechtsabteilung zu wenden. Fragen Sie Ihr Team nach früheren Initiativen, um die Einhaltung zu gewährleisten, bevor Sie Änderungen vornehmen.</td>
  </tr>
 </tbody> 
</table>

## E-Mails {#emails}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Globale E-Mails</td> 
   <td><li>Wie viele globale <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md" target="_blank">E-Mails</a> gibt es? Werden sie von Programmen genutzt?</li></td>
  </tr>
  <tr> 
   <td>Vorlagen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md" target="_blank">E-Mail-Vorlagen</a> gibt es? Werden sie genutzt?</li></td>
  </tr>
  <tr> 
   <td>E-Mail-Tests</td> 
   <td><li>Wie werden <a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/understanding-email-testing-options.md" target="_blank">E-Mail-Tests</a> verwendet? Ist Ihre Methode noch effektiv?</li></td>
  </tr>
  </tr>
  <tr> 
   <td>Datenschutz und Compliance</td> 
   <td><li>Haben alle Ihre E-Mails die entsprechenden Fußzeilen? Betrachten Sie DSGVO, CASL, CAN-SPAM, CCPA usw. für die Einhaltung der Vorschriften.</li>
<p><img src="assets/tip-icon.png" alt="Tippsymbol">Tipp: Denken Sie daran, sich immer an Ihr Rechtsabteilung zu diesen Compliance-Fragen zu wenden. Fragen Sie Ihr Team nach früheren Initiativen, um die Einhaltung zu gewährleisten, bevor Sie Änderungen vornehmen.</td>
  </tr>
 </tbody> 
</table>

## Ausschnitte {#snippets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Ausschnitte</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md" target="_blank">Snippets</a> gibt es? Werden sie verwendet? 
   <br/>     Wenn nicht, sollten Sie sie für den Fußzeileninhalt <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md" target="_blank">E-Mail</a> und den Fußzeileninhalt <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page.md" target="_blank">Landingpage</a>, Logos und mehr verwenden.</li></td>
  </tr>
 </tbody> 
</table>

## Alle Assets {#all-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Asset-Status</td> 
   <td><li>Wie viele Assets befinden sich im Status <i>Entwurf</i> und <i>Genehmigt mit Entwurf</i> (z. B. <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md" target="_blank">E-Mails</a>, <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md#approve-a-landing-page" target="_blank">Einstiegsseiten</a>, <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/approve-a-form.md" target="_blank">Formulare</a>, <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/approve-a-snippet.md" target="_blank">Ausschnitte</a>)?
   <br/>     Wenn es viele gibt, sollten Sie sie löschen oder genehmigen.</li></td>
  </tr>
  <tr> 
   <td>Asset-Freigabe</td> 
   <td><li>Welche Assets werden <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md#sharing-across-workspaces" target="_blank">über Workspaces</a> hinweg freigegeben?</li>
   <p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Es ist wichtig, dies zu wissen, da in einer Workspace durchgeführte Aktionen dazu führen können, dass ein Asset in einer anderen Workspace für einen anderen Benutzer nicht zugänglich ist.</td>
  </tr>
 </tbody> 
</table>
