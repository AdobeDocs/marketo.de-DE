---
unique-page-id: 14352464
description: Reporting-Dashboards in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Berichterstellungs-Dashboards in Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 4%

---

# Berichterstellungs-Dashboards in Salesforce {#reporting-dashboards-in-salesforce}

Im Folgenden erfahren Sie, wie Sie Dashboards einrichten.

## Bericht öffnen und klicken {#open-and-click-report}

1. Wählen Sie **[!UICONTROL Datensatztyp]** Aufgaben und Ereignisse“ aus.
1. Definieren Sie die Berichtsparameter basierend auf Ihrem gewünschten Zeitrahmen und Ihrer Hierarchiestruktur.
1. Fügen Sie einen Filter hinzu, um interne E-Mails zu entfernen, die in [!DNL Salesforce] protokolliert wurden (z. B. Unternehmen/Konto, das nicht Marketo entspricht).
1. Wählen Sie das **[!UICONTROL Zusammenfassung]** Berichtsformat aus.
1. Fügen Sie die Felder „Betreff“, „Zugewiesen“ und &quot;Marketo-Vertrieb angeklickt/Marketo-Vertrieb angezeigt“ zum Bericht hinzu.
1. Doppelklicken Sie auf **[!UICONTROL Formel hinzufügen]** im Bereich Felder .
1. Fügen Sie der Formel einen Namen hinzu, wählen Sie **[!UICONTROL Prozent]** im Format aus und wählen Sie **[!UICONTROL Gruppierung 1]** aus.
1. Wählen Sie **[!UICONTROL Marketo Sales klickte/Marketo Sales Viewed]** und dann **[!UICONTROL sum]** in den Zusammenfassungsfeldern aus.
1. Fügen Sie der Formel ein Trennzeichen hinzu und wählen Sie dann **[!UICONTROL Datensatzanzahl]** in den Zusammenfassungsfeldern - _Speichern unter_.

## Vorlagen-Leistungsbericht {#template-performance-report}

1. Passen Sie den Bericht Öffnen und Klicken an, um die folgenden Felder einzuschließen: _Speichern unter_.

## Vorlagenvolumenbericht {#template-volume-report}

1. Ändern Sie den Vorlagenleistungsbericht und schließen Sie den Filter &quot;Marketo-Verkaufsvorlage ist nicht leer“ ein.
1. Entfernen Sie das Feld Angeklickter Marketo-Vertrieb _Speichern unter_.

## Bericht zu Trend-Konten {#trending-accounts-report}

1. Wählen Sie Aktivitäten mit dem Datensatztyp Konten aus.
1. Richten Sie die Berichtsparameter und -felder wie unten angegeben ein - _Speichern unter_.
