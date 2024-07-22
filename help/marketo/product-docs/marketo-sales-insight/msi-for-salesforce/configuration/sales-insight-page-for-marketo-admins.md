---
unique-page-id: 42762409
description: Sales Insight-Seite für Marketo-Administratoren - Marketo-Dokumente - Produktdokumentation
title: Sales Insight-Seite für Marketo-Administratoren
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 1%

---

# Sales Insight-Seite für Marketo-Administratoren {#sales-insight-page-for-marketo-admins}

Marketo-Administratoren verfügen über bestimmte Berechtigungen in Sales Insight. Erfahren Sie, was sie unten sind.

## Soap-API-Konfiguration {#soap-api-configuration}

Diese Anmeldedaten werden verwendet, um Ihr Salesforce-Konto mit Ihrer Marketo-Instanz zu verbinden und MSI in Salesforce zu verwenden.

![](assets/one-1.png)

## Rest-API-Konfiguration {#rest-api-configuration}

Mit diesen Anmeldedaten wird Ihr Salesforce-Konto mit Ihrer Marketo-Instanz verbunden, um das MSI Insights-Dashboard in Salesforce zu verwenden.

![](assets/two-1.png)

## Personenbewertungseinstellungen {#person-score-settings}

* **Sterne**: Sterne stellen den Gesamt-Lead-Punktstand im Vergleich zu anderen Leads dar.
* **Flammen**: Flammen stellen die Dringlichkeit dar - wie stark sich das Ergebnis eines Leads in letzter Zeit geändert hat.

Standardmäßig verwendet Marketo Sales Insight das Feld Lead-Score , um Sterne und Flammen zu berechnen. Wenn Sie jedoch ein anderes Feld auswählen möchten, sehen Sie wie:

1. Klicken Sie im Bereich **Admin** von Marketo auf **Sales Insight**.

   ![](assets/four.png)

1. Klicken Sie unter &quot;Lead-Scoring-Einstellungen&quot;auf **Bearbeiten**.

   ![](assets/five.png)

1. Wählen Sie das Feld aus, das Sie für Sterne verwenden möchten.

   ![](assets/six.png)

1. Wählen Sie das Feld aus, das Sie für Flammen verwenden möchten.

   ![](assets/seven.png)

1. Klicken Sie auf **Speichern**. Die Neuberechnung von Sales Insight dauert einige Zeit. Sie können Ihr CRM später überprüfen, um die Sterne und Flammen zu sehen.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Wenn Sie noch nicht über benutzerdefinierte Punktfelder verfügen, können Sie wie [diese erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Sterne und Flammen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Einstellungen {#settings}

![](assets/nine.png)

**Abmeldeeinstellungen:**

Sie können die folgenden Abmeldeeinstellungen für &quot;Keine Vorlage&quot;, &quot;Standard-E-Mails und operative E-Mails&quot;auswählen

* Einstellung zum Abmelden respektieren
* Respektieren Sie die Abmeldeeinstellungen, wenn mehr als ein Empfänger
* Respektieren Sie die Abmeldeeinstellungen, wenn mehr als fünf Empfänger
* Abbestelleinstellungen ignorieren

**Aktivieren der Möglichkeit, Vorlagen zu sperren:**

Wenn diese Option aktiviert ist, können MSI-Benutzer beim Senden von E-Mails aus Salesforce keine Vorlagen bearbeiten

**RSS-Feed aktivieren:**

Wenn diese Option aktiviert ist, können MSI-Benutzer ihren Lead-Feed in einem RSS-Feed anzeigen (zusätzlich zum Lead-Feed in Salesforce ). RSS-Feeds können nur funktionieren, wenn die Funktion &quot;Token-Ablauf&quot;deaktiviert ist.

**Token-Ablauf:**

Der Token-Ablauf wird im Feature Manager gesteuert. Wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support), um ihn zu aktivieren/deaktivieren. Wenn diese Option aktiviert ist, laufen alle Marketo-Token innerhalb von 10 Minuten ab. Wenn diese Option deaktiviert ist, laufen Marketo-Token nicht ab.

Token, die vor der Aktivierung des Token-Ablaufs generiert wurden, haben keine Ablaufzeit, um sie zu validieren. Daher laufen sie auch dann nicht ab, wenn die Funktion derzeit aktiviert ist.

Token, die nach der Aktivierung des Token-Ablaufs generiert wurden, haben eine Ablaufzeit von 10 Minuten, sodass sie auch nach der Deaktivierung der Funktion noch in 10 Minuten ablaufen.

Das Token-Verhalten basiert auf dem Zeitpunkt der Erstellung (wenn die Token-Ablauffunktion aktiviert/deaktiviert wurde, anstatt auf dem aktuellen Funktionsstatus).
