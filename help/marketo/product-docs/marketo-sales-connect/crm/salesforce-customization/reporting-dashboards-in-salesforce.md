---
unique-page-id: 14352464
description: Berichte-Dashboard in Salesforce - Marketing Docs - Produktdokumentation
title: Berichte-Dashboards in Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Berichte-Dashboard in Salesforce {#reporting-dashboards-in-salesforce}

Hier erfahren Sie, wie Sie Dashboard einrichten.

## Öffnen und auf Bericht {#open-and-click-report} klicken

1. Wählen Sie den Datensatztyp **Aufgaben und Ereignis** aus.
1. Definieren Sie die Berichtsparameter basierend auf Ihrem gewünschten Zeitraum und Ihrer Hierarchiestruktur.
1. hinzufügen Sie einen Filter, um bei Salesforce angemeldete interne E-Mails zu entfernen (z. B. Firma/Konto nicht gleich Marketo).
1. Wählen Sie das Berichtsformat **Zusammenfassung**.
1. hinzufügen die Felder Betreff, Zugewiesen und Marketo-Verkauf angeklickt/Verkauf angezeigt zum Bericht.
1. Klicken Sie im Bereich &quot;Felder&quot;mit der Dublette auf **Hinzufügen Formel**.
1. hinzufügen Sie der Formel einen Namen, wählen Sie **Prozent** im Format aus und wählen Sie **Gruppierung 1**.
1. Wählen Sie **Angeklickter/marketo-Verkauf,** und **Summe** in den Zusammenfassungsfeldern.
1. hinzufügen Sie ein Divide-Zeichen zur Formel und wählen Sie dann **Record Count** in den Feldern Summary - _Save As_.

## Vorlagenleistungsbericht {#template-performance-report}

1. Passen Sie den Bericht Öffnen und Klicken an, um die folgenden Felder einzuschließen: _Speichern unter_.

## Vorlagenvolumenbericht {#template-volume-report}

1. Ändern Sie den Bericht &quot;Vorlagenleistung&quot;und fügen Sie den Filter &quot;Vorlage für den Vertrieb nicht leer&quot;ein.
1. Entfernen Sie das angeklickte Feld Markieren zum Verkauf - _Speichern unter_.

## Trendkontenbericht {#trending-accounts-report}

1. Wählen Sie Aktivitäten mit Datensatztyp &quot;Konten&quot;aus.
1. Richten Sie die Berichtsparameter und -felder wie unten beschrieben ein - _Speichern unter_.
