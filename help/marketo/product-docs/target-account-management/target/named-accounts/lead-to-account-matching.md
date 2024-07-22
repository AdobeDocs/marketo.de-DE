---
unique-page-id: 11381156
description: Lead zur Kontoübereinstimmung - Marketo-Dokumente - Produktdokumentation
title: Lead zur Kontoübereinstimmung
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Lead zur Kontoübereinstimmung {#lead-to-account-matching}

Match right führt zu Konten mit rechtlichem Namen, die Marketo Lead-zu-Konto-Abgleich verwenden.

>[!NOTE]
>
>**Übereinstimmung zwischen Interessenten und Konten** ist eine integrierte Funktion der Marketo Target-Kontoverwaltung. Es verwendet unscharfe Logik, um Leads in nahezu Echtzeit automatisch mit den richtigen benannten Konten abzugleichen. Diese benannten Konten können CRM-Konten oder Marketo-Unternehmen sein.

## Überblick {#overview}

Die Zuordnung von Marketo-Lead zu Konto erfolgt in vier Schritten:

**Schritt 1 -** Unser Abgleichsprozess beginnt mit der Verwendung von Schlüsselinformationen für die Lead-Datensätze, z. B.:

* E-Mail-Domäne (z. B. acme.com)
* Abgeleiteter Firmenname von der IP-Adresse
* Firmenname - Dies kann der CRM-Kontoname oder das Attribut für den Namen des Lead-Unternehmens sein (z. B. stammt aus dem Ausfüllen des Formulars)

**Schritt 2 -** Wir normalisieren die Unternehmensnamen, die wir anhand verschiedener Lead-Attribute finden (z. B. werden Acme Inc. und Acme Corp automatisch in Acme normalisiert). Dieser Schritt stellt sicher, dass wir über eine einzige Darstellung des benannten Kontos in Marketo verfügen und alle Leads in einem einzigen benannten Konto sehen können.

**Schritt 3 -** Wir haben die Leads in 2 Buckets aufgeteilt: Starke Übereinstimmung und schwache Übereinstimmung.

* Auf den benannten Konten werden weniger übereinstimmende Leads angezeigt, die dann manuell aufgelöst werden können.

**Schritt 4 -** Wir stellen eine Liste der vorgeschlagenen Unternehmen mit starken und schwachen Übereinstimmungen vor. Wenn ein benanntes Konto basierend auf einem der vorgeschlagenen Unternehmen erstellt wird, erstellen wir Übereinstimmungsregeln, um automatisch neue Leads (z. B. Lead-Ausfüllen eines Formulars) zu verknüpfen, die an die richtigen benannten Konten weitergeleitet werden. Auf diese Weise können Sie sich weniger um übereinstimmende Leads und mehr um den Umsatz sorgen.

Da der Marketo-Lead-zu-Konto-Abgleich eine integrierte Funktion der Marketo Target-Kontoverwaltung ist, führt der Abgleich fast in Echtzeit zu Konten (wenn z. B. ein Lead ein Marketo-Formular ausfüllt, wird Lead mit dem richtigen benannten Konto verknüpft). Mit diesem Ereignis können Warnhinweise Trigger und Kontoinhaber über die neuen Leads informiert werden, die von ihren benannten Konten eingehen.

>[!NOTE]
>
>Wenn Sie LeanData in Salesforce zum Abgleich von Lead-zu-Konto verwenden, verfügt Marketo über eine Integration, die diese Übereinstimmungen mit Ihrer Marketo-Instanz synchronisiert. Wenden Sie sich zur Aktivierung dieser Funktion an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support). Erfahren Sie unten, wie Sie LeanData einrichten.

## Verwenden von LeanData für Lead-to-Account-Übereinstimmung {#using-leandata-for-lead-to-account-matching}

Nachdem der [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support) LeanData für Ihr Konto aktiviert hat, führen Sie die folgenden Schritte aus, um es einzurichten.

1. Klicken Sie in Salesforce im linken Navigationsbereich auf **Startseite einrichten** .

1. Klicken Sie im linken Navigationsbereich unter &quot;Administration&quot;auf **Benutzer** und dann auf **Profile**.

1. Suchen Sie das Profil &quot;**Marketo Sync**&quot; und wählen Sie es aus.

1. Scrollen Sie nach unten zum Abschnitt Sicherheit auf Feldebene und suchen Sie das Lead-Objekt. Wählen Sie **Ansicht** aus.

1. Stellen Sie für den Feldnamen &quot;Reporting Matched Account&quot;sicher, dass das Kontrollkästchen in der Spalte **Lesezugriff** aktiviert ist.

1. Wechseln Sie in Marketo zum Abschnitt **Admin** .

   ![](assets/lead-to-account-matching-1.png)

1. Wählen Sie **Feldverwaltung** aus.

   ![](assets/lead-to-account-matching-2.png)

1. Vergewissern Sie sich, dass das Feld vorhanden ist, indem Sie nach &quot;Reporting Matched Account&quot;suchen.

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Discover-Konten](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
