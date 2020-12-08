---
unique-page-id: 11381156
description: Interessentenabgleich - Marketing Docs - Produktdokumentation
title: Interessenten-zu-Konto-Übereinstimmung
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Interessenten-zu-Konto-Übereinstimmung {#lead-to-account-matching}

Die Übereinstimmungsrechte führen zu rechtsbenannten Konten mit der Abgleichung von &quot;Interessent zu Konto&quot;.

>[!NOTE]
>
>**Die Interessenten-zu-Konto-Übereinstimmung** ist eine integrierte Funktion von Marketing-to-Account-basiertem Marketing. Es verwendet unscharfe Logik, um automatisch Interessenten zu den richtigen Konten in Echtzeit zuzuordnen. Diese benannten Konten können CRM-Konten oder Marketo-Firmen sein.

Die Suche nach einer Marketing-to-Account-Übereinstimmung erfolgt in vier Schritten:

**Schritt 1 -** Unser Abgleichprozess beginnt mit der Verwendung wichtiger Informationen zu den Interessentendatensätzen, z. B.:

* E-Mail-Domäne (z. B. acme.com)
* Vorgestellter Name der Firma aus IP-Adresse
* Name der Firma - Dies könnte der CRM-Kontoname oder das Namensattribut der Interessenten-Firma sein, z. B. aus dem Ausfüllen des Formulars

**Schritt 2 -** Wir normalisieren die Firmen, die wir auf Grundlage verschiedener Interessentenattribute finden (z.B. Acme Inc. und Acme Corp werden automatisch zu Acme normalisiert). Dieser Schritt stellt sicher, dass wir eine einzige Darstellung des benannten Kontos in Marketo haben und alle Interessenten in einem einzigen benannten Konto sehen können.

**Schritt 3 -** Wir partitionieren übereinstimmende Interessenten in 2 Behälter: Starke Übereinstimmung und schwache Übereinstimmung.

* Auf den benannten Konten werden weniger übereinstimmende Interessenten angezeigt, die dann manuell behoben werden können.

**Schritt 4 -** Wir stellen eine Liste der vorgeschlagenen Firmen mit starken und schwachen Übereinstimmungen vor. Wenn ein benanntes Konto auf der Grundlage einer der vorgeschlagenen Firmen erstellt wird, erstellen wir Übereinstimmungsregeln, um automatisch neue Interessenten (z. B. Interessenten, die ein Formular ausgefüllt haben) zuzuordnen, die an die richtigen benannten Konten weitergeleitet werden. Auf diese Weise können Sie sich weniger um die Zuordnung von Interessenten und mehr um die Erzielung von Umsatz sorgen!

Da die Interessenten-zu-Konto-Abwägung von Marketo eine integrierte Funktion des Marketing-Kontos ist, erfolgt die Abgleichung von Interessenten in Echtzeit (z. B. wenn ein Interessent ein Marketo-Formular ausfüllt, verbinden wir diesen Interessenten mit dem richtig benannten Konto). Dieses Ereignis kann verwendet werden, um Warnungen auszulösen und Kontoinhaber über die neuen Interessenten zu informieren, die von ihren benannten Konten eingehen.

>[!NOTE]
>
>Wenn Sie LeanData in Salesforce verwenden, um eine Interessenten-zu-Konto-Übereinstimmung zu erzielen, verfügt Marketo über eine Integration, die diese Übereinstimmungen mit Ihrer Marketing-Instanz synchronisiert. Wenden Sie sich zwecks Aktivierung dieser Funktion an den [MarketingTo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>* [Discover-Konten](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md)

