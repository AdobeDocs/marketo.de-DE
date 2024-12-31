---
description: Gründe für Anrufe und Anrufergebnisse in Salesforce protokollieren - Marketo-Dokumente - Produktdokumentation
title: Gründe und Anrufergebnisse bei Salesforce protokollieren
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 3%

---

# Gründe und Anrufergebnisse bei Salesforce protokollieren {#log-call-reasons-and-call-outcomes-to-salesforce}

Wenn Sie Anrufergebnisse und Anrufgründe zu Berichts- oder Sichtbarkeitszwecken in Salesforce protokollieren möchten, können Sie für jede Aktivität ein benutzerdefiniertes Feld erstellen. Jedes Feld muss einen bestimmten API-Namen (in Salesforce als „Feldname“ bezeichnet) verwenden.

* Feldname für Anrufergebnisse: motosales_call_result
* Feldname für Anrufgründe: motosales_call_reason

Um diese Felder zu verwenden, müssen Sie das Feld zunächst als benutzerdefiniertes Aktivitätsfeld erstellen. Um sie für Benutzer sichtbar zu machen, müssen Sie sie zum Aufgabenobjekt-Seiten-Layout hinzufügen.

## Salesforce Classic {#salesforce-classic}

### Benutzerdefiniertes Aktivitätsfeld in Salesforce Classic erstellen  {#create-custom-activity-field-in-salesforce-classic}

1. Klicken Sie in Salesforce auf **Setup**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Geben Sie „Aktivitäten“ in das Feld „Schnellsuche“ ein.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Klicken Sie auf **Aktivität Benutzerdefinierte Felder**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Klicken Sie auf **Neu**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Wählen Sie den Datentyp „Text“ und klicken Sie auf **Weiter**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Geben Sie dem benutzerdefinierten Feld den Feldnamen wie oben definiert. Die Feldlänge ist auf 255 Zeichen begrenzt. Die Feldbezeichnung ist das Feld, das für Ihr Vertriebsteam sichtbar ist, und kann an die Anforderungen Ihres Teams angepasst werden.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Die übrigen Einstellungen sind optional. Klicken Sie nach Abschluss der Konfiguration auf **Weiter**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Wählen Sie die gewünschten Sicherheitseinstellungen auf Feldebene für dieses Feld aus und klicken Sie auf **Weiter** (die Abbildung unten ist nur ein Beispiel).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass das benutzerdefinierte Feld für das Profil sichtbar ist, das Ihre Sales Connect-Benutzer verwenden, zusammen mit überall dort, wo es sichtbar sein soll.

1. Wählen Sie aus, welchen Seiten-Layouts das Feld hinzugefügt werden soll, und klicken Sie auf **Speichern** (optional können Sie auf **Speichern und neu** klicken und den Vorgang für das Feld Anrufgrund wiederholen).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Hinzufügen eines benutzerdefinierten Aktivitätsfelds zum Aufgabenseiten-Layout in Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Sie müssen diese Schritte nur ausführen, wenn Sie das gewünschte Seiten-Layout in Schritt 9 oben nicht ausgewählt haben.

1. Klicken Sie in Salesforce auf **Setup**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Geben Sie „Aufgabe“ in das Feld „Schnellsuche“ ein.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Klicken Sie **Aufgabenseiten-Layouts**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Klicken Sie **Bearbeiten** neben dem Aufgabenseiten-Layout, dem Sie dieses Feld hinzufügen möchten.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Ziehen Sie das Feld per Drag-and-Drop in den gewünschten Bereich des Aufgabenseiten-Layouts.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Benutzerdefiniertes Aktivitätsfeld in Salesforce Lightning erstellen {#create-custom-activity-field-in-salesforce-lightning}

1. Klicken Sie in Salesforce oben rechts auf das Zahnradsymbol und dann auf **Setup**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Klicken Sie auf **Objekt-Manager**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Geben Sie „Aktivität“ in das Feld „Schnellsuche“ ein.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Klicken Sie auf die **Aktivität** Bezeichnung.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Klicken Sie **Felder und Beziehungen**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Klicken Sie auf **Neu**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Benutzerdefiniertes Aktivitätsfeld zum Aufgabenseiten-Layout in Salesforce Lightning hinzufügen {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. Klicken Sie in Salesforce oben rechts auf das Zahnradsymbol und dann auf **Setup**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Klicken Sie auf **Objekt-Manager**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Geben Sie „Aufgabe“ in das Feld „Schnellsuche“ ein.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Klicken Sie auf die **Aufgabe** Bezeichnung.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Klicken Sie auf **Seiten-Layouts**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Klicken Sie auf das Aufgabenseiten-Layout, dem Sie dieses Feld hinzufügen möchten.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Ziehen Sie das Feld per Drag-and-Drop in den gewünschten Bereich des Aufgabenseiten-Layouts.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Installieren von Sales Connect-Ereignisfeldern im Aktivitätsverlauf](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
