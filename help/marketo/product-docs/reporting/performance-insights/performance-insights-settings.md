---
unique-page-id: 13795492
description: Einstellungen für Performance Insights - Marketo-Dokumente - Produktdokumentation
title: Einstellungen für Performance Insights
exl-id: 894df9de-d416-44f7-8253-ebf3c2a36c90
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 10%

---

# [!UICONTROL Performance Insights] Einstellungen {#performance-insights-settings}

Erfahren Sie mehr über die verschiedenen Einstellungsoptionen in MPI.

![](assets/1-3.png)

>[!NOTE]
>
>Je nachdem, in welchem Dashboard Sie sich befinden, werden unterschiedliche Einstellungsoptionen angezeigt.

## Anzeigen des Programmerfolgs nach {#view-program-success-by}

**[!UICONTROL Interaktion] Dashboard - Beitrag und Trend**

<table>
 <tbody>
  <tr>
   <td><strong>Kostenzeitraum</strong></td>
   <td>Wenn Sie dies aktivieren, aggregieren Performance Insights alle neuen Namen und Erfolge zurück zum Monat, der als Kostenzeitraum eingerichtet wurde.</td>
  </tr>
  <tr>
   <td><strong>Aktivitätszeitraum</strong></td>
   <td>Wenn Sie dies aktivieren, aggregieren Performance Insights alle neuen Namen, Erfolge und Zugehörigkeiten nach Aktivitätsdatum, unabhängig vom Programmkostenzeitraum.</td>
  </tr>
 </tbody>
</table>

## Konfiguration vorheriger Zeitraum {#previous-period-configuration}

**[!UICONTROL Interaktion], [!UICONTROL Pipeline], [!UICONTROL Umsatz] Dashboards - nur Beitrag**

<table>
 <tbody>
  <tr>
   <td><strong>Kalenderzeitraum</strong></td>
   <td>Legen Sie die vorherige Periode wie folgt fest: vorherigen Kalendermonat, Quartal oder Jahr.</td>
  </tr>
  <tr>
   <td><strong>Jahresübergreifender Zeitraum</strong></td>
   <td>Stellen Sie den vorherigen Zeitraum auf denselben Monat oder dasselbe Quartal im Vorjahr ein.</td>
  </tr>
 </tbody>
</table>

## Marketing-beeinflusste Opportunities {#marketing-influenced-opportunities}

**[!UICONTROL Pipeline] Dashboard - Beitrag und Trend**

<table>
 <tbody>
  <tr>
   <td><strong>Erstkontakt anzeigen, bevor Opportunity erstellt wird</strong></td>
   <td><p>Wenn Sie diese Option aktivieren, enthält das MPI Opportunities, die mit mindestens einem Lead verknüpft sind, der vor der Erstellung der Opportunity von einem Marketo-Programm erworben wurde (Erstkontakt/FTP). Es gelten die Einstellungen für explizite, implizite und hybride Attribution .</p></td>
  </tr>
  <tr>
   <td><strong>Multi-Touch anzeigen, bevor Opportunity erstellt wird</strong></td>
   <td><p>Wenn Sie diese Option aktivieren, enthält das MPI Opportunities mit mindestens einem Lead, der vor der Erstellung der Opportunity von einem Marketo-Programm erworben wurde (Multi-Touch/MT). Es gelten die Einstellungen für explizite, implizite und hybride Attribution .</p></td>
  </tr>
 </tbody>
</table>

**[!UICONTROL Umsatz] Dashboard - Beitrag und Trend**

<table>
 <tbody>
  <tr>
   <td><strong>Erstkontakt anzeigen, vor Abschluss der Opportunity</strong></td>
   <td><p>Wenn Sie diese Option aktivieren, enthält das MPI Opportunities, die mit mindestens einem Lead verbunden sind, der vor Abschluss der Opportunity von einem Marketo-Programm erworben wurde (Erstkontakt/FTP). Es gelten die Einstellungen für explizite, implizite und hybride Attribution .</p></td>
  </tr>
  <tr>
   <td><strong>Multi-Touch anzeigen, bevor die Opportunity geschlossen wird</strong></td>
   <td><p>Wenn Sie diese Option aktivieren, enthält das MPI Opportunities mit mindestens einem Lead, der vor Abschluss der Opportunity von einem Marketo-Programm erworben wurde (Multi-Touch/MT). Es gelten die Einstellungen für explizite, implizite und hybride Attribution .</p></td>
  </tr>
 </tbody>
</table>

## Kostenberechnung {#cost-calculation}

**[!UICONTROL Pipeline] und [!UICONTROL Umsatz] Dashboards - Beitrag und Trend**

<table>
 <tbody>
  <tr>
   <td><strong>Basierend auf dem Investitionszeitraum</strong></td>
   <td>Die Investitionskosten werden einfach als Summe der monatlichen Programmkosten berechnet, die durch den Investitionszeitraumfilter definiert werden.</td>
  </tr>
  <tr>
   <td><strong>Basierend auf der Programmzuweisung</strong></td>
   <td>Die zugewiesenen Kosten basieren auf einem Teil der Programmkosten, der durch Leads oder Kontakte bestimmt wird, die im Programm erworben oder erfolgreich abgeschlossen wurden und letztendlich zu einer gewonnenen Opportunity geführt haben.</td>
  </tr>
 </tbody>
</table>
