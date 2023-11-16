---
unique-page-id: 9437903
description: Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics - Marketo Docs - Produktdokumentation
title: Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: a9aa55184a7971d3c82d106481f1f83593a7dd99
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics {#create-a-custom-dynamics-sync-filter}

Möchten Sie nicht alles in Ihrem Dynamics CRM mit Marketo synchronisieren? Mach dir keine Sorgen! Mit Marketo können Sie einen Synchronisierungsfilter einrichten und nur einen Teil Ihrer Datensätze synchronisieren.

## Überblick {#overview}

So richten Sie einen Dynamics-Synchronisierungsfilter ein:

1. Erstellen Sie in Ihrem Dynamics CRM ein benutzerdefiniertes Feld mit dem Namen new_synctomkto (zwei Optionen (boolesch) für ein beliebiges Objekt (Lead, Kontakt, Konto, Gelegenheit und andere benutzerdefinierte Entitäten).
1. Weisen Sie diesem Feld einen Ja/Nein -Wert zu.

Sie müssen diese Änderungen in Dynamics CRM vornehmen, nicht in Ihrer Datenbank oder in Marketo.

>[!CAUTION]
>
>Wenn Sie das Feld nicht zuweisen und leer/NULL lassen, wird es zwar heruntersynchronisiert, aber nicht aktualisiert.

Marketo sucht bei der automatischen Hintergrundsynchronisierung nach diesem Feld und bestimmt anhand dieser Logik, über welche Datensätze synchronisiert werden sollen:

| Feldwert | Mit Marketo synchronisieren? |
|---|---|
| Feld ist nicht vorhanden | Ja |
| Feld ist leer | Ja |
| Feld hat den Wert Ja | Ja |
| Feld hat den Wert Nein | Nein |

>[!CAUTION]
>
>Die einzige Möglichkeit, Marketo anzuweisen, einen Datensatz zu überspringen, besteht darin, den Feldwert explizit auf **Nein**. Marketo synchronisiert Datensätze weiterhin, auch wenn die Feldwerte leer sind.

>[!PREREQUISITES]
>
>Installieren Sie die neueste Version des Marketo-Plug-ins (3.0.0.1 oder höher). Navigieren Sie zu Marketo > Admin > Microsoft Dynamics > Marketo-Lösung herunterladen .

## Erstellen des SyncToMkto-Felds {#create-synctomkto-field}

1. Melden Sie sich bei Ihrem Dynamics CRM an. Klicks **Einstellungen** Klicken Sie auf **Anpassungen**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Klicks **System anpassen**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Klicks ![](assets/image2015-8-10-21-3a44-3a23.png) neben **Entitäten**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Klicks ![](assets/image2015-8-10-21-3a44-3a23.png) neben **Lead** und wählen **Felder**. Klicken Sie anschließend auf **Neu**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Eingabe **SyncToMkto** im **Anzeigename** Feld und wählen Sie **Zwei Optionen** als **Datentyp**. Klicken Sie anschließend auf **Speichern und schließen**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Wählen Sie einen beliebigen Anzeigenamen für dieses Feld aus, aber das Feld &quot;Name&quot;muss genau **new_synctomkto**. Sie müssen **new** als Standardpräfix. Wenn Sie die Standardeinstellung geändert haben, gehen Sie hier zu [Zurücksetzen des Standardpräfixes für die benutzerdefinierten Feldnamen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Sie können sie nach der Erstellung der neuen Felder wieder ändern.

   >[!NOTE]
   >
   >Wenn Sie einen asynchronen Workflow eingerichtet haben, erhält der Datensatz den standardmäßigen SyncToMkto -Wert, den Sie im Feld eingerichtet haben, und erhält einige Sekunden später den korrekten Wert, wenn der Workflow abgeschlossen ist. Wenn der Standardwert auf Ja gesetzt ist, werden diese Datensätze in Marketo erstellt und dann veraltet. Verwendung **Nein** als Standardwert verwenden, um dies zu vermeiden.

1. Wiederholen Sie diesen Vorgang und erstellen Sie die **SyncToMkto** für alle anderen Entitäten, für die Sie die Synchronisierung einschränken möchten, wie z. B. Kontakt, Konto, Opportunity und benutzerdefinierte Entitäten.

## Filter in Marketo auswählen {#select-the-filter-in-marketo}

Auch wenn Sie die Erstsynchronisierung bereits durchgeführt haben, wählen Sie die zu synchronisierenden Felder aus.

1. Navigieren Sie zu Admin und wählen Sie **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicks **[!UICONTROL Bearbeiten]** in den Details zur Feldsynchronisierung.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss &quot;new_synctomkto&quot;lauten, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Gut, jetzt haben Sie den Synchronisierungsfilter für Marketo aktiviert.

## Erstellen eines Dynamics-Workflows zum automatischen Zuweisen von Synchronisierungsfilterwerten {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Sie können den SyncToMkto-Feldern für Ihre Datensätze immer manuell einen Wert zuweisen. Warum sollten Sie jedoch nicht die Leistungsfähigkeit eines Dynamics-Workflows nutzen und dem Feld SyncToMkto automatisch einen Wert zuweisen, wenn ein Datensatz erstellt oder aktualisiert wird?

>[!NOTE]
>
>Dies ist auf Datenbankebene nicht möglich. Dies muss entweder manuell im CRM-System oder mithilfe eines Workflows erfolgen.
>
>Ein Dynamics-Workflow funktioniert nur mit neuen Datensätzen, die in Zukunft erstellt werden, nicht mit historischen Daten. Verwenden Sie eine Batch-Aktualisierung, um vorhandene Datensätze zu verschieben.

1. Gehen Sie zu Ihrem Dynamics CRM. Klicks **Einstellungen**, dann **Prozesse**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Klicks **Neu**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Geben Sie einen Namen für den Workflow ein und wählen Sie **Workflow** als Kategorie und **Lead** als Entität. Klicken Sie anschließend auf **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Erstellen Sie Regeln, um dem **SyncToMkto** -Feld auf Grundlage der Präferenz Ihres Unternehmens. Klicks **Speichern und schließen**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Definieren einer Standardaktion nach dem Klicken auf **Schritt hinzufügen** , um eine Prüfbedingung hinzuzufügen. Dadurch werden die Datensätze festgelegt, mit denen Sie nicht synchronisieren möchten **Nein**. Andernfalls werden sie synchronisiert.

1. Wählen Sie den Workflow aus und klicken Sie auf **Aktivieren**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Siehe [Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} , um Regeln einzurichten, die nur Datensätze für Personen mit E-Mail-Adressen synchronisieren.

## Filterdetails synchronisieren {#sync-filter-details}

Im Folgenden finden Sie einige Implementierungsdetails, von denen wir dachten, dass Sie sie wissen sollten:

* Starten eines Synchronisierungsvorgangs

  Wenn die Variable **SyncToMkto** Werteänderungen aus **Nein** nach **Ja**, benachrichtigt Dynamics Marketo sofort, um mit der Synchronisierung dieses Datensatzes zu beginnen. Wenn der Datensatz bereits vorhanden ist, aktualisiert Marketo ihn. Andernfalls erstellt Marketo den Datensatz.

  >[!TIP]
  >
  >A `Create [StartSync]` wird dem Marketo-Protokoll in diesem Fall hinzugefügt.

* Synchronisierungsvorgang anhalten

  Wenn ein Datensatz seinen SyncToMkto-Wert von Ja in Nein ändert, wird Marketo benachrichtigt, die Synchronisierung dieses Datensatzes zu beenden. Der Datensatz wird jedoch nicht gelöscht, stattdessen werden keine Updates mehr abgerufen und veraltet.

>[!MORELIKETHIS]
>
>* [Synchronisierungsfilter für Microsoft Dynamics: Qualifizieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Microsoft Dynamics Sync-Filter: Zusammenführen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
