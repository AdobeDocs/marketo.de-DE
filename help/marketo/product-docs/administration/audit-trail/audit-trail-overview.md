---
unique-page-id: 11377945
description: Audit-Trail-Übersicht - Marketing-Dokumente - Produktdokumentation
title: Übersicht über Prüfprotokolle
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Übersicht über Prüfprotokolle {#audit-trail-overview}

Audit Trail bietet Ihnen die Möglichkeit, einen vollständigen Verlauf (sechs Monate) von Änderungen zu erhalten, die in Ihrer Marketo-Instanz vorgenommen wurden.

>[!NOTE]
>
>Der Audit-Trail-Datenverlauf begann am 14. September 2016.

![](assets/one.png)

## Was ist Prüfpfad {#what-is-audit-trail}

Audit Trail erfasst in Echtzeit eine umfassende Liste von Aktionen und Ereignissen, die in einem Marketing-Abonnement auftreten. Es bietet eine Self-Service-Möglichkeit zum Zugriff auf eine sechsmonatige Datengeschichte, um Antworten auf Fragen wie die folgenden zu erhalten:

Was ist mit diesem Asset oder dieser Einstellung passiert und wer hat es zuletzt aktualisiert?

Was hat Benutzer X bisher gemacht?

Wer meldet sich bei unserem Konto an?

## Was wir prüfen {#what-we-audit}

Marketo prüft die Aktionen zum [Erstellen, Bearbeiten und Löschen](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) für:

* Design von Studio-Assets
* Alle Programm
* Intelligente Kampagnen
* Listen (intelligent/statisch)
* Benutzer (Admin)
* Rollen und Berechtigungen (Admin)
* Arbeitsbereich und Partitionen (Admin)
* Anmeldeverlauf des Benutzers

>[!NOTE]
>
>Marketo prüft derzeit **keine** Änderungen, die in Web-Personalisierung, Predictive Content oder Sales Insight vorgenommen wurden.

## Prüfprotokoll-Komponenten {#audit-trail-components}

Prüfpfad besteht aus drei Komponenten.

**1) [Asset-Prüfpfad](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

Siehe Aktivität für bestimmte Assets.

**2) [Admin-Prüfpfad](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

Überwachen Sie benutzerbasierte Details.

**3) [Benutzeranmeldeverlauf](http://docs.marketo.com/display/DOCS/User+Login+History)**

Erkennen Sie, wer sich bei Ihrem Abonnement angemeldet hat und wann. Enthält auch fehlgeschlagene Anmeldeversuche.

>[!TIP]
>
>Es gibt so viel, dass Sie prüfen können mit Audit Trail, stellen Sie sicher, verwenden Sie [Filter](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## Exportieren von Daten {#exporting-data}

Sie können in Ihrer Instanz nur Daten im Wert von 30 Ansichten speichern. Verwenden Sie die Exportoption, um einen Wert von bis zu sechs Monaten zu erhalten.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Unbekannt:** Im Audit-Protokoll werden der Name und die E-Mail eines Benutzers als &quot;Unbekannt&quot;aufgeführt. Dies geschieht, wenn Sie eine Änderung an Ihren picklist-Werten in Ihrem CRM vornehmen. Diese Werte werden in Marketo-Formularen und -Landingpages angezeigt. Wenn Sie dieses Update auf der CRM-Seite durchführen, werden Ihre Landingpages automatisch entworfen, die auf das Formular verweisen. Im Audit-Protokoll werden wir feststellen, dass die Landingpage entworfen wurde, aber der Benutzername und die E-Mail-Adresse werden als &quot;Unbekannt&quot;angezeigt, da wir die Benutzerinformationen nicht von der CRM-Seite aus erfassen können.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Prüfpfad aktivieren](enable-audit-trail.md)

>



