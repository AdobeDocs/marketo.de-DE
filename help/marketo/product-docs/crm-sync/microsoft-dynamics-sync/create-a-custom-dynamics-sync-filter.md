---
unique-page-id: 9437903
description: Erstellen eines benutzerspezifischen Dynamiksynchronisierungsfilters - Marketo Docs - Produktdokumentation
title: Erstellen eines benutzerspezifischen Synchronisierungsfilters
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---


# Erstellen eines benutzerspezifischen Synchronisierungsfilters {#create-a-custom-dynamics-sync-filter}

Möchten Sie nicht alles in Ihrem Dynamics CRM mit Marketo synchronisieren? Mach dir keine Sorgen! Mit Marketo können Sie einen Synchronisierungsfilter einrichten und nur einen Teil Ihrer Datensätze synchronisieren.

## Übersicht {#overview}

So richten Sie einen Dynamics-Synchronisierungsfilter ein:

1. Erstellen Sie ein benutzerdefiniertes Feld mit dem Namen new_synctomkto in Dynamics CRM für jedes Objekt (Lead, Kontakt, Konto, Gelegenheit und andere benutzerdefinierte Entitäten).
1. Weisen Sie diesem Feld den Wert &quot;Ja/Nein&quot;zu oder lassen Sie ihn leer.

>[!NOTE]
>
>Sie müssen diese Änderungen in Dynamics CRM vornehmen, nicht in Ihrer Datenbank oder in Marketo.

Marketo sucht bei der automatischen Hintergrundsynchronisierung nach diesem Feld und bestimmt anhand dieser Logik, über welche Datensätze synchronisiert werden soll:

| Feldwert | Mit Marketo synchronisieren? |
|---|---|
| Feld nicht vorhanden | Ja |
| Feld ist leer | Ja |
| Feld hat den Wert &quot;Ja&quot; | Ja |
| Feld hat den Wert &quot;Nein&quot; | Nein |

>[!CAUTION]
>
>Die einzige Möglichkeit, Marketo anzuweisen, einen Datensatz zu überspringen, besteht darin, den Feldwert explizit auf **Nein** festzulegen. Marketo synchronisiert weiterhin Datensätze, auch wenn die Feldwerte leer sind.

>[!NOTE]
>
>**Voraussetzungen**
>
>Installieren Sie die neueste Version des Marketo-Plug-ins (3.0.0.1 oder höher). Gehen Sie zu Marketing > Admin > Microsoft Dynamics > Marketing-Lösung herunterladen.

## SyncToMkto-Feld erstellen {#create-synctomkto-field}

1. Melden Sie sich bei Dynamics CRM an. Klicken Sie auf **Einstellungen** und dann auf **Anpassungen**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Klicken Sie auf System **anpassen**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Klicken Sie ![](assets/image2015-8-10-21-3a44-3a23.png) neben **Entitäten** auf .

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Klicken Sie ![](assets/image2015-8-10-21-3a44-3a23.png) neben **Interessent **und wählen Sie **Felder**. Klicken Sie dann auf **Neu**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Geben Sie **SyncToMkto** in das Feld **Anzeigename** ein und wählen Sie **zwei Optionen** als **Datentyp**. Klicken Sie dann auf **Speichern und Schließen**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Wählen Sie einen beliebigen Anzeigenamen für dieses Feld, aber das Feld Name muss genau **new_synctomkto** sein. Sie müssen **new** als Standardpräfix verwenden. Wenn Sie die Standardeinstellung geändert haben, [setzen Sie hier das Standardpräfix für die benutzerdefinierten Feldnamen](create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md)zurück. Sie können sie nach Erstellung der neuen Felder wieder ändern.

   >[!NOTE]
   >
   >Wenn Sie einen asynchronen Workflow eingerichtet haben, erhält der Datensatz den standardmäßigen SyncToMkto-Wert, den Sie im Feld eingerichtet haben, und ruft nach Abschluss der Ausführung des Workflows einige Sekunden den korrekten Wert ab. Wenn der Standardwert auf &quot;Ja&quot;festgelegt ist, werden diese Datensätze in Marketo erstellt und dann veraltet. Verwenden Sie **Nein** als Standardwert, um dies zu vermeiden.

