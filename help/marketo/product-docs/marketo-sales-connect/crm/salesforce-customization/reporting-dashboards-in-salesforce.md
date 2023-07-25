---
unique-page-id: 14352464
description: Reporting-Dashboards in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Reporting-Dashboards in Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Reporting-Dashboards in Salesforce {#reporting-dashboards-in-salesforce}

Erfahren Sie unten, wie Sie Dashboards einrichten.

## Bericht öffnen und klicken {#open-and-click-report}

1. Wählen Sie die **Aufgaben und Ereignisse** Record Type.
1. Definieren Sie die Berichtsparameter basierend auf dem gewünschten Zeitraum und der gewünschten Hierarchie-Struktur.
1. Fügen Sie einen Filter hinzu, um in Salesforce protokollierte interne E-Mails zu entfernen (z. B. Unternehmen/Konto nicht gleich Marketo).
1. Wählen Sie die **Zusammenfassung** Berichtsformat.
1. Fügen Sie die Felder Betreff, Zugeordneter und Marketo Sales Clicked/Marketo Sales Viewed zum Bericht hinzu.
1. Doppelklicken Sie auf **Formel hinzufügen** im Bereich Felder .
1. Fügen Sie der Formel einen Namen hinzu, wählen Sie **Prozent** im Format und wählen Sie **Gruppierung 1**.
1. Auswählen **Marketo Sales Clicked/Marketo Sales Viewed,** then **Summe** in den Zusammenfassungsfeldern.
1. Fügen Sie der Formel ein Trennzeichen hinzu und wählen Sie dann **Datensatzanzahl** in den Feldern &quot;Zusammenfassung&quot;- _Speichern unter_.

## Vorlagenleistungsbericht {#template-performance-report}

1. Anpassen des Berichts &quot;Öffnen und Klicken&quot;, um die folgenden Felder einzuschließen: _Speichern unter_.

## Vorlagenvolumenbericht {#template-volume-report}

1. Ändern Sie den Vorlagenleistungsbericht und fügen Sie den Filter &quot;Marketo Sales Template not equal to blank&quot;ein.
1. Entfernen Sie das Feld Marketo Sales Clicked : _Speichern unter_.

## Trendberichte zu Konten {#trending-accounts-report}

1. Wählen Sie Aktivitäten mit Datensatztyp Konten aus.
1. Richten Sie die Berichtsparameter und -felder wie unten angegeben ein - _Speichern unter_.
