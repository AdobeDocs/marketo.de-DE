---
description: Januar 2024 - Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Januar 2024 - Versionshinweise
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 6%

---

# Januar 2024 - Versionshinweise {#release-notes-jan-24}

Unten finden Sie alle Funktionen der Version vom 24. Januar. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Versionszyklus und werden am **12. Januar 2024** veröffentlicht. Der Rollout der verbleibenden Funktionen erfolgt schrittweise in den darauffolgenden Wochen. Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>On-Demand-Webinare für interaktive Webinare</strong>: Mit On-Demand-Webinaren können Sie die Webinaraufzeichnung veröffentlichen und ihre Besuche/Uhren verfolgen. Dies hilft Ihnen, mehr Leads durch Registrierungspflichtige zu erhalten, die nicht am Webinar teilgenommen haben (keine Sendung), aber trotzdem daran interessiert sind, mehr Details zu erhalten und die Aufzeichnung anzuzeigen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">On-Demand-Webinare</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Konversative Einstiegsseiten</strong>: Betten Sie einen Dynamic Chat-Konversationsfluss direkt in eine Marketo Engage-Einstiegsseite ein, damit Besucher ein Treffen über Dynamic Chat planen können, ohne ein Formular ausfüllen oder mit einem Chat interagieren zu müssen.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Filtern der E-Mail-Bot-Aktivität</strong>: Verbessert die Erfassung von Bot-Aktivitäten für E-Mail-Interaktionen, indem Sie auswählen können, wie aggressiv die Filterung der Bot-Aktivitätserkennung sein soll.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtern der E-Mail-Bot-Aktivität</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
    <tr> 
   <td><strong>Aktualisierung der Bulk-Lead-Import-API</strong>: Das Verhalten der Bulk-Lead-Import-API wurde geringfügig angepasst, wenn <b>id</b> bei der Auftragserstellung als <b>lookupField</b> angegeben wurde. Wenn ein mit der bereitgestellten <b>id</b> verknüpfter Personendatensatz nicht in der Marketo Engage-Datenbank gefunden wird, erfolgt keine Aktualisierung des Datensatzes, da der Datensatz nicht gefunden werden kann. Das aktualisierte Verhalten umfasst nun die Erhöhung der Anzahl in der Eigenschaft <b>numOfRowsFailed</b> innerhalb der Antwort und weist darauf hin, dass der Vorgang in solchen Fällen fehlgeschlagen ist.</td> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
  <tr> 
   <td><strong>Co-Hosts für interaktive Webinare</strong>: Mithilfe von Hosts im Bereich Webinar-Team der interaktiven Webinare kann der Ersteller von Ereignissen interne oder externe Benutzer zum Programm der interaktiven Webinare hinzufügen, um Verwaltungs- und Bereitstellungsaufgaben zu teilen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">Webinar-Team hinzufügen</a></td>
  </tr>
  <tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Einen Benutzer in interaktiven Webinaren entfernen</strong>: Ein Marketo Engage-Administrator kann jetzt einen oder mehrere Benutzer in interaktiven Webinaren entfernen.</td> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
 </tbody> 
</table>
<br/>

## Agile Release-Funktionen {#agile-release-features}

Alle unten aufgeführten Funktionen entsprechen dem Agile-Format und werden an verschiedenen Daten vor oder nach dem standardmäßigen Veröffentlichungsdatum veröffentlicht. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

### Sales Insight-Aktionen {#sales-insight-actions}

![(star)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:15%">Status</th>
   <th style="width:20%">Dokumentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Fenster zum Erstellen erweitern</strong>: Das Fenster zum Erstellen einer E-Mail komprimiert jetzt automatisch nicht verwendeten Speicherplatz, wodurch mehr Platz im Editor verfügbar ist. Darüber hinaus kann das Fenster geöffnet und erweitert werden, sodass Benutzer so viel Platz haben, wie sie benötigen, um ihre E-Mails zu bearbeiten.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>
  </tbody> 
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:15%">Status</th>
   <th style="width:20%">Dokumentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Chatbot-Benutzeroberfläche für Conversational Forms</strong>: Website-Besucher können jetzt einen Live-Chat in einem Konversationsfluss anfordern.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Chatbot Font Color Options</strong>: Passen Sie Schriftfarben in einer Chatbot-Konfiguration an.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Option zum Wiederholen des Dialogfelds</strong>: Sie können jetzt einen Dialog zu Beginn neu starten, nachdem ein Besucher das Ende erreicht hat.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Manuelles Beenden des Live-Chat</strong>: Sowohl Besucher als auch Agenten können jetzt eine Live-Chat-Sitzung manuell beenden.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">Agenten-Posteingang</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Letzte Marketo Engage-Aktivitäten im Agent-Posteingang</strong>: Letzte Marketo Engage-Aktivitäten wie "Geöffnete E-Mail"und "Ausgefülltes Formular"werden für Leads im Agenten-Posteingang angezeigt.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Bedingte Verzweigung</strong>: Sie können Besuchern nun unterschiedliche Konversationsinhalte basierend auf vordefinierten Bedingungen anzeigen, z. B. den Standort des Besuchers oder die Verfügbarkeit von Live-Agenten.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **One-Click List-Unsubscribe Update**: Gmail und Yahoo haben mehrere neue Absenderanforderungen implementiert, die am 1. Februar 2024 in Kraft traten. Erfahren Sie [was sie sind und wie sie sich auf Sie auswirken](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}.

* **Lead-API-Update synchronisieren**: Das Verhalten der [Lead-API synchronisieren](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"} wurde in Bezug auf Aktualisierungen am Feld `unsubscribed` geringfügig angepasst. Wenn Sie jetzt `null` als Wert übergeben, ist es gleich der Übergabe eines Werts von `false`.

* **Marketo Engage Forms jQuery 1.x**: In unserer Version vom Januar 2024 aktualisieren wir jQuery für Marketo Engage Forms auf jQuery 3.x. Dies kann sich auf die Implementierung benutzerdefinierter Formulare auswirken, die auf älteren jQuery-Versionen basieren. [Weitere Informationen finden Sie hier](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **E-Mail-Überprüfung für Benutzer mit SSO-Berechtigung**: Nur Benutzer mit SSO, die zuvor automatisch überprüft wurden, sodass sie ein nicht zugängliches E-Mail-Konto verwenden können. Ab Mitte Januar werden alle bestehenden Benutzer von SSO Only nicht mehr überprüft und aufgefordert, ihre E-Mail über einen Link, den wir an das E-Mail-Konto senden, zu überprüfen. Alle neuen Benutzer von SSO Nur Benutzer müssen ihre E-Mail-Adressen in Zukunft überprüfen.

* Sehen Sie sich das Webinar ](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"} zur Marketo Engage-Version vom [Januar 2024 an.
