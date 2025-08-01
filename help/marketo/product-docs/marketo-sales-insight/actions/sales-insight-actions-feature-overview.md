---
description: Übersicht über die Funktionen von Sales Insight-Aktionen - Marketo-Dokumente - Produktdokumentation
title: Übersicht über die Aktionsfunktionen in Sales Insight
exl-id: 059de248-d1a2-42cd-a7ec-f10b15d0b526
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1361'
ht-degree: 0%

---

# Übersicht über die Aktionsfunktionen in Sales Insight {#msi-actions-feature-overview}

Beschleunigen Sie die Akquise mit Marketing-gestützten Intelligence- und Interaktions-Tools in einem einzigen Workflow mithilfe von Sales Insight-Aktionen.

>[!NOTE]
>
>Marketo Sales Insight Actions ist ein Web-basiertes Programm, das über das [Marketo Sales Insight Package&rbrace; ausschließlich mit dem Salesforce CRM integriert ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Dies wird manchmal als &quot;Marketo-Vertrieb“ oder einfach als „Aktionen“ bezeichnet.

Eine Videoübersicht der Sales Insight-Aktionen finden Sie [hier](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/sales-insight-actions/overview.html?lang=de){target="_blank"}.

![](assets/sales-insight-actions-feature-overview-1.png)

## Lead-Layout und Kontakt-Layout {#lead-layout-and-contact-layout}

Die folgenden Aktionen sind im Dropdown-Menü „Aktionen auswählen“ im oberen Navigationsbereich verfügbar:

* Verkaufs-E-Mail senden
   * Verkaufs-E-Mails verfügen über Ansicht-, Klick- und Antwort-Tracking (wenn der Versandkanal eingerichtet ist)
   * Enthält E-Mail-Personalization, benutzerdefinierte Signatur und Anhänge
   * Vorlagenfreigabe und Berichte
   * Team-Freigabe, Gruppen-E-Mails und CC/BCC-Funktion
   * Die E-Mail-Aktivität für den Verkauf wird im Personendatensatz von Marketo protokolliert.
   * Entsprechende Filter und Trigger in Marketo Smart Campaign (Details unten)

* Zur Verkaufskampagne hinzufügen
   * Leads zu Verkaufs-Playbooks hinzufügen, das aus einer Abfolge von E-Mails und Aufgaben besteht
   * Umfasst Zugriff und Freigabe durch das Team, Aufgabenerstellung, Überspringen von Wochenenden, Ignorieren von OOO-E-Mails als Antworten und automatisches Ende
   * Die Kampagnenaktivität wird im Marketo-Personendatensatz protokolliert.
   * Entsprechende Filter und Trigger in Marketo Smart Campaign (Details unten)

* Verkaufsgespräch
   * Verkaufsanrufe mit dem Dialer im CRM tätigen
   * Einschließlich lokaler Präsenz, voraufgezeichnet
   * Aufrufergebnis, Aufrufaufzeichnung im Bedienfeld und Aktivitätsverlauf protokollieren
   * Die Aufruffaktivität wird im Marketo-Personendatensatz protokolliert.
   * Filter und Trigger in Marketo Smart Campaign

* Aufgabe hinzufügen
   * E-Mail, Anruf, InMail und benutzerdefinierte Aufgaben für Ihre Leads erstellen
   * Automatisieren der Aufgabenerstellung mit Verkaufskampagnen
   * Aufgaben mit [!DNL Salesforce] synchronisieren
   * Aufgaben [!DNL Salesforce] Abschnitt Aktivitätsverlauf protokollieren

Sie können auf den Live-Feed zugreifen, indem Sie auf das Symbol (0) in der oberen Navigationsleiste klicken. Dazu gehört die Möglichkeit, Live-Updates zu Vertriebsaktivitäten zusammen mit der Bildschirm-Dockingfunktion anzuzeigen.

![](assets/sales-insight-actions-feature-overview-2.png)

Die folgenden Daten sind auf den Registerkarten im MSI-Bedienfeld verfügbar:

* Insights-Dashboard
   * Das Interaktionsgeschwindigkeits-Raster enthält Aktivitäten aus Verkaufs-E-Mails, Verkaufskampagnen-Aktionen und Verkaufsanrufen
   * Anstehende Verkaufskampagnen : Wenn ein Lead Teil einer laufenden Kampagne ist, sind diese Informationen auf der Registerkarte Anstehende Verkaufskampagnen verfügbar
   * Anstehende Aufgaben - Wenn eine anstehende Aufgabe in Bezug auf einen Lead vorhanden ist, sind diese Informationen auf der Registerkarte Anstehende Aufgaben verfügbar.

* Registerkarte „E-Mail“
   * Alle gesendeten Verkaufs-E-Mails werden hier protokolliert. Die Aktivitäten werden auch im Marketo-Personendatensatz protokolliert.
   * Die Spalten umfassen Betreff, Öffnen, Klicken, Antworten (nur für Verkaufs-E-Mails mit eingerichtetem Versandkanal verfügbar), Absender, Datum
   * Enthält eine ausziehbare Karte mit zusätzlichen Details wie Absender, Vorlage, Verkaufskampagne und Vorschau der E-Mail

* Registerkarte „Aufruf“
   * Hier werden alle Anrufe protokolliert, die über die Sales Dialer-Funktion getätigt werden. Die Aktivitäten werden auch im Marketo-Personendatensatz protokolliert.
   * Zu den Spalten gehören Name, Ergebnis, Notizen, Aufgerufenes Datum, Dauer und Link zur Aufzeichnung
   * Enthält eine Erweiterungskarte mit zusätzlichen Details wie „Anruf von“, „Angenommen von“, „Telefonnummer“ und „Status“

## Konto- und Opportunity-Layout {#account-and-opportunity-layout}

Die folgenden Aktionen sind in der oberen Navigationsleiste verfügbar:

* Verkaufs-E-Mail senden - Möglichkeit, personalisierte oder vorlagenbasierte Gruppen-E-Mails mit Ansicht-, Klick- und Antwort-Tracking an alle Kontakte zu senden, die mit einem Konto/einer Opportunity verbunden sind
   * Verkaufs-E-Mails verfügen über Ansicht-, Klick- und Antwort-Tracking (wenn der Versandkanal eingerichtet ist)
   * Enthält E-Mail-Personalization, benutzerdefinierte Signatur und Anhänge
   * Vorlagenfreigabe und Berichte
   * Team-Freigabe, Gruppen-E-Mails und CC/BCC-Funktion
   * Die E-Mail-Aktivität für den Verkauf wird im Personendatensatz von Marketo protokolliert.
   * Entsprechende Filter und Trigger in Marketo Smart Campaign (Details unten)

* Zu Vertriebskampagne hinzufügen - Alle Kontakte, die mit einem Konto/einer Opportunity verbunden sind, werden zu Vertriebs-Playbooks hinzugefügt, d. h. zu einer Abfolge von E-Mails und Aufgaben
   * Leads zu Verkaufs-Playbooks hinzufügen, das aus einer Abfolge von E-Mails und Aufgaben besteht
   * Umfasst Zugriff und Freigabe durch das Team, Aufgabenerstellung, Überspringen von Wochenenden, Ignorieren von OOO-E-Mails als Antworten und automatisches Ende
   * Die Kampagnenaktivität wird im Marketo-Personendatensatz protokolliert.
   * Entsprechende Filter und Trigger in Marketo Smart Campaign (Details unten)

Sie können auf den Live-Feed zugreifen, indem Sie auf das Symbol (0) in der oberen Navigationsleiste klicken. Dazu gehört die Möglichkeit, Live-Updates zu Vertriebsaktivitäten zusammen mit der Bildschirm-Dockingfunktion anzuzeigen.

Folgende Daten sind auf den Registerkarten verfügbar:

* Insights-Dashboard
   * Das Interaktionsgeschwindigkeits-Raster enthält Aktivitäten aus Sales-E-Mails, Sales-Kampagnenaktionen und dem Sales-Call
   * Anstehende Verkaufskampagnen : Wenn ein Kontakt aus dem Konto/der Opportunity Teil einer laufenden Kampagne ist, sind diese Informationen auf der Registerkarte Anstehende Verkaufskampagnen verfügbar
   * Anstehende Aufgaben - Wenn eine anstehende Aufgabe mit einem Kontakt aus dem Konto/der Opportunity verknüpft ist, sind diese Informationen auf der Registerkarte Anstehende Aufgaben verfügbar.

* Registerkarte „E-Mail“
   * Alle Verkaufs-E-Mails, die von dem Konto/der Opportunity an Kontakte gesendet werden, werden hier protokolliert. Die Aktivitäten werden auch im Marketo-Personendatensatz protokolliert.
   * Die Spalten umfassen Betreff, Öffnen, Klicken, Antworten (nur für Verkaufs-E-Mails mit eingerichtetem Versandkanal verfügbar), Absender und Datum
   * Enthält eine ausziehbare Karte mit zusätzlichen Details wie Absender, Vorlage, Verkaufskampagne und Vorschau der E-Mail

* Registerkarte „Aufruf“
   * Hier werden alle Aufrufe an Kontakte aus dem Konto/der Opportunity, die die Funktion „Vertriebs-Dialer“ verwenden, protokolliert. Die Aktivitäten werden auch im Marketo-Personendatensatz protokolliert.
   * Zu den Spalten gehören Name, Ergebnis, Notizen, Abrufzeit, Dauer und Link zur Aufzeichnung
   * Enthält eine Erweiterungskarte mit zusätzlichen Details wie „Anruf von“, „Angenommen von“, „Telefonnummer“ und „Status“

## Lead- und Kontaktlistenansicht (Massenaktionen) {#lead-and-contact-list-view}

* [!UICONTROL Verkaufs-E-Mail senden] - Möglichkeit, personalisierte oder vorlagenbasierte E-Mails mit Ansicht-, Klick- und Antwort-Tracking an eine Liste von Kontakten/Leads zu senden
* [!UICONTROL Zu Vertriebskampagne hinzufügen] - Zu Verkaufs-Playbooks hinzufügen, das eine Abfolge von E-Mails und Aufgaben zu einer Liste von Kontakten/Leads ist

## Registerkarte &quot;Marketo Global“ {#marketo-global-tab}

**[!UICONTROL Best Bets]-Registerkarte**

![](assets/sales-insight-actions-feature-overview-3.png)

Die folgenden Massenaktionen sind aus der Dropdown-Liste auf der Registerkarte [!UICONTROL Best Bets] verfügbar:

* [!UICONTROL Verkaufs-E-Mail senden] - Möglichkeit zum Senden personalisierter oder vorlagenbasierter E-Mails mit Ansicht-, Klick- und Antwort-Tracking
* [!UICONTROL Zu Vertriebskampagne hinzufügen] - Hinzufügen von Leads zu Verkaufs-Playbooks, d. h. einer Sequenz von E-Mails und Aufgaben

  ![](assets/sales-insight-actions-feature-overview-4.png)

Die folgenden Inline-Aktionen sind für einzelne Leads/Kontakte auf der Registerkarte [!UICONTROL Best Bets] verfügbar:

* [!UICONTROL Verkaufs-E-Mail senden] - Möglichkeit zum Senden personalisierter oder vorlagenbasierter E-Mails mit Ansicht-, Klick- und Antwort-Tracking
* [!UICONTROL Zu Vertriebskampagne hinzufügen] - Hinzufügen von Leads zu Verkaufs-Playbooks, d. h. einer Sequenz von E-Mails und Aufgaben
* [!UICONTROL Verkaufsanruf] - Führen Sie Verkaufsanrufe mit dem Dialer im CRM durch
* [!UICONTROL Aufgabe hinzufügen] - E-Mail-, Anruf-, Kunden- oder LinkedIn-Aufgaben für potenzielle Leads erstellen

  ![](assets/sales-insight-actions-feature-overview-5.png)

**Registerkarte „E-Mail“**

* Alle gesendeten Verkaufs-E-Mails werden hier protokolliert. Die Aktivitäten werden auch im Marketo-Personendatensatz protokolliert.
* Die Spalten umfassen Betreff, Öffnen, Klicken, Antworten (nur für Verkaufs-E-Mails mit eingerichtetem Versandkanal verfügbar), Absender und Datum
* Enthält eine ausziehbare Karte mit zusätzlichen Details wie Absender, Vorlage, Verkaufskampagne und Vorschau der E-Mail

**Registerkarte „Aufruf“**

* Hier werden alle Anrufe protokolliert, die über die Sales Dialer-Funktion getätigt werden. Die Aktivitäten werden auch im Marketo-Personendatensatz protokolliert.
* Zu den Spalten gehören Name, Ergebnis, Notizen, Abrufzeit, Dauer und Link zur Aufzeichnung
* Enthält eine Erweiterungskarte mit zusätzlichen Details wie „Anruf von“, „Angenommen von“, „Telefonnummer“ und „Status“

**Registerkarte „Aufgabe“**

* Erstellte und abgeschlossene E-Mail-, Anruf-, InMail- und benutzerdefinierte Aufgaben stehen auf dieser Registerkarte für die Aufgabenverwaltung zur Verfügung. Umfasst die Möglichkeit, Aufgaben hinzuzufügen
* Automatisieren der Aufgabenerstellung mit Verkaufskampagnen
* Aufgaben mit [!DNL Salesforce] synchronisieren
* Aufgaben [!DNL Salesforce] Abschnitt Aktivitätsverlauf protokollieren

  ![](assets/sales-insight-actions-feature-overview-6.png)

**Live-Feed**

* Möglichkeit, Live-Updates zu Vertriebsaktivitäten zusammen mit der Bildschirm-Dockingfunktion anzuzeigen
* Eingebettete E-Mail-, Anruf- und Kadenz-Schaltflächen machen jeden Kunden-insight umsetzbar

## In Marketo verfügbare Funktionen {#features-available-in-marketo}

Vertriebsaktivitäten, die in Marketo erfasst werden:

* Verkaufs-E-Mail senden - Benutzer hat eine Verkaufs-E-Mail an einen Lead gesendet
* Verkaufs-E-Mail öffnen - Lead hat eine gesendete Verkaufs-E-Mail geöffnet
* Auf Verkaufs-E-Mail klicken - Lead hat auf einen Link in einer Verkaufs-E-Mail geklickt
* E-Mail zum Verkauf beantwortet - Lead hat auf E-Mail zum Verkauf geantwortet
* Verkaufsanruf empfangen - Der Lead hat einen Anruf von einem Vertriebsmitarbeiter mithilfe des Verkaufsanrufs erhalten.
* Zur Verkaufskampagne hinzufügen - Lead wurde zu einer erstellten Verkaufskampagne hinzugefügt
* Aus Vertriebskampagne entfernt - Lead wurde aus einer erstellten Vertriebskampagne entfernt

Zu den Filtern und Triggern gehören:

* [!UICONTROL Wird per Verkaufs-E-Mail gesendet]
* [!UICONTROL Öffnet Verkaufs-E-Mail]
* [!UICONTROL Klicks auf Verkaufs-E-]
* [!UICONTROL Antworten auf Verkaufs-E-Mails]
* [!UICONTROL Erhält einen Verkaufsanruf]
* [!UICONTROL Zu Vertriebskampagne hinzugefügt]
* [!UICONTROL Aus Vertriebskampagne entfernt]

  ![](assets/sales-insight-actions-feature-overview-7.png)
