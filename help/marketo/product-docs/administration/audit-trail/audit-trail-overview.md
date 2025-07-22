---
unique-page-id: 11377945
description: Audit-Protokoll] Übersicht - Marketo-Dokumente - Produktdokumentation
title: Audit-Protokoll - Übersicht
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Audit-Protokoll - Übersicht {#audit-trail-overview}

Das Audit-Protokoll bietet Ihnen die Möglichkeit, einen vollständigen Verlauf (sechs Monate) der Änderungen abzurufen, die in Ihrer Marketo-Instanz vorgenommen wurden.

>[!NOTE]
>
>Der Verlauf der Audit-Protokoll-Daten begann am 14. September 2016.

![](assets/audit-trail-overview-1.png)

## Was ist Audit-Protokoll {#what-is-audit-trail}

Das Audit-Protokoll erfasst in Echtzeit eine umfassende Liste von Aktionen und Ereignissen, die innerhalb eines Marketo-Abonnements auftreten. Es bietet eine Self-Service-Option für den Zugriff auf einen sechsmonatigen Datenverlauf, damit sich zum Beispiel folgende Fragen beantworten lassen:

Was ist mit diesem Asset oder dieser Einstellung passiert und wer hat es zuletzt aktualisiert?

Was hat Benutzer X so gemacht?

Wer meldet sich bei unserem Konto an?

## Was wir prüfen {#what-we-audit}

Marketo prüft die [Erstellen, Bearbeiten und Löschen](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) Aktionen für:

* Entwerfen von Studio-Assets
* Alle Marketo-Programme
* Intelligente Kampagnen
* Listen (intelligent/statisch)
* Benutzer (Admin)
* Rollen und Berechtigungen (Admin)
* Workspace und Partitionen (admin)
* Anmeldeverlauf des Benutzers

>[!NOTE]
>
>Marketo prüft _nicht_ Änderungen, die derzeit in Web Personalization, Predictive Content oder Sales Insight vorgenommen werden.

## Audit-Protokoll-Komponenten {#audit-trail-components}

Audit-Protokoll besteht aus drei Komponenten.

**1) [Asset-Audit-Protokoll](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Siehe Aktivität für bestimmte Assets.

**2) [Admin-Audit-Protokoll](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Überwachen von benutzerbasierten Details.

**3) [Anmeldeverlauf des Benutzers](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Sehen Sie, wer sich wann bei Ihrem Abonnement angemeldet hat. Umfasst auch fehlgeschlagene Anmeldeversuche.

>[!TIP]
>
>Es gibt so viel, was Sie mit dem Audit-Protokoll prüfen können, stellen Sie sicher, dass Sie [Filtern](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) verwenden.

## Daten werden exportiert {#exporting-data}

Sie können nur Daten von 30 Tagen in Ihrer Instanz anzeigen. Verwenden Sie die Exportoption, um einen Zeitraum von (bis zu) sechs Monaten zu erhalten.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Unbekannt:** In [!DNL Webhook] werden der Name und die E-Mail-Adresse von Benutzenden möglicherweise als „Unbekannt“ aufgeführt. Dies geschieht, wenn Sie die Werte Ihrer Auswahllisten in Ihrem CRM ändern. Diese Werte werden in Marketo Forms und Landingpages angezeigt. Wenn Sie diese Aktualisierung auf CRM-Seite durchführen, werden Ihre Landingpages mit Verweis auf das Formular automatisch erstellt. In [!DNL Webhook] erfassen wir, dass die Landingpage entworfen wurde, aber der Name und die E-Mail-Adresse des Benutzers werden als „Unbekannt“ angezeigt, da wir die Benutzerinformationen nicht von der CRM-Seite erfassen können.

>[!MORELIKETHIS]
>
>[Audit-Protokoll aktivieren](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
