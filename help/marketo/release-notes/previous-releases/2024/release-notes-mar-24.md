---
description: März 2024 - Versionshinweise zu Marketo - Produktdokumentation
title: März 2024 - Versionshinweise
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: fd92f5307880019f54bb2f1778093c110a53ed2c
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 3%

---

# März 2024 - Versionshinweise {#release-notes-mar-24}

Unten finden Sie alle Funktionen, die in der Version vom 24. März enthalten sind. Überprüfen Sie die Verfügbarkeit der Funktionen in Ihrer Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![Stern](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den Standard-Veröffentlichungszyklus und werden ab dem veröffentlicht. **8. März 2024**, mit einem schrittweisen Rollout der verbleibenden Funktionen in den folgenden Wochen. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr> 
   <td><strong>Erweiterte Konversationsflusslogik</strong>: Zusätzliche Felder zur Auswertung in einer einzigen Auswahl für die Konversationsfluss-Nachverfolgung hinzufügen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversationsflusseinstellungen für Marketo Engage Forms</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Neuanordnung der Konversationsflusslogik</strong>: Beim Marketo Engage von Forms können Sie jetzt die Auswahl des Konversionsflusses neu anordnen, anstatt ihn löschen und wieder hinzufügen zu müssen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversationsflusseinstellungen für Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API-Aktivitätsmetadaten</strong>: Metadaten wie Benutzeragent, Plattform und Gerät sind jetzt in Web- und E-Mail-Aktivitäten enthalten, was über die Marketo REST-API zu konsistenten Einblicken in diese Aktivitäten beiträgt.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Abrufen der API-Fehlerbehebung für Programmteilnehmer**: Kürzlich wurde eine Änderung vorgenommen, um das Verhalten der [Abrufen von Programmmitgliedern](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} Endpunkt. Zuvor bei Verwendung von `updatedAt` Filtertyp Um einen Datumsbereich anzugeben, bestand die Möglichkeit, dass in diesem Bereich aktualisierte Programmmitgliedschaftsdatensätze nicht in der Antwort enthalten waren. Darüber hinaus bestand die Möglichkeit, dass Programmmitgliedschaftsdatensätze, die außerhalb des angegebenen Datumsbereichs aktualisiert wurden, fälschlicherweise in der Antwort enthalten waren. Beide Probleme wurden behoben.

* **Einstellung des Account Insight Browser-Plug-ins**: Adobe entfernt die Target-Kontoverwaltung [Account Insight Browser-Plug-in](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on April 8, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
