---
unique-page-id: 42762409
description: Sales Insight-Seite für Marketing-Administratoren - Marketing-Dokumente - Produktdokumentation
title: Sales Insight-Seite für Marketing-Administratoren
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '438'
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

* **Sterne**: Sterne stellen den Gesamt-Interessentenwert im Vergleich zu anderen Interessenten dar.
* **Flammen**: Flammen stellen Dringlichkeit dar - wie stark sich das Ergebnis eines Interessenten in letzter Zeit verändert hat.

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
   >Wenn Sie noch keine benutzerdefinierten Ergebnisfelder haben, können Sie diese hier [erstellen.](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

   >[!MORELIKETHIS]
   >
   >[Sterne und Flammen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Einstellungen {#settings}

![](assets/nine.png)

**Abmeldeeinstellungen:**

Sie können die folgenden Abmeldeeinstellungen für &quot;Keine Vorlage&quot;, &quot;Standard-E-Mails und operative E-Mails auswählen

* Einstellung zum Abmelden respektieren
* Einstellungen für das Abmelden bei mehr als 1 Empfänger respektieren
* Einstellungen für das Abmelden bei mehr als 5 Empfängern respektieren
* Einstellungen für das Abmelden ignorieren

**Möglichkeit zum Sperren von Vorlagen:**

Wenn diese Option aktiviert ist, können MSI-Benutzer beim Senden von E-Mails aus Salesforce keine Vorlagen bearbeiten

**RSS-Feed aktivieren:**

Wenn diese Option aktiviert ist, können MSI-Benutzer ihren Lead-Feed in einem RSS-Feed (zusätzlich zum Lead-Feed in Salesforce) Ansicht haben. RSS-Feeds können nur funktionieren, wenn die Funktion &quot;Token-Ablauf&quot;deaktiviert ist.

**Token-Ablauf:**

Der Token-Ablauf wird im Feature Manager gesteuert. Um sie zu aktivieren/deaktivieren, wenden Sie sich an [Marketing Support](https://nation.marketo.com/t5/Support/ct-p/Support). Wenn diese Option aktiviert ist, laufen alle Marketo-Token innerhalb von 10 Minuten ab. Wenn diese Option deaktiviert ist, laufen Marketo-Token nicht ab.

Token, die vor dem Aktivieren des Token-Ablaufs generiert wurden, haben keine Ablaufzeit für die Überprüfung, sodass sie auch dann nicht ablaufen, wenn die Funktion derzeit aktiviert ist.

Token, die nach der Aktivierung des Token-Ablaufs generiert wurden, haben eine Ablaufzeit von 10 Minuten. Daher laufen sie auch nach der Deaktivierung der Funktion in 10 Minuten immer noch ab.

Das Token-Verhalten basiert auf dem Zeitpunkt, zu dem es generiert wurde (bei Aktivierung/Deaktivierung der Token-Ablauffunktion anstelle des aktuellen Funktionsstatus).
