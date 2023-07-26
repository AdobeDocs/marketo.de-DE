---
unique-page-id: 11378812
description: Discover Accounts - Marketo Docs - Produktdokumentation
title: Discover-Konten
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 2%

---

# Discover-Konten {#discover-accounts}

Verwenden Sie die Discover -Option, um potenzielle Zielkonten zu identifizieren.

## CRM-Kontos entdecken {#discover-crm-accounts}

Identifizieren Sie potenzielle Zielkonten aus Ihrem CRM-System.

>[!NOTE]
>
>Nachdem Sie Ihr CRM mit Marketo TAM verbunden haben, **CRM-Konten kennenlernen** zeigt alle CRM-Konten und relevante Informationen an, die Ihnen bei der Auswahl der richtigen benannten Konten helfen. Marketo fügt zusätzlich zu den vom CRM-System empfangenen Informationen weitere Informationen hinzu.

**Personen** (In Discover CRM-Konten und Discover Marketo-Unternehmen): Enthält Kontakte und Leads. Leads können mit Marketo [Lead-zu-Konto-Abgleich](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**Potenzielle Personen** (In Discover CRM-Konten und Discover Marketo-Unternehmen): Zeigt an, wie viele Leads Marketo gefunden hat, die möglicherweise zu einem CRM-Konto gehören könnten.

**Benutzerdefiniertes CRM-Feld** (Nur in Discover CRM-Konten): Dies hilft Ihnen, Ihre Vertriebs- und Marketingorganisation auf die Auswahl der richtigen Zielkonten auszurichten. Einmal [Zuordnen des benutzerdefinierten CRM-Felds](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) Mit Marketo TAM zeigen wir Ihnen die zugeordneten Daten, die Ihnen bei der Identifizierung Ihrer Zielkonten helfen.

1. Klicken Sie in &quot;Spezifische Konten&quot;auf die **Neu** und wählen Sie **CRM-Konten kennenlernen**.

   ![](assets/disc-crm-one.png)

1. Daraufhin wird ein neues Fenster/eine neue Registerkarte geöffnet. Wählen Sie die CRM-Konten aus, die Sie Ihren spezifischen Konten hinzufügen möchten, und klicken Sie auf **Nächste**.

   ![](assets/disc-crm-two.png)

1. Der Vorschaubildschirm bestätigt die Anzahl der ausgewählten Optionen. Klicken Sie auf **Erstellen**.

   ![](assets/disc-three.png)

   Das ist alles!

   ![](assets/disc-four.png)

## Marketo-Unternehmen entdecken {#discover-marketo-companies}

Identifizieren Sie die richtigen Unternehmen für die Zielgruppenbestimmung.

>[!NOTE]
>
>In Discover Marketo-Unternehmen sehen Sie Marketo-Unternehmen, die nicht aus Ihrem CRM-System stammen.

1. Klicken Sie in &quot;Spezifische Konten&quot;auf die **Neu** und wählen Sie **Entdecken Sie Marketo-Unternehmen**.

   ![](assets/one-1.png)

1. Daraufhin wird ein neues Fenster/eine neue Registerkarte geöffnet. Wählen Sie die Unternehmen aus, die Sie Ihren spezifischen Konten hinzufügen möchten, und klicken Sie auf **Nächste**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >In Discover Marketo-Unternehmen und Discover-CRM wird Marketo automatisch:
   >
   >* Findet Personen aus Ihrer Marketo-Datenbank, bei denen dieses Unternehmen in seinem Datensatz aufgeführt ist. Wenn mehrere Werte für einige der Attribute (z. B. &quot;Branche&quot;) angezeigt werden, liegt dies daran, dass Marketo für diese Personen unterschiedliche Werte gefunden hat. Das Attribut mit den meisten Treffern gewinnt
   >
   >In **CRM kennenlernen** nur Marketo automatisch:
   >
   >* Synchronisiert und verknüpft CRM-Kontakte mit dem benannten Konto
   >
   >In **Entdecken Sie Marketo-Unternehmen** nur Marketo automatisch:
   >
   >* Filtert die meisten Internet Service Provider und Public Domains (z. B. yahoo.com, gmail.com) als Unternehmensnamen heraus
   >
   >* Dedupliziert CRM-Konten. Wenn Sie &quot;Acme&quot;in einem Datensatz und &quot;Acme Inc&quot; (oder eines der folgenden Suffixe: Co, Corp, Corporation, GmbH, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC) haben, werden wir sie in TAM als &quot;Acme&quot;zusammenführen.
   >
   >Wenn Sie möchten, dass Marketo Konten nach CRM-ID oder Kontoinhaber anstatt nach Unternehmensname dedupliziert, wenden Sie sich an [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Klicken Sie unter der Spalte &quot;Spezifisches Konto&quot;auf den Abwärtspfeil, um die Dropdown-Liste anzuzeigen.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >Künftig werden alle neuen Personen aus diesen ausgewählten Unternehmen automatisch ihren jeweiligen benannten Konten zugewiesen. Überprüfen Sie diese Unternehmen und stellen Sie sicher, dass sie dem richtigen benannten Konto zugewiesen sind.

1. Um ein vorhandenes Konto auszuwählen, klicken Sie auf die Schaltfläche **Benanntes Konto** in der Dropdown-Liste, das gewünschte Konto auswählen und auf **Nächste**.

   ![](assets/disc-comp-four.png)

   Sie können auch ein neues benanntes Konto erstellen, indem Sie den gewünschten Namen direkt in das Dropdown-Feld eingeben. Klicken Sie nach Abschluss des Vorgangs aus dem Feld..

   ![](assets/disc-comp-five.png)

   ... und Sie sehen Ihr neues benanntes Konto. Klicken Sie an diesem Punkt auf **Nächste** wie in Schritt 4.

   ![](assets/disc-comp-six.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/disc-comp-seven.png)

   Gut gemacht!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Wenn zwischen den von Ihnen ausgewählten CRM-Konten und den Elementen im Discover CRM-Raster Abweichungen auftreten, liegt dies wahrscheinlich an einer oder mehreren der folgenden Ursachen:
>
>* Verschiedene CRM-Konten mit ähnlichen Namen, die dedupliziert wurden
>* Die nächste geplante Synchronisation ist noch nicht erfolgt.

>[!MORELIKETHIS]
>
>[Lead zur Kontoübereinstimmung](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
