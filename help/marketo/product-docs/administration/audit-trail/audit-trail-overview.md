---
unique-page-id: 11377945
description: Überblick über das Audit-Protokoll und wie es einen sechsmonatigen Verlauf der Änderungen und Anmeldeaktivitäten in Ihrer Marketo-Instanz erfasst.
title: Überblick über Audit-Protokolle
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
TQID: https://experienceleague.adobe.com/4MTpv09ZFWkX6tirnq7ZIABSkfoz07qljcUUORwYNn8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 2%

---

# Überblick über Audit-Protokolle {#audit-trail-overview}

Das Audit-Protokoll bietet Ihnen die Möglichkeit, einen vollständigen Verlauf (sechs Monate) der Änderungen abzurufen, die in Ihrer Marketo-Instanz vorgenommen wurden.

>[!NOTE]
>
>Der Verlauf der Audit-Protokoll-Daten begann am 14. September 2016.

![](assets/audit-trail-overview-1.png)

## Was ist Audit-Protokoll {#what-is-audit-trail}

Das Audit-Protokoll erfasst in Echtzeit eine umfassende Liste von Aktionen und Ereignissen, die innerhalb eines Marketo-Abonnements auftreten. Es bietet eine Self-Service-Option für den Zugriff auf einen sechsmonatigen Datenverlauf, damit sich zum Beispiel folgende Fragen beantworten lassen:

„Was ist mit diesem Asset oder dieser Einstellung passiert und wer hat es zuletzt aktualisiert?“

„Was hat Benutzer X so gemacht?“

„Wer meldet sich bei unserem Konto an?“

## Was wir prüfen {#what-we-audit}

Marketo prüft die [Erstellen, Bearbeiten und Löschen](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) für:

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

Ermitteln Sie, wer sich wann bei Ihrem Abonnement angemeldet hat (einschließlich fehlgeschlagener Anmeldeversuche).

>[!TIP]
>
>Da Sie mit dem Audit-Protokoll so viele Audits durchführen können[&#x200B; kann &#x200B;](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) Filtern viel Zeit sparen.

## Daten werden exportiert {#exporting-data}

Sie können nur Daten von 30 Tagen in Ihrer Instanz anzeigen. Verwenden Sie die Exportoption, um einen Zeitraum von (bis zu) sechs Monaten zu erhalten.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Unbekannt:** In [!DNL Webhook] werden der Name und die E-Mail-Adresse von Benutzenden möglicherweise als „Unbekannt“ aufgeführt. Dies geschieht, wenn Sie die Werte Ihrer Auswahllisten in Ihrem CRM ändern. Diese Werte werden in Marketo Forms und Landingpages angezeigt. Wenn Sie diese Aktualisierung auf CRM-Seite durchführen, werden Ihre Landingpages mit Verweis auf das Formular automatisch erstellt. In [!DNL Webhook] erfasst Marketo, dass die Landingpage entworfen wurde, aber der Name und die E-Mail-Adresse des Benutzers werden als „Unbekannt“ angezeigt, da Marketo die Benutzerinformationen nicht von der CRM-Seite erfassen kann.

>[!MORELIKETHIS]
>
>[Audit-Protokoll aktivieren](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