1. Wiederholen Sie diesen Vorgang und erstellen Sie das **Feld SyncToMkto** für alle weiteren Entitäten, für die Sie die Synchronisierung einschränken möchten, z. B. Kontakt, Konto, Gelegenheit und benutzerdefinierte Entitäten.

## Filter in Markieren auswählen {#select-the-filter-in-marketo}

Auch wenn Sie Ihre erste Synchronisierung bereits durchgeführt haben, wählen Sie die Felder aus, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **MIcrosoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie unter &quot;Details zur Feldsynchronisierung&quot;auf **Bearbeiten** .

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Blättern Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomkto sein, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **Speichern**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Gut, jetzt haben Sie den Synchronisierungsfilter für Marketo aktiviert.

## Erstellen eines Arbeitsablaufs für Dynamiken zum automatischen Zuweisen von Synchronisierungsfilterwerten {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Sie können den SyncToMkto-Feldern für Ihre Datensätze immer manuell einen Wert zuweisen. Aber warum sollten Sie nicht die Leistungsfähigkeit eines Dynamics-Workflows nutzen und dem SyncToMkto-Feld automatisch einen Wert zuweisen, wenn ein Datensatz erstellt oder aktualisiert wird?

>[!NOTE]
>
>Dies ist auf Datenbankebene nicht möglich. Dies muss im CRM manuell oder mithilfe eines Workflows erfolgen.
>
>Ein Dynamics-Arbeitsablauf funktioniert nur bei neuen Datensätzen, die im Laufe der Zeit erstellt wurden, nicht bei historischen Daten. Verwenden Sie eine Batch-Aktualisierung, um über vorhandene Datensätze zu wechseln.

1. Gehen Sie zu Dynamics CRM. Klicken Sie auf **Einstellungen** und dann auf **Prozesse**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Geben Sie einen Namen für den Workflow ein und wählen Sie **Workflow** als Kategorie und **Interessent** als Entität. Klicken Sie dann auf **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Erstellen Sie Regeln, um dem Feld &quot; **SyncToMkto** &quot;je nach den Vorlieben Ihres Unternehmens einen Wert für &quot;true&quot;oder &quot;false&quot;zuzuweisen. Klicken Sie auf **Speichern und schließen**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Definieren Sie eine Standardaktion, nachdem Sie auf **Hinzufügen Schritt** klicken, um eine Prüfbedingung hinzuzufügen. Dadurch werden die Datensätze festgelegt, die nicht mit **Nein** synchronisiert werden sollen. Andernfalls werden sie synchronisiert.

1. Wählen Sie den Workflow aus und klicken Sie auf **Aktivieren**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Eine E-Mail-Adresse [finden Sie unter](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) Benutzerdefinierte Synchronisierungsfilterregeln, um Regeln einzurichten, mit denen nur Datensätze für Personen mit E-Mail-Adressen synchronisiert werden.

## Filterdetails synchronisieren {#sync-filter-details}

Im Folgenden finden Sie einige Implementierungsdetails, die wir dachten Sie sollten wissen:

1. Beginn eines Synchronisierungsvorgangs

   Wenn sich der **SyncToMkto** -Wert von **&quot;Nein** &quot;in &quot; **Ja**&quot;ändert, benachrichtigt Dynamics Marketo sofort, um diesen Datensatz zu synchronisieren. Wenn der Datensatz bereits vorhanden ist, wird er von Marketo aktualisiert. Andernfalls erstellt Marketo den Datensatz.

   >[!TIP]
   >
   >In diesem Fall wird dem MarketingTo-Protokoll ein Vorgang zum **Erstellen von [StartSync]** hinzugefügt.

1. Synchronisierungsvorgang beenden

   Wenn ein Datensatz seinen SyncToMkto-Wert von Yes in No ändert, wird Marketo benachrichtigt, diesen Datensatz nicht mehr zu synchronisieren. Der Datensatz wird jedoch nicht gelöscht, sondern es werden keine Updates mehr angezeigt.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Microsoft Dynamics Sync-Filter: Qualifizieren](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Microsoft Dynamics Sync-Filter: Zusammenführen](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [Benutzerdefinierte Sync-Filterregeln für eine E-Mail-Adresse](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

>



