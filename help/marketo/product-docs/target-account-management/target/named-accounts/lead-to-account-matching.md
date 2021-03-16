---
unique-page-id: 11381156
description: Interessentenabgleich - Marketing Docs - Produktdokumentation
title: Interessenten-zu-Konto-Übereinstimmung
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Interessenten zu Kontoübereinstimmung {#lead-to-account-matching}

Die Übereinstimmungsrechte führen zu rechtsbenannten Konten mit der Abgleichung von &quot;Interessent zu Konto&quot;.

>[!NOTE]
>
>**Interessenten-zu-Konto-** Übereinstimmung ist eine integrierte Funktion der Marketing Zielgruppe-Kontoverwaltung. Es verwendet unscharfe Logik, um automatisch Interessenten zu den richtigen Konten in Echtzeit zuzuordnen. Diese benannten Konten können CRM-Konten oder Marketo-Firmen sein.

Die Suche nach einer Marketing-to-Account-Übereinstimmung erfolgt in vier Schritten:

**Schritt 1 -** Unser Übereinstimmungsprozess beginnt mit der Verwendung wichtiger Informationen zu den Interessentendatensätzen, z. B.:

* E-Mail-Domäne (z. B. acme.com)
* Vorgestellter Name der Firma aus IP-Adresse
* Name der Firma - Dies könnte der CRM-Kontoname oder das Attribut des Namens der Interessenten-Firma sein (z. B. stammt aus dem Ausfüllen des Formulars)

**Schritt 2 -** Wir normalisieren die Firmen, die wir auf Grundlage verschiedener Interessentenattribute finden (z.B. Acme Inc. und Acme Corp werden automatisch auf Acme normalisiert). Dieser Schritt stellt sicher, dass wir eine einzige Darstellung des benannten Kontos in Marketo haben und alle Interessenten in einem einzigen benannten Konto sehen können.

**Schritt 3 -** Wir partitionieren übereinstimmende Interessenten in 2 Behälter: Starke Übereinstimmung und schwache Übereinstimmung.

* Auf den benannten Konten werden weniger übereinstimmende Interessenten angezeigt, die dann manuell behoben werden können.

**Schritt 4 -** Wir stellen eine Liste der vorgeschlagenen Firmen mit starken und schwachen Übereinstimmungen vor. Wenn ein benanntes Konto auf der Grundlage einer der vorgeschlagenen Firmen erstellt wird, erstellen wir Übereinstimmungsregeln, um automatisch neue Interessenten (z. B. Ausfüllen eines Formulars) zuzuordnen, die an die richtigen benannten Konten weitergeleitet werden. Auf diese Weise können Sie sich weniger um die Zuordnung von Interessenten und mehr um die Erzielung von Umsatz sorgen!

Da Marketo Lead-to-Account-Abgleich eine integrierte Funktion des Kontomanagements von Marketo Zielgruppe ist, erfolgt die Abgleichung von Interessenten zu Konten in Echtzeit (z. B. wenn ein Interessent ein Marketo-Formular ausfüllt, verbinden wir diesen Interessenten mit dem richtig benannten Konto). Dieses Ereignis kann zum Trigger von Warnungen und zur Benachrichtigung der Kontoinhaber über die neuen Interessenten verwendet werden, die von ihren benannten Konten eingehen.

>[!NOTE]
>
>Wenn Sie LeanData in Salesforce verwenden, um eine Interessenten-zu-Konto-Übereinstimmung zu erzielen, verfügt Marketo über eine Integration, die diese Übereinstimmungen mit Ihrer Marketing-Instanz synchronisiert. Um diese Funktion aktivieren zu lassen, wenden Sie sich bitte an [Marketing Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Discover-Konten](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
