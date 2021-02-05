---
unique-page-id: 42762409
description: Sales Insight-Seite für Marketing-Administratoren - Marketing-Dokumente - Produktdokumentation
title: Sales Insight-Seite für Marketing-Administratoren
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# Sales Insight-Seite für Marketing-Administratoren {#sales-insight-page-for-marketo-admins}

Marketo Admins verfügen über bestimmte Rechte in Sales Insight. Erfahren Sie, was sie unten sind.

## Soap-API-Konfiguration {#soap-api-configuration}

Diese Anmeldeinformationen werden verwendet, um Ihr Salesforce-Konto mit Ihrer Marketo-Instanz zu verbinden, um MSI in Salesforce zu verwenden.

![](assets/one-1.png)

## Rest-API-Konfiguration {#rest-api-configuration}

Diese Anmeldeinformationen werden verwendet, um Ihr Salesforce-Konto mit Ihrer Marketo-Instanz zu verbinden, um MSI Insights-Dashboard in Salesforce zu verwenden.

![](assets/two-1.png)

Sie können die Rest-API-Anmeldeinformationen in SFDC entfernen und nur SOAP-APIs verwenden. Dadurch wird das Insight-Dashboard deaktiviert.

![](assets/three-1.png)

## Personenbewertungseinstellungen {#person-score-settings}

| **Sterne:** | Sterne stellen den Gesamt-Interessentenwert im Vergleich zu anderen Interessenten dar. |
|---|---|
| **Flammen:** | Flammen stellen Dringlichkeit dar - wie stark sich das Ergebnis eines Interessenten in letzter Zeit verändert hat. |

Standardmäßig verwendet Marketo Sales Insight das Feld Interessentenbewertung, um Sterne und Flammen zu berechnen. Aber wenn Sie ein anderes Feld auswählen möchten, hier:

1. Klicken Sie im Bereich **Admin** von Marketo auf **Sales Insight**.

   ![](assets/four.png)

1. Klicken Sie unter Interessentenbewertungseinstellungen auf **Bearbeiten**.

   ![](assets/five.png)

1. Wählen Sie das Feld aus, das Sie für Sterne verwenden möchten.

   ![](assets/six.png)

1. Wählen Sie das Feld aus, das Sie für Flammen verwenden möchten.

   ![](assets/seven.png)

1. Klicken Sie auf **Speichern**. Die Neuberechnung von Sales Insight dauert einige Zeit. Sie können Ihr CRM später überprüfen, um die Sterne und Flammen zu sehen.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Wenn Sie noch keine benutzerdefinierten Ergebnisfelder haben, können Sie diese hier [erstellen.](http://docs.marketo.com/x/3wMk)

   >[!MORELIKETHIS]
   >
   >
   >
   >[Sterne und Flammen](http://docs.marketo.com/x/qgU6Ag)

## Einstellungen {#settings}

![](assets/nine.png)

**Abmelden-Einstellungen: **

Sie können die folgenden Abmeldeeinstellungen für &quot;Keine Vorlage&quot;, &quot;Standard-E-Mails und operative E-Mails auswählen

* Einstellung zum Abmelden respektieren
* Einstellungen für das Abmelden bei mehr als 1 Empfänger respektieren
* Einstellungen für das Abmelden bei mehr als 5 Empfängern respektieren
* Einstellungen für das Abmelden ignorieren

**Möglichkeit zum Sperren von Vorlagen aktivieren: **

Wenn diese Option aktiviert ist, können MSI-Benutzer beim Senden von E-Mails aus Salesforce keine Vorlagen bearbeiten

**RSS-Feed aktivieren:**

Wenn diese Option aktiviert ist, können MSI-Benutzer ihren Interessenten-Feed in einem RSS-Feed (zusätzlich zum Interessenten-Feed in Salesforce)**.** Ansicht haben.
