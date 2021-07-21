---
unique-page-id: 42762514
description: Insights-Dashboard Funktionsübersicht - Marketo-Dokumente - Produktdokumentation
title: Übersicht über die Funktionen des Insights-Dashboards
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
source-git-commit: 6679e1e0bdb53d3f330c15415a5fbe38f61d28d2
workflow-type: tm+mt
source-wordcount: '1460'
ht-degree: 0%

---

# Übersicht über die Funktionen des Insights-Dashboards {#insights-dashboard-feature-overview}

Erfahren Sie mehr über die Funktionen, die in Ihrem Sales Insights-Dashboard verfügbar sind.

>[!PREREQUISITES]
>
>Sie müssen über das neueste MSI SFDC-Paket und [configuration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md) verfügen.

![](assets/one.png)

## Kontaktlayout {#contact-layout}

**Interaktions-Velocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten der letzten 90 Tage
* Der Benutzer kann die Aktivität &quot;Konto anzeigen&quot;auswählen. Dadurch werden alle auf Kontoebene interessanten Momente, E-Mail und Web-Aktivität in der Kontaktansicht eingebettet.
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt

**Interaktionsanalyse und Zusammenfassung**

* Drilldown von Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse**

Registerkarte &quot;E-Mail-Kampagnen&quot;:

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller in der Marketo-Instanz geplanten E-Mail-Kampagnen). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

![](assets/three.png)

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme, die für die nächsten 90 Tage geplant sind
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

![](assets/two.png)

## Lead-Layout {#lead-layout}

**Interaktions-Velocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten der letzten 90 Tage
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt
* Die Funktion &quot;Kontoaktivität anzeigen&quot;ist nicht für Leads verfügbar, da sie in Salesforce erst dann Teil eines Kontos ist, wenn sie in einen Kontakt konvertiert wird

**Interaktionsanalyse und Zusammenfassung**

* Drilldown-Aktivitätskarten für interessante Momente, E-Mail und Web-Aktivität
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse:**

Registerkarte &quot;E-Mail-Kampagnen&quot;:

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller in der Marketo-Instanz geplanten E-Mail-Kampagnen). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

![](assets/five.png)

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme, die für die nächsten 90 Tage geplant sind
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

![](assets/four.png)

## Kontolayout {#account-layout}

**Interaktions-Velocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten in den letzten 90 Tagen für alle Kontakte in dem Konto
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt

**Interaktions-Drilldown und -Zusammenfassung**

* Drilldown-Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität, einschließlich Kontaktname
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse**

Registerkarte &quot;E-Mail-Kampagnen&quot;:

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller in der Marketo-Instanz geplanten E-Mail-Kampagnen). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme, die für die nächsten 90 Tage geplant sind
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

## Opportunity Layout {#opportunity-layout}

**Interaktions-Velocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten in den letzten 90 Tagen für alle Kontakte in der Gelegenheit
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt

**Interaktions-Drilldown und -Zusammenfassung**

* Drilldown-Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität, einschließlich Kontaktname
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und** EreignisseRegisterkarte E-Mail-Kampagnen :

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller in der Marketo-Instanz geplanten E-Mail-Kampagnen). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme, die für die nächsten 90 Tage geplant sind
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;
