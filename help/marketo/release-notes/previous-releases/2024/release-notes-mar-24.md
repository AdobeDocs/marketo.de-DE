---
description: Versionshinweise - März 2024 - Marketo-Dokumente - Produktdokumentation
title: März 2024 - Versionshinweise
feature: Release Information
source-git-commit: c7359cc95a3e90f228353dc3d21c92712f9d5684
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 3%

---

# März 2024 - Versionshinweise {#release-notes-mar-24}

Unten finden Sie alle Funktionen der Version vom 24. März. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den Standard-Versionszyklus und werden ab der Veröffentlichung auf **8. März 2024**, mit einer stufenweisen Einführung der verbleibenden Funktionen in den darauffolgenden Wochen. Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr> 
   <td><strong>Erweiterte Konversationsflusslogik</strong>: Fügen Sie zusätzliche Felder zur Auswertung in einer einzigen Auswahl für die Weiterverfolgung von Konversationsströmen hinzu.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversionsflusseinstellungen für Marketo Engage Forms</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Konversionsflusslogik neu anordnen</strong>: In Marketo Engage Forms können Sie jetzt die Optionen für den Konversionsfluss neu anordnen, anstatt sie löschen und wieder hinzufügen zu müssen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversionsflusseinstellungen für Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API-Aktivitätsmetadaten</strong>: Metadaten wie Benutzeragent, Plattform und Gerät sind jetzt in Web- und E-Mail-Aktivitäten enthalten, was dazu beiträgt, über die Marketo REST-API konsistente Einblicke in diese Aktivitäten zu erhalten.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **API-Fehlerbehebung für Programmteilnehmer abrufen**: Kürzlich wurde eine Änderung vorgenommen, um das Verhalten der [Abrufen von Programmmitgliedern](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} -Endpunkt. Bisher wurde bei Verwendung der Variablen `updatedAt` Filtertyp, um einen Datumsbereich anzugeben, bestand die Möglichkeit, dass in diesem Bereich aktualisierte Programmmitgliedschaftsdatensätze nicht in der Antwort enthalten waren. Darüber hinaus bestand die Möglichkeit, dass außerhalb des angegebenen Datumsbereichs aktualisierte Programmmitgliedschaftsdatensätze fälschlicherweise in die Antwort aufgenommen wurden. Beide Probleme wurden behoben.

* **Einstellung des Kontoinsight-Browser-Plug-ins**: Adobe entfernt die Target-Kontoverwaltung [Account Insight-Browser-Plugin](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on March 18, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.