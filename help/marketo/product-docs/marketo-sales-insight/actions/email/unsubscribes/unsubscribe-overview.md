---
description: Übersicht über die Abmeldung - Marketo-Dokumente - Produktdokumentation
title: Abmelde-Übersicht
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Abmelde-Übersicht {#unsubscribe-overview}

Es wird immer wichtiger, dass Unternehmen die Datenschutzgesetze für E-Mails einhalten. Um Ihnen dabei zu helfen, haben wir unsere Abmeldeerfahrung verbessert.

* Abmelde-Links werden in allen E-Mails platziert, die von Marketo Sales und Salesforce gesendet werden (dies gilt nicht für von Outlook oder Gmail gesendete benutzerdefinierte E-Mails).
* Administratoren können die Abmelde-Nachrichten für ihr gesamtes Team bearbeiten
* Abmeldeinformationen werden in PDV gespeichert.
* Abmeldungen können manuell vorgenommen werden: angeklickter Link, Salesforce-Synchronisation und Bounce
* Neue Landingpage für Abmelde-Links

## Abmelde-Link-Landingpage {#unsubscribe-link-landing-page}

Wenn eine Person auf Ihren Abmelde-Link klickt, wird sie auf eine Landingpage zum Abmelden weitergeleitet, auf der sie auswählen kann, von welcher Seite sie sich abmelden möchte und warum.

![](assets/unsubscribe-overview-1.png)

Diese Informationen werden in der Personendetailansicht gespeichert und können später angezeigt werden.

## Abmeldegruppe {#unsubscribe-group}

Sehen und verwalten Sie alle abgemeldeten Personen an einem Ort.

![](assets/unsubscribe-overview-2.png)

Verwenden Sie die Suchleiste, um nach allen abgemeldeten Personen zu suchen.

![](assets/unsubscribe-overview-3.png)

Wenn Sie Administrator sind, können Sie zur Gruppe &quot;Abmeldung&quot;wechseln, um nach &quot;Kontoabmeldungen&quot;zu filtern und alle Abmeldungen anzuzeigen, die in Ihrer Personendatenbank erfasst wurden.

![](assets/unsubscribe-overview-4.png)

## Verlauf der Abmeldung {#unsubscribe-history-card}

Die Karte Verlauf der Abmeldung hilft Administratoren und Benutzern, kontextbezogene Informationen über den Abmeldeverlauf ihrer Kontakte zu erhalten. Navigieren Sie dort zur Registerkarte Personen und wählen Sie eine Person aus. Sie befindet sich unten auf der Registerkarte Info in der Ansicht &quot;Persönliche Details&quot;.

>[!NOTE]
>
>Es gibt nur dann die Karte Verlauf des Abonnements abmelden , wenn die Person irgendwann _resubscribed_ hat.

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Datum</strong></td> 
   <td><p>Zeigt das Datum der Abmeldung/erneuten Anmeldung an.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Details</strong></td> 
   <td><p>Neu anmelden: Ein Sales Connect-Administrator hat die Abmeldung manuell aus dem Kontaktdatensatz entfernt. Es können auch einige Details angezeigt werden, die darauf hinweisen, warum sich der Kontakt abgemeldet hat.</p><p>Abmeldung: Der Kontakt wurde abgemeldet.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Quelle</strong></td> 
   <td><p>Salesforce Sync: Die Abmeldung wurde durch eine Synchronisation von Salesforce erfasst.</p><p>Manuell: Der Benutzer hat zum Abmelden auf die Schaltfläche zum Abmelden geklickt.</p><p>Angeklickter Link: Der Empfänger einer E-Mail hat auf den Abmelde-Link geklickt.</p><p>"Administratorname": Der Name eines Administrators wird angezeigt, wenn die Aktion darin bestand, Kontakte erneut anzumelden. Auf diese Weise können Benutzer wissen, wer die Abmeldung entfernt hat.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Nachricht zum Abmelden von Links anpassen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
