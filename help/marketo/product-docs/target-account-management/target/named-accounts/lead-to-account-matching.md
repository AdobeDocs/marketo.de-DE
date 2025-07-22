---
unique-page-id: 11381156
description: Lead-Konto-Zuordnung - Marketo-Dokumente - Produktdokumentation
title: Lead-Konto-Zuordnung
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Lead-Konto-Zuordnung {#lead-to-account-matching}

Abgleichen von rechten Leads zu Konten mit rechtlichem Namen mithilfe von Marketo Lead-Konto-Abgleich.

>[!NOTE]
>
>**Lead-Konto-Zuordnung** ist eine integrierte Funktion von Marketo [!UICONTROL Target-]. Es wird Fuzzy-Logik verwendet, um Leads nahezu in Echtzeit automatisch mit den richtigen benannten Konten abzugleichen. Bei diesen benannten Konten kann es sich um CRM-Konten oder Marketo-Unternehmen handeln.

## Überblick {#overview}

Die Lead-Konto-Zuordnung von Marketo erfolgt in vier Schritten:

**Schritt 1 -** Unser Abgleichsprozess beginnt mit der Verwendung von Schlüsselinformationen zu den Lead-Datensätzen, z. B.:

* E-Mail-Domain (z. B. acme.com)
* Abgeleiteter Firmenname aus IP-Adresse
* Firmenname - Dies kann der CRM-Kontoname oder das Attribut des Lead-Firmennamens sein (z. B. vom Ausfüllen des Formulars)

**Schritt 2 -** Wir normalisieren die Firmennamen, die wir basierend auf verschiedenen Lead-Attributen finden (z. B. werden Acme Inc. und Acme Corp automatisch auf Acme normalisiert). Dieser Schritt stellt sicher, dass wir eine einzige Darstellung des benannten Kontos in Marketo haben und alle Leads in einem einzigen benannten Konto sehen können.

**Schritt 3 -** Wir teilen abgeglichene Leads in 2 Buckets auf: Strong Match und Weak Match.

* Leads mit schwacher Übereinstimmung werden in den benannten Konten angezeigt, die dann manuell aufgelöst werden können.

**Schritt 4 -** Wir präsentieren eine Liste von vorgeschlagenen Unternehmen mit starken und schwachen Übereinstimmungen. Wenn ein benanntes Konto auf der Grundlage eines der vorgeschlagenen Unternehmen erstellt wird, erstellen wir übereinstimmende Regeln, um neue Leads (z. B. Leads, die ein Formular ausgefüllt haben) automatisch den richtigen benannten Konten zuzuordnen. Auf diese Weise können Sie sich weniger Gedanken über übereinstimmende Leads machen und mehr darüber, Umsätze zu erzielen!

Da die Lead-Konto-Zuordnung von Marketo eine integrierte Funktion von Marketo [!UICONTROL Target Account Management] ist, erfolgt die Zuordnung von Leads zu Konten nahezu in Echtzeit (z. B. in dem Moment, in dem ein Lead ein Marketo-Formular ausfüllt, verknüpfen wir diesen Lead mit dem richtigen benannten Konto). Dieses Ereignis kann verwendet werden, um Warnhinweise Trigger und Kontoinhaber über die neuen Leads zu informieren, die von ihren benannten Konten eingehen.

>[!NOTE]
>
>Wenn Sie LeanData in Salesforce für die Lead-Konto-Zuordnung verwenden, verfügt Marketo über eine Integration, die diese Übereinstimmungen mit Ihrer Marketo-Instanz synchronisiert. Um diese Funktion aktivieren zu lassen, wenden Sie sich bitte an den [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) Im Folgenden erfahren Sie, wie Sie LeanData einrichten.

## LeanData für Lead-Konto-Zuordnung verwenden {#using-leandata-for-lead-to-account-matching}

Nachdem der [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) LeanData für Ihr Konto aktiviert hat, führen Sie die folgenden Schritte aus, um es einzurichten.

1. Klicken Sie in Salesforce **[!UICONTROL Startseite einrichten]** im linken Navigationsbereich.

1. Klicken Sie im linken Navigationsbereich unter Administration auf **[!UICONTROL Benutzer]** und dann **[!UICONTROL Profile]**.

1. Suchen Sie das Profil **Marketo Sync** und wählen Sie es aus.

1. Scrollen Sie nach unten zum Abschnitt Sicherheit auf Feldebene und suchen Sie das Lead -Objekt. Wählen Sie **[!UICONTROL Ansicht]** aus.

1. Stellen Sie für den Feldnamen „Reporting Matched Account“ sicher, dass das Kontrollkästchen in der Spalte **[!UICONTROL Lesezugriff]** aktiviert ist.

1. Navigieren Sie in Marketo zum Abschnitt **[!UICONTROL Admin]** .

   ![](assets/lead-to-account-matching-1.png)

1. Wählen Sie **[!UICONTROL Feldverwaltung]** aus.

   ![](assets/lead-to-account-matching-2.png)

1. Bestätigen Sie, dass das Feld vorhanden ist, indem Sie nach &quot;[!UICONTROL Abgestimmtes Berichtskonto“ ].

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Erkunden von Konten](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
