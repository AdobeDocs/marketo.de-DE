---
description: Übersicht über die Abmeldung - Marketo-Dokumente - Produktdokumentation
title: Übersicht über die Abmeldung
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Übersicht über die Abmeldung {#unsubscribe-overview}

Für Unternehmen wird es immer wichtiger, die Datenschutzgesetze für E-Mails einzuhalten. Um Ihnen dabei zu helfen, haben wir einige Verbesserungen an unserem Abmeldeerlebnis vorgenommen.

* Abmelde-Links werden in allen E-Mails platziert, die von [!DNL Marketo Sales] und [!DNL Salesforce] gesendet werden (dies gilt nicht für benutzerdefinierte E-Mails, die von [!DNL Outlook] oder Gmail gesendet werden)
* Administratoren können Nachrichten zur Abmeldung für ihr gesamtes Team bearbeiten
* Abmeldeinformationen werden in PDV gespeichert
* Abmeldungen können manuell erfolgen: angeklickter Link, [!DNL Salesforce] Synchronisierung und Bounce
* Neuer Abmelde-Link für Landingpage

## Abmelde-Link-Landingpage {#unsubscribe-link-landing-page}

Wenn eine Person auf Ihren Abmelde-Link klickt, wird sie zu einer Landingpage weitergeleitet, auf der sie auswählen kann, wofür sie sich abmelden möchte und warum.

![](assets/unsubscribe-overview-1.png)

Diese Informationen werden in der Ansicht „Personendetails“ gespeichert, um sie später anzuzeigen.

## Gruppe abmelden {#unsubscribe-group}

Alle abgemeldeten Personen an einem Ort anzeigen und verwalten.

![](assets/unsubscribe-overview-2.png)

Verwenden Sie die Suchleiste, um nach abgemeldeten Personen zu suchen.

![](assets/unsubscribe-overview-3.png)

Wenn Sie Administrator sind, können Sie zur Abmeldegruppe gehen, um nach [!UICONTROL Konto-Abmeldungen] zu filtern und alle Abmeldungen anzuzeigen, die in Ihrer Personendatenbank erfasst wurden.

![](assets/unsubscribe-overview-4.png)

## Verlaufskarte für Abmeldung {#unsubscribe-history-card}

Die Karte [!UICONTROL Abmeldeverlauf] hilft Admins und Benutzern, kontextuelle Informationen über den Abmeldeverlauf ihrer Kontakte zu erhalten. Navigieren Sie dorthin, indem Sie zur Registerkarte [!UICONTROL Personen] wechseln und eine Person auswählen. Er befindet sich am unteren Rand der Registerkarte [!UICONTROL Info] in der Ansicht „Personendetails“.

>[!NOTE]
>
>Es wird nur dann eine Karte [!UICONTROL Abmeldeverlauf] geben, wenn sich die Person _einmal_ hat.

![](assets/unsubscribe-overview-5.png)

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>[!UICONTROL Datum]</strong></td>
   <td><p>Zeigt das Datum, an dem das Abmelden/erneute Abonnieren stattgefunden hat.</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Details]</strong></td>
   <td><p>Erneut abonnieren: Ein [!DNL Sales Connect] hat die Abmeldung manuell aus dem Kontaktdatensatz entfernt. Möglicherweise werden auch Details zu den Gründen angezeigt, aus denen der Kontakt das Abonnement gekündigt hat.</p><p>Abo beenden: Das Abonnement des Kontakts wurde gekündigt.</p></td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td><p>[!DNL Salesforce] Synchronisierung: Die Abmeldung wurde von einer Synchronisierung mit [!DNL Salesforce] erfasst.</p><p>Manuell: Benutzende haben auf die Schaltfläche zum Abmelden geklickt, um sich abzumelden.</p><p>Angeklickter Link: Empfänger einer E-Mail hat auf den Abmelde-Link geklickt.</p><p>„Admin-Name“: Der Name eines Administrators wird angezeigt, wenn die Aktion zum erneuten Abonnieren von Kontakten ausgeführt wurde. Auf diese Weise erfahren Benutzende, wer die Abmeldung entfernt hat.</p></td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Abmelde-Link-Nachricht anpassen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
