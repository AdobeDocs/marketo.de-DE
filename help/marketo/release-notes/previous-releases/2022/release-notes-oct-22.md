---
description: Versionshinweise - Oktober 2022 - Marketo-Dokumente - Produktdokumentation
title: Oktober 2022 - Versionshinweise
source-git-commit: 39eb451117a5f165ceccc0435db77aa22f1bfdcd
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 5%

---

# Versionshinweise: Oktober 2022 {#release-notes-oct-22}

Unten finden Sie alle Funktionen der Version vom 22. Oktober. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den Standard-Versionszyklus und werden ab der Veröffentlichung auf **14. Oktober 2022**, mit einer stufenweisen Einführung der verbleibenden Funktionen in den darauffolgenden Wochen. Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte prüfen Sie unten jedes Feature nach seinem Status.

### Marketing-Datenumgebung {#marketing-data-environment}

</br>

* **Benutzerdefinierte Feldsynchronisierung für Programmteilnehmer**: Möglichkeit der bidirektionalen Synchronisierung erweiterbarer Felder, die für ein Programmmitglied erfasst werden (z. B. Teilnehmerpräferenzen während der Ereignisregistrierung, wie Essen, Sitzungen, Tracks usw.)

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Benutzerdefinierte Feldsynchronisierung für Programmteilnehmer</a></td>
  </tr>
  </tbody>
</table>

* **Integration von Adobe Privacy Service**: Harmonisierung mit Privacy Service zur Automatisierung der Einhaltung von Datenschutzbestimmungen für Experience Cloud-Produkte. Derzeit ist dieser Dienst nur für Marketo Engage-Kunden verfügbar, die mit dem Adobe Identity Management System integriert sind.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Erlebnis der nächsten Generation {#modern-ux}

</br>

* **Aktualisierte Screens im Erlebnis der nächsten Generation**: Wir stellen zusätzliche, aktualisierte Bildschirme der nächsten Generation bereit, die aktualisierte Design- und Benutzerfreundlichkeitsverbesserungen bieten, auf die über einen Umschalter zugegriffen werden kann:

   * Details zur Landingpage-Vorlage
   * E-Mail-Vorlagenliste

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Umschalten</a></td>
  </tr>
  </tbody>
</table>

* **Verbesserte Verwendung nach Registerkarte in Details von E-Mail-Vorlagen**: Im neuen Erlebnis sehen Sie zusätzliche Informationen zu Assets, die die E-Mail-Vorlage verwenden, einschließlich Asset-Status, Last Modified und Last Modified By. Sie können auch die Liste der von Assets verwendeten suchen, sortieren und filtern.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

* **Report Asset-Filtermodelle**: Neues Design für Berichtskonfigurationsmodelle, das eine neue Asset-Struktur im Konfigurationsmenü und einen Filter für das Erstellungsdatum und das Änderungsdatum anzeigt.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

### API-Verbesserungen {#api-enhancements}

</br>

* **Massenimport von Blei: SalesPersonenverein**: Parität mit der Lead-REST-API, um Leads während des Massenimport-Prozesses mit SalesPERS zu verknüpfen, wodurch die Komplexität und die Anzahl der erforderlichen API-Aufrufe verringert werden.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="https://developers.marketo.com/rest-api/bulk-import/bulk-lead-import/">Import von Bulk Lead</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight {#sales-insight}

</br>

![(Stern)](assets/yellow-star.png)

* **Integration von Sales Insight mit Dynamic Chat**: Das Insights-Dashboard enthält jetzt Aktivitäten des dynamischen Cats im Smart-Raster sowie eine wöchentliche Zusammenfassung und Detailkarten.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Dynamic Chat-Integration</a></td>
  </tr>
  </tbody>
</table>

## Agile Release-Funktionen

Die folgenden Funktionen entsprechen einem Agile-Format und werden an verschiedenen Daten vor oder nach dem standardmäßigen Veröffentlichungsdatum veröffentlicht. Bitte prüfen Sie unten jedes Feature nach seinem Status.

* **Dialogfeld-Streams für dynamischen Chat automatisch anordnen**: Verbessern Sie Ihre überfüllte Dialog-Arbeitsfläche, indem Sie alles auf der Arbeitsfläche in einem sauberen und leicht lesbaren Format organisieren, indem Sie die Taste drücken, indem Sie Auto Arrange auswählen.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md#stream-designer-icons">Stream-Designer-Symbole</a></td>
  </tr>
  </tbody>
</table>

* **Meeting-Links für dynamischen Chat**: Option zur automatischen Einbindung eines Teams- oder Meet-Links für Google und Outlook in jede Kalendereinladung, die an Besucher gesendet wird.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md">Kalender</a></td>
  </tr>
  </tbody>
</table>

* **Unterstützung zusätzlicher Datentypen für dynamischen Chat**: Drei neue Datentypen (boolesch, Ganzzahl, Gleitkommazahl) ermöglichen es Ihnen, vorhandene Marketo Engage-Felder im dynamischen Chat für Dinge wie das Targeting auf Grundlage von Bewertungen oder die Frage, ob Besucher Ja/Nein-Fragen haben, besser zu nutzen.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td><i>Demnächst verfügbar</i></td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

* **Terminierte Meetingbenachrichtigungen für dynamischen Chat**: Vertriebsmitarbeiter erhalten automatisierte E-Mail-Benachrichtigungen zu geplanten Sitzungen sowie relevante Informationen zur Chatbot-Interaktion des Besuchers.

<table> 
  <tr> 
   <td><b>Status</b></td>
   <td><b>Aktualisierungen der Dokumentation</b></td>
  </tr>
  <tr> 
   <td><i>Demnächst verfügbar</i></td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>

## Ankündigungen {#announcements}

* **Forms 1.0**: Die Einstellung von Forms 1.0 wird mit der Oktober-Version abgeschlossen. Forms 1.0-Assets können keine Daten mehr an Marketo Engage senden und geben bei Versuchen Fehler zurück.

* **NoScript Forms**: Forms funktioniert nicht mehr, wenn JavaScript im Browser deaktiviert ist. Für die Übermittlung von Formularen muss JavaScript aktiviert sein.