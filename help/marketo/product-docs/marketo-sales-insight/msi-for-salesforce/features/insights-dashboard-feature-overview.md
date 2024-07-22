---
unique-page-id: 42762514
description: Insights-Dashboard Funktionsübersicht - Marketo-Dokumente - Produktdokumentation
title: Übersicht über die Funktionen des Insight Dashboard
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 0%

---

# Übersicht über die Funktionen des Insight Dashboard {#insights-dashboard-feature-overview}

Erfahren Sie mehr über die Funktionen, die in Ihrem Sales Insights-Dashboard verfügbar sind.

>[!PREREQUISITES]
>
>Sie müssen über das neueste MSI SFDC-Paket und die [Konfiguration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md) verfügen.

![](assets/insights-dashboard-feature-overview-1.png)

## Kontaktlayout {#contact-layout}

**InteraktionsVelocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten der letzten 90 Tage
* Der Benutzer kann die Aktivität &quot;Konto anzeigen&quot;auswählen. Dadurch werden alle auf Kontoebene interessanten Momente, E-Mail und Web-Aktivität in der Kontaktansicht eingebettet.
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt

**Interaktionsdarstellung und Zusammenfassung**

* Drilldown von Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse**

Registerkarte &quot;E-Mail-Kampagnen&quot;:

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller E-Mail-Kampagnen, die in der Marketo-Instanz geplant sind). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

![](assets/insights-dashboard-feature-overview-2.png)

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme für die nächsten 90 Tage
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

![](assets/insights-dashboard-feature-overview-3.png)

## Lead-Layout {#lead-layout}

**InteraktionsVelocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten der letzten 90 Tage
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt
* Die Funktion &quot;Kontoaktivität anzeigen&quot;ist nicht für Leads verfügbar, da sie in Salesforce erst dann Teil eines Kontos ist, wenn sie in einen Kontakt konvertiert wird

**Interaktionsdarstellung und Zusammenfassung**

* Drilldown-Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse:**

Registerkarte &quot;E-Mail-Kampagnen&quot;:

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller E-Mail-Kampagnen, die in der Marketo-Instanz geplant sind). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

![](assets/insights-dashboard-feature-overview-4.png)

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme für die nächsten 90 Tage
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

![](assets/insights-dashboard-feature-overview-5.png)

## Kontolayout {#account-layout}

**InteraktionsVelocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten in den letzten 90 Tagen für alle Kontakte in dem Konto
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt

**Drilldown und Zusammenfassung der Interaktion**

* Drilldown-Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität, einschließlich Kontaktname
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse**

Registerkarte &quot;E-Mail-Kampagnen&quot;:

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller E-Mail-Kampagnen, die in der Marketo-Instanz geplant sind). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme für die nächsten 90 Tage
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

## Opportunity Layout {#opportunity-layout}

**InteraktionsVelocity-Raster**

* Dieses intelligente Raster enthält interessante Momente, E-Mail- und Web-Aktivitäten in den letzten 90 Tagen für alle Kontakte in der Gelegenheit
* Benutzer können bestimmte Wochen hervorheben, um Aktivitäten innerhalb dieser Woche anzuzeigen
* Standardansicht: Aktuelle Woche ist ausgewählt

**Drilldown und Zusammenfassung der Interaktion**

* Drilldown-Aktivitätskarten für interessante Momente, E-Mail- und Web-Aktivität, einschließlich Kontaktname
* Interessante Momente Aktivitätskarte - Enthält die Option Abonnieren
* E-Mail-Aktivitätskarte - einschließlich Vorschauoption
* Web-Aktivitätskarte - Bietet die Möglichkeit, auf einen Link zu klicken
* In der wöchentlichen Zusammenfassungsleiste werden interessante Momente, E-Mail- und Web-Aktivitäten für diese Woche angezeigt. Jedes Symbol kann angeklickt werden und als Filter verwendet werden, um bestimmte Aktivitäten anzuzeigen
* Standardansicht: Dies ist eine Liste der Aktivitäten der aktuellen Ansicht

**Bevorstehende E-Mail-Kampagnen und -Ereignisse** Registerkarte E-Mail-Kampagnen :

* Umfasst Kampagnen, die Teil von E-Mail-Programmen oder Standardprogrammen sind, die für die nächsten 90 Tage geplant sind
* Nicht spezifisch für Kontakt/Lead (d. h. die Kampagnenliste ist eine allgemeine Liste aller E-Mail-Kampagnen, die in der Marketo-Instanz geplant sind). Die Liste der Kampagnen in allen Lead-, Kontakt-, Konto- und Opportunity-Bereichen ist identisch.
* Wenn die Kampagnenwiederholung in den nächsten 90 Tagen mehr als dreimal ausgeführt wird, werden zu jedem beliebigen Zeitpunkt nur die nächsten drei Ausführungen angezeigt (ähnlich dem Verhalten in Marketo)
* Die Karte mit den Aktivitätsdetails in diesem Abschnitt enthält eine Vorschauoption. Wenn der Ablauf mehrere Schritte zum Senden von E-Mails umfasst, stehen alle E-Mails für die Vorschau zur Verfügung. Wenn im Schritt E-Mail-Ablauf des Versands mehrere &quot;E-Mail-Optionen&quot;vorhanden sind, ist die Standardoption für die Vorschau verfügbar
* Zu den Filtern gehören &quot;Suche&quot;und &quot;Datumsbereich&quot;.

Registerkarte Ereignis :

* Enthält Veranstaltungsprogramme für die nächsten 90 Tage
* Verwenden Sie die Filteroption, um alle Ereignisse/eingeladenen Ereignisse anzuzeigen (basierend auf den Admin-Einstellungen).
* Bei der Auswahl der eingeladenen Ereignisse werden Ereignisse, zu denen ein bestimmter Kontakt eingeladen wurde, zusammen mit dem Mitgliedsstatus angezeigt
* Bei Auswahl aller Ereignisse wird die Liste der Ereignisse angezeigt, die für die nächsten 90 Tage geplant sind
* Karte mit Aktivitätsdetails in diesem Abschnitt verfügt über eine Vorschauoption
* Filter enthält &quot;Suche&quot;, &quot;Nur eingeladene Ereignisse anzeigen&quot;und &quot;Datumsbereich&quot;

>[!NOTE]
>
>Wenn Ihr Konto oder Ihre Gelegenheit mehr als 800 Kontakte hat, werden im Dashboard keine Daten angezeigt. Sie können jedoch zu einzelnen Kontakten gehen, um deren Einblicke und Interaktion zu sehen. Wenn Ihr Konto mehr als 800 Kontakte hat, wird &quot;Aktivität auf Kontoebene anzeigen&quot;deaktiviert.
