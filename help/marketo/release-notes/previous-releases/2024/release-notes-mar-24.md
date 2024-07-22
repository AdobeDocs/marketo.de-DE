---
description: Versionshinweise - März 2024 - Marketo-Dokumente - Produktdokumentation
title: März 2024 - Versionshinweise
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 2%

---

# März 2024 - Versionshinweise {#release-notes-mar-24}

Unten finden Sie alle Funktionen der Version vom 24. März. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Versionszyklus und werden ab dem 8. März 2024 veröffentlicht. Außerdem wird in den folgenden Wochen ein stufenweiser Rollout der verbleibenden Funktionen veröffentlicht. **** Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr> 
   <td><strong>Erweiterte Konversationsflusslogik</strong>: Fügen Sie zusätzliche Felder zur Auswertung in einer einzigen Auswahl für die Weiterverfolgung des Konversationsflusses hinzu.</td> 
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
   <td><strong>Konversionsflusslogik neu anordnen</strong>: In Marketo Engage Forms können Sie jetzt die Konversionsflussoptionen neu anordnen, anstatt sie löschen und wieder hinzufügen zu müssen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversionsflusseinstellungen für Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API Activity Metadata</strong>: 
   Metadaten wie Benutzeragent, Plattform und Gerät sind jetzt in Web- und E-Mail-Aktivitäten enthalten, was dazu beiträgt, über die Marketo REST-API konsistente Einblicke in diese Aktivitäten zu erhalten.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **API-Fehlerbehebung für Programmteilnehmer abrufen**: Vor Kurzem wurde eine Änderung vorgenommen, um das Verhalten des Endpunkts [Programmmitglieder abrufen](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} zu korrigieren. Bei der Verwendung des Filtertyps `updatedAt` zur Angabe eines Datumsbereichs bestand die Möglichkeit, dass in der Antwort keine in diesem Bereich aktualisierten Einträge für Programmmitgliedschaften enthalten waren. Darüber hinaus bestand die Möglichkeit, dass außerhalb des angegebenen Datumsbereichs aktualisierte Programmmitgliedschaftsdatensätze fälschlicherweise in die Antwort aufgenommen wurden. Beide Probleme wurden behoben.

* **Einstellung des Kontoinsight-Browser-Plug-ins**: Adobe entfernt am 8. April 2024 das Browser-Plugin für Kontoverwaltung [Kontoeinblick](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} aus dem Chrome-Webspeicher. Vorhandene Benutzer: Sie können das Plug-in weiter verwenden, bis Sie Ihre Marketo Engage-Instanz zu Adobe Identity und Admin Console migrieren. Diese Änderung **wirkt sich nicht auf** andere TAM-Funktionen/Daten innerhalb von Marketo Engage oder die E-Mail-Plug-ins Chrome und Outlook aus, die mit Sales Insight funktionieren. [Weitere Infos](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
