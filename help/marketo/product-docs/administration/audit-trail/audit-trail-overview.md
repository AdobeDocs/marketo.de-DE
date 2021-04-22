---
unique-page-id: 11377945
description: Übersicht über den Prüfpfad - Marketo Dokumente - Produktdokumentation
title: Übersicht über Prüfprotokolle
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Prüfpfad-Übersicht {#audit-trail-overview}

Audit Trail bietet Ihnen die Möglichkeit, einen vollständigen Verlauf der in Ihrer Marketo-Instanz vorgenommenen Änderungen (im Wert von sechs Monaten) zu erhalten.

>[!NOTE]
>
>Der Audit-Trail-Datenverlauf begann am 14. September 2016.

![](assets/one.png)

## Was ist Prüfpfad {#what-is-audit-trail}

Audit Trail erfasst in Echtzeit eine umfassende Liste von Maßnahmen und Ereignissen, die in einem Marketo-Abonnement auftreten. Es bietet eine Self-Service-Möglichkeit zum Zugriff auf eine sechsmonatige Datengeschichte, um Antworten auf Fragen wie die folgenden zu erhalten:

Was ist mit diesem Asset oder dieser Einstellung passiert und wer hat es zuletzt aktualisiert?

Was hat Benutzer X bisher gemacht?

Wer meldet sich bei unserem Konto an?

## Was wir prüfen {#what-we-audit}

Marketo prüft die Aktionen [Erstellen, Bearbeiten und Löschen](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) für:

* Design von Studio-Assets
* Alle Marketo-Programme
* Intelligente Kampagnen
* Listen (intelligent/statisch)
* Benutzer (Admin)
* Rollen und Berechtigungen (Admin)
* Arbeitsbereich und Partitionen (Admin)
* Anmeldeverlauf des Benutzers

>[!NOTE]
>
>Marketo prüft derzeit Änderungen, die in Web-Personalisierung, Predictive Content oder Sales Insight vorgenommen wurden.__

## Prüfprotokoll-Komponenten {#audit-trail-components}

Prüfpfad besteht aus drei Komponenten.

**1)  [Asset-Prüfpfad](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Siehe Aktivität für bestimmte Assets.

**2)  [Admin-Prüfpfad](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Überwachen Sie benutzerbasierte Details.

**3)  [Benutzeranmeldeverlauf](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Erkennen Sie, wer sich bei Ihrem Abonnement angemeldet hat und wann. Enthält auch fehlgeschlagene Anmeldeversuche.

>[!TIP]
>
>Es gibt so viel, dass Sie mit Audit Trail prüfen können, stellen Sie sicher, dass Sie [Filter](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) verwenden!

## Daten werden exportiert {#exporting-data}

Sie können in Ihrer Instanz nur Daten im Wert von 30 Ansichten speichern. Verwenden Sie die Exportoption, um einen Wert von bis zu sechs Monaten zu erhalten.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Unbekannt:** Im Prüfpfad werden der Name und die E-Mail eines Benutzers möglicherweise als &quot;Unbekannt&quot;aufgelistet. Dies geschieht, wenn Sie eine Änderung an Ihren picklist-Werten in Ihrem CRM vornehmen. Diese Werte werden in Marketo-Formularen und -Landingpages angezeigt. Wenn Sie dieses Update auf der CRM-Seite durchführen, werden Ihre Landingpages automatisch entworfen, die auf das Formular verweisen. Im Audit-Protokoll werden wir feststellen, dass die Landingpage entworfen wurde, aber der Benutzername und die E-Mail-Adresse werden als &quot;Unbekannt&quot;angezeigt, da wir die Benutzerinformationen nicht von der CRM-Seite aus erfassen können.

>[!MORELIKETHIS]
>
>[Prüfpfad aktivieren](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
