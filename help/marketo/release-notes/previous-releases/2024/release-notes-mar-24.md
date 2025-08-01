---
description: März 2024 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – März 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 4%

---

# März 2024 - Versionshinweise {#release-notes-mar-24}

Nachstehend finden Sie alle Funktionen, die in der Version vom 24. März enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **. März 2024 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise eingeführt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Erweiterte Konversationsflusslogik</strong>: Fügen Sie zusätzliche Felder zur Auswertung in einer einzigen Auswahl für die Konversationsflussverfolgung hinzu.</td>
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Gesprächsflusseinstellungen für Marketo Engage Forms</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Konversationsflusslogik neu anordnen</strong>: In Marketo Engage Forms können Sie jetzt die Optionen für den Konversationsfluss neu anordnen, anstatt ihn löschen und wieder hinzufügen zu müssen.</td>
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Gesprächsflusseinstellungen für Marketo Engage Forms</a></td>
   </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>API-Aktivitätsmetadaten</strong>:
   Metadaten wie Benutzeragent, Plattform und Gerät sind jetzt in Web- und E-Mail-Aktivitäten enthalten, was über die Marketo-REST-API zu konsistenten Einblicken in diese Aktivitäten beiträgt.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
 </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Fehlerbehebung für die Programmteilnehmer-API**: Kürzlich wurde eine Änderung vorgenommen, um das Verhalten des Endpunkts [Programmmitglieder abrufen](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} zu korrigieren. Zuvor bestand bei Verwendung des `updatedAt` Filtertyps zum Angeben eines Datumsbereichs die Möglichkeit, dass in diesem Bereich aktualisierte Programmmitgliedschaftsdatensätze nicht in der Antwort enthalten waren. Darüber hinaus bestand die Möglichkeit, dass Programmmitgliedschaftsdatensätze, die außerhalb des angegebenen Datumsbereichs aktualisiert wurden, fälschlicherweise in die Antwort aufgenommen wurden. Beide Probleme wurden behoben.

* **Einstellung des Account Insight Browser-Plug**: Adobe entfernt das Target Account Management [Account Insight Browser-Plug-in](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} am 8. April 2024 aus dem Chrome Web Store. Vorhandene Benutzende: Sie können das Plug-in weiterhin verwenden, bis Sie Ihre Marketo Engage-Instanz zu Adobe Identity und Admin Console migrieren. Diese Änderung **sich nicht** andere TAM-Funktionen/Daten in Marketo Engage oder die Chrome- und Outlook-E-Mail-Plug-ins aus, die mit Sales Insight funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
