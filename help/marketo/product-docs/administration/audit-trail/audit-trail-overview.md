---
unique-page-id: 11377945
description: Audit-Protokoll - Marketo-Dokumente - Produktdokumentation
title: Audit-Protokoll - Überblick
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Audit-Protokoll - Überblick {#audit-trail-overview}

Mit dem Audit-Protokoll können Sie einen vollständigen Verlauf (im Wert von sechs Monaten) der in Ihrer Marketo-Instanz vorgenommenen Änderungen abrufen.

>[!NOTE]
>
>Der Datenverlauf des Audit-Protokolls begann am 14. September 2016.

![](assets/audit-trail-overview-1.png)

## Was ist das Audit-Protokoll {#what-is-audit-trail}

Das Audit-Protokoll erfasst in Echtzeit eine umfassende Liste von Aktionen und Ereignissen, die innerhalb eines Marketo-Abonnements auftreten. Es bietet eine Self-Service-Möglichkeit für den Zugriff auf einen sechsmonatigen Datenverlauf, der Ihnen bei der Beantwortung von Fragen hilft, z. B.:

Was ist mit diesem Asset oder dieser Einstellung passiert und wer hat es zuletzt aktualisiert?

Was hat Benutzer X so gemacht?

Wer meldet sich bei unserem Konto an?

## Was wir überprüfen {#what-we-audit}

Marketo prüft die [Aktionen zum Erstellen, Bearbeiten und Löschen von](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) für:

* Erstellen von Studio-Assets
* Alle Marketo-Programme
* Smart-Kampagnen
* Listen (smart/static)
* Benutzer (admin)
* Rollen und Berechtigungen (Admin)
* Workspace und Partitionen (admin)
* Anmeldeverlauf des Benutzers

>[!NOTE]
>
>Marketo prüft derzeit Änderungen, die in Web Personalization, Predictive Content oder Sales Insight vorgenommen wurden, _nicht_.

## Audit-Protokollkomponenten {#audit-trail-components}

Audit-Protokoll besteht aus drei Komponenten.

**1) [Asset-Audit-Protokoll](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Siehe Aktivitäten, die mit bestimmten Assets durchgeführt wurden.

**2) [Audit-Protokoll für Administratoren](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Überwachen benutzerbasierter Details.

**3) [User Login History](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Finden Sie heraus, wer sich bei Ihrem Abonnement angemeldet hat und wann. Enthält auch fehlgeschlagene Anmeldeversuche.

>[!TIP]
>
>Es gibt so viel, was Sie mit dem Audit-Protokoll überprüfen können. Verwenden Sie unbedingt den [Filter](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Daten werden exportiert {#exporting-data}

Sie können nur Daten im Wert von 30 Tagen in Ihrer Instanz anzeigen. Verwenden Sie die Exportoption, um (bis zu) einen Zeitraum von sechs Monaten zu erhalten.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Unbekannt:** In [!DNL Webhook] werden der Name und die E-Mail eines Benutzers möglicherweise als &quot;Unbekannt&quot;aufgeführt. Dies geschieht, wenn Sie Ihre Picklist-Werte in Ihrem CRM-System ändern. Diese Werte werden in Marketo forms und Landingpages angezeigt. Durch diese Aktualisierung auf der CRM-Seite werden Ihre Landingpages, die auf das Formular verweisen, automatisch entworfen. In [!DNL Webhook] erfassen wir, dass die Landingpage entworfen wurde. Der Name des Benutzers und die E-Mail-Adresse werden jedoch als &quot;Unbekannt&quot;angezeigt, da wir die Benutzerinformationen nicht von der CRM-Seite aus erfassen können.

>[!MORELIKETHIS]
>
>[Audit-Protokoll aktivieren](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
