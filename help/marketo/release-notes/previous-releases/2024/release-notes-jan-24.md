---
description: Januar 2024 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – Januar 2024
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 7%

---

# Versionshinweise: Januar 2024 {#release-notes-jan-24}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Januar 2024 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 12. **2024 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>On-Demand-Webinare für interaktive Webinare</strong>: Mit On-Demand-Webinaren können Sie die Webinar-Aufzeichnung veröffentlichen und ihre Besuche/Aufrufe verfolgen. Auf diese Weise erhalten Sie weitere Leads durch Teilnehmer, die nicht am Webinar teilgenommen haben (nicht angezeigt), aber dennoch daran interessiert sind, weitere Details zu erfahren und die Aufzeichnung anzusehen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">On-Demand-Webinare</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Konversative Landingpages</strong>: Betten Sie einen Dynamic Chat-Konversationsfluss direkt in eine Marketo Engage-Landingpage ein, damit Besuchende ein Meeting per Dynamic Chat planen können, ohne ein Formular ausfüllen oder mit einem Chatbot interagieren zu müssen.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>E-Mail-Bot-Aktivität filtern</strong>: Verbessert die Erfassung von Bot-Aktivitäten für E-Mail-Interaktionen, indem Sie auswählen können, wie aggressiv die Filterung der Bot-Aktivität sein soll.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Bot-Aktivität für E-Mails filtern</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
    <tr> 
   <td><strong>API-Aktualisierung für den Massenimport von Leads</strong>: Das Verhalten der API für den Massenimport von Leads wurde geringfügig angepasst, wenn <b>id</b> bei der </b> der Auftragserstellung als <b>lookupField“ angegeben wird. Wenn ein mit der angegebenen <b>ID</b> verknüpfter Personendatensatz nicht in der Marketo Engage-Datenbank gefunden wird, erfolgt keine Datensatzaktualisierung, da der Datensatz nicht gefunden werden kann. Das aktualisierte Verhalten umfasst jetzt die Erhöhung der Anzahl in der <b>numOfRowsFailed</b>-Eigenschaft in der Antwort, wodurch signalisiert wird, dass der Vorgang in solchen Fällen fehlgeschlagen ist.</td> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
  <tr> 
   <td><strong>Co-Hosts für interaktive Webinare</strong>: Die Co-Hosts im Webinar-Team-Bereich interaktiver Webinare ermöglichen es dem Ersteller der Veranstaltung, interne oder externe Benutzer zum Programm für interaktive Webinare hinzuzufügen, um administrative und Bereitstellungs-Zuständigkeiten zu teilen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">Hinzufügen eines Webinar-Teams</a></td>
  </tr>
  <tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Benutzer in interaktiven Webinaren entfernen</strong>: Ein Marketo Engage-Administrator kann jetzt bestimmte Benutzer in interaktiven Webinaren entfernen.</td> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
 </tbody> 
</table>
<br/>

## Funktionen für Agile Versionen {#agile-release-features}

Alle unten aufgeführten Funktionen folgen einem Agile-Format und werden an verschiedenen Daten vor oder nach dem standardmäßigen Veröffentlichungsdatum veröffentlicht. Überprüfen Sie neben jeder Funktion auf ihren Status.

### Sales Insight-Aktionen {#sales-insight-actions}

![(Stern)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:15%">Status</th>
   <th style="width:20%">Dokumentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Erweiterbares Fenster erstellen</strong>: Das Fenster E-Mail erstellen komprimiert jetzt automatisch ungenutzten Platz, sodass der Editor mehr Platz hat. Darüber hinaus kann das Fenster noch weiter geöffnet werden, sodass die Benutzer so viel Platz haben, wie sie benötigen, um ihre E-Mails zu bearbeiten.</td> 
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
   <td><strong>Chatbot-Benutzeroberfläche für Conversational Forms</strong>: Website-Besuchende können jetzt Live-Chat in einem Conversational Flow anfordern.</td> 
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
   <td><strong>Chatbot-Schriftfarbenoptionen</strong>: Passen Sie Schriftfarben in einer Chatbot-Konfiguration an.</td> 
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
   <td><strong>Option zum Wiederholen des </strong>: Sie können jetzt ein Dialogfeld am Anfang neu starten, nachdem ein Besucher das Ende erreicht hat.</td> 
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
   <td><strong>Manuelle Beendigung des Live</strong>Chats: Sowohl Besucher als auch Agenten können jetzt eine Live-Chat-Sitzung manuell beenden.</td> 
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
   <td><strong>Letzte Marketo Engage-Aktivitäten im Agenten-Posteingang</strong>: Die letzten Marketo Engage-Aktivitäten, wie z. B. geöffnete E-Mails und ausgefüllte Formulare, werden für Leads im Agenten-Posteingang angezeigt.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Bedingte Verzweigung</strong>: Sie können Besuchenden jetzt unterschiedliche Konversationsinhalte anzeigen, die auf vordefinierten Bedingungen basieren, z. B. Besucherstandort oder Verfügbarkeit von Live-Agenten.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **One-Click List-Unsubscribe Update**: Gmail und Yahoo haben mehrere neue Absenderanforderungen implementiert, die am 1. Februar 2024 in Kraft traten. Erfahren Sie [was sie sind und wie sie sich auf Sie auswirken](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}.

* **Aktualisierung der Lead**: Das Verhalten [Lead-API synchronisieren](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"} wurde in Bezug auf Aktualisierungen des `unsubscribed` Felds leicht angepasst. Wenn Sie jetzt `null` als -Wert übergeben, ist dies gleich der Übergabe eines -Werts von `false`.

* **Marketo Engage Forms jQuery 1.x**: In unserer Version vom Januar 2024 aktualisieren wir die jQuery für das Marketo Engage von Forms auf jQuery 3.x. Dies kann sich auf die Implementierung benutzerdefinierter Formulare auswirken, die auf älteren Versionen von jQuery basieren. [Weitere Informationen finden Sie hier](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **E-Mail-Überprüfung nur für SSO-Benutzer**: Nur SSO-Benutzer wurden automatisch überprüft, sodass sie ein nicht zugängliches E-Mail-Konto verwenden können. Ab Mitte Januar werden alle bestehenden SSO Only-Benutzer nicht mehr verifiziert und werden über einen Link, den wir an das E-Mail-Konto senden, aufgefordert, ihre E-Mail erneut zu verifizieren. Alle neuen SSO-Benutzer müssen in Zukunft nur noch ihre E-Mail-Adressen verifizieren.

* Sehen Sie sich [ Webinar zur Marketo Engage vom Januar 2024 ](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}.
