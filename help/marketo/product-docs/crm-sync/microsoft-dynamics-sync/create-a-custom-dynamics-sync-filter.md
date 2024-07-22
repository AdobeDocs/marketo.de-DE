---
unique-page-id: 9437903
description: Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics - Marketo Docs - Produktdokumentation
title: Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 1%

---

# Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics {#create-a-custom-dynamics-sync-filter}

Möchten Sie nicht alles in Ihrem Dynamics CRM mit Marketo Engage synchronisieren? Mach dir keine Sorgen! Mit Marketo können Sie einen Synchronisierungsfilter einrichten und nur einen Teil Ihrer Datensätze synchronisieren.

## Überblick {#overview}

So richten Sie einen Dynamics-Synchronisierungsfilter ein:

1. Erstellen Sie in Ihrem Dynamics CRM ein benutzerdefiniertes Feld mit dem Namen new_synctomkto (zwei Optionen (boolesch) für ein beliebiges Objekt (Lead, Kontakt, Konto, Gelegenheit und andere benutzerdefinierte Entitäten).
1. Weisen Sie diesem Feld einen Ja/Nein -Wert zu.

Sie müssen diese Änderungen in Dynamics CRM vornehmen, nicht in Ihrer Datenbank oder in Marketo.

>[!CAUTION]
>
>Wenn Sie das Feld nicht zuweisen und leer/NULL lassen, wird es zwar heruntersynchronisiert, aber nicht aktualisiert. Datensätze mit einem Feldwert leer/NULL in Dynamics CRM zeigen diesen Feldwert in Marketo als &quot;false&quot;.

Marketo sucht bei der automatischen Hintergrundsynchronisierung nach diesem Feld und bestimmt anhand dieser Logik, über welche Datensätze synchronisiert werden sollen:

| Feldwert | Mit Marketo synchronisieren? |
|---|---|
| Feld ist nicht vorhanden | Ja |
| Feld ist leer | Ja |
| Feld hat den Wert Ja | Ja |
| Feld hat den Wert Nein | Nein |

>[!CAUTION]
>
>Die einzige Möglichkeit, Marketo anzuweisen, einen Datensatz zu überspringen, besteht darin, den Feldwert explizit auf **Nein** festzulegen. Marketo synchronisiert Datensätze weiterhin, auch wenn die Feldwerte leer sind.

>[!PREREQUISITES]
>
>Installieren Sie die neueste Version des Marketo-Plug-ins (3.0.0.1 oder höher). Navigieren Sie zu Marketo > Admin > Microsoft Dynamics > Marketo-Lösung herunterladen .

## Erstellen des SyncToMkto-Felds {#create-synctomkto-field}

1. Melden Sie sich bei Ihrem Dynamics CRM an. Klicken Sie auf **Einstellungen** und dann auf **Anpassungen**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Klicken Sie auf **Anpassen des Systems**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Klicken Sie auf ![](assets/image2015-8-10-21-3a44-3a23.png) neben **Entitäten**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Klicken Sie auf ![](assets/image2015-8-10-21-3a44-3a23.png) neben **Lead** und wählen Sie **Felder** aus. Klicken Sie dann auf **Neu**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Geben Sie **SyncToMkto** in das Feld **Anzeigename** ein und wählen Sie **Zwei Optionen** als **Datentyp** aus. Klicken Sie dann auf **Speichern und schließen**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Wählen Sie einen beliebigen Anzeigenamen für dieses Feld aus, aber das Feld &quot;Name&quot;muss genau **new_synctomkto** sein. Sie müssen **new** als Standardpräfix verwenden. Wenn Sie die Standardeinstellung geändert haben, wechseln Sie hier zu [Zurücksetzen des Standardpräfixes für die benutzerdefinierten Feldnamen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Sie können sie nach der Erstellung der neuen Felder wieder ändern.

   >[!NOTE]
   >
   >Wenn Sie einen asynchronen Workflow eingerichtet haben, erhält der Datensatz den standardmäßigen SyncToMkto -Wert, den Sie im Feld eingerichtet haben, und erhält einige Sekunden später den korrekten Wert, wenn der Workflow abgeschlossen ist. Wenn der Standardwert auf Ja gesetzt ist, werden diese Datensätze in Marketo erstellt und dann veraltet. Verwenden Sie **Nein** als Standardwert, um dies zu vermeiden.

1. Wiederholen Sie diesen Vorgang und erstellen Sie das Feld **SyncToMkto** für alle anderen Entitäten, für die Sie die Synchronisierung einschränken möchten, z. B. Kontakte, Konten, Opportunities und benutzerdefinierte Entitäten.

## Filter in Marketo auswählen {#select-the-filter-in-marketo}

Auch wenn Sie die Erstsynchronisierung bereits durchgeführt haben, wählen Sie die zu synchronisierenden Felder aus.

1. Wechseln Sie zu Admin und wählen Sie **[!UICONTROL Microsoft Dynamics]** aus.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie in den Details zur Feldsynchronisierung auf **[!UICONTROL Bearbeiten]** .

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

1. Gehen Sie zu Ihrem Dynamics CRM. Klicken Sie auf **Einstellungen** und dann auf **Prozesse**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Klicken Sie auf **Neu**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Geben Sie einen Namen für den Workflow ein und wählen Sie **Workflow** als Kategorie und **Lead** als Entität aus. Klicken Sie dann auf **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Erstellen Sie Regeln, um dem Feld **SyncToMkto** je nach Präferenz Ihres Unternehmens den Wert &quot;true&quot;oder &quot;false&quot;zuzuweisen. Klicken Sie auf **Speichern und schließen**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Definieren Sie eine Standardaktion, nachdem Sie auf &quot;**Schritt hinzufügen**&quot;geklickt haben, um eine Prüfbedingung hinzuzufügen. Dadurch werden die Datensätze festgelegt, die Sie nicht mit **Nein** synchronisieren möchten. Andernfalls werden sie synchronisiert.

1. Wählen Sie den Workflow aus und klicken Sie auf **Aktivieren**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Siehe [Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} , um Regeln einzurichten, die nur Datensätze für Personen mit E-Mail-Adressen synchronisieren.

## Filterdetails synchronisieren {#sync-filter-details}

Im Folgenden finden Sie einige Implementierungsdetails, von denen wir dachten, dass Sie sie wissen sollten:

* Starten eines Synchronisierungsvorgangs

  Wenn sich der Wert **SyncToMkto** von **No** in **Yes** ändert, benachrichtigt Dynamics Marketo sofort, mit der Synchronisierung dieses Datensatzes zu beginnen. Wenn der Datensatz bereits vorhanden ist, aktualisiert Marketo ihn. Andernfalls erstellt Marketo den Datensatz.

  >[!TIP]
  >
  >In diesem Fall wird dem Marketo-Protokoll ein `Create [StartSync]` -Vorgang hinzugefügt.

* Synchronisierungsvorgang anhalten

  Wenn ein Datensatz seinen SyncToMkto-Wert von Ja in Nein ändert, wird Marketo benachrichtigt, die Synchronisierung dieses Datensatzes zu beenden. Der Datensatz wird jedoch nicht gelöscht, stattdessen werden keine Updates mehr abgerufen und veraltet.

>[!MORELIKETHIS]
>
>* [Synchronisierungsfilter für Microsoft Dynamics: Qualify](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Synchronisierungsfilter für Microsoft Dynamics: Zusammenführen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
