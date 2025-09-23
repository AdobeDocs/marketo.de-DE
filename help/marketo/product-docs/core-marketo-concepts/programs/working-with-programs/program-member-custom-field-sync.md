---
description: Benutzerdefinierte Feldsynchronisierung für Programmteilnehmer - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren benutzerdefinierter Felder für Programmmitglieder
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 12%

---

# Synchronisieren benutzerdefinierter Felder für Programmmitglieder {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Erstellung [ benutzerdefinierten Felder für Programmteilnehmer](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Synchronisieren einer  [!DNL Salesforce]  mit einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>Das Objekt Programmteilnehmer kann bis zu 20 benutzerdefinierte Felder enthalten. Diese Felder stehen jedem Programm zur Verfügung.

## Zuordnen von Salesforce-Feldern zu benutzerdefinierten Feldern für Programmteilnehmer {#map-salesforce-fields-to-program-member-custom-fields}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Klicken Sie auf **[!DNL Salesforce]** und dann auf **[!UICONTROL Bearbeiten]** neben „Programmteilnehmer - Benutzerdefiniertes Feld synchronisieren“.

   ![](assets/program-member-custom-field-sync-2.png)

1. Verwenden Sie das Suchfeld, um die [!DNL Salesforce] Felder zu finden, die Sie zuordnen möchten. In diesem Beispiel verwenden wir „Nicht aufrufen“.

   ![](assets/program-member-custom-field-sync-3.png)

1. Klicken Sie auf die Dropdown-Liste.

   ![](assets/program-member-custom-field-sync-4.png)

1. Wählen Sie das gewünschte Marketo-[!UICONTROL Benutzerdefiniertes Feld für Programmteilnehmer] für die Zuordnung aus.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >In der Dropdown-Liste werden nur [!UICONTROL Benutzerdefinierte Felder für Programmmitglieder] angezeigt, die dem Datentyp des [!DNL Salesforce]-Felds entsprechen.

1. Deaktivieren Sie für zusätzliche Feldzuordnungen das Suchfeld und wiederholen Sie die Schritte 3 bis 5.

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >Änderungen an den Programmmitgliedsdaten in den zugeordneten Feldern werden zwischen Marketo und [!DNL Salesforce] synchronisiert.

   >[!NOTE]
   >
   >Wenn Sie den Datentyp eines Felds in [!DNL Salesforce] umbenennen oder ändern, werden alle Zuordnungen dieses Felds zum benutzerdefinierten Feld [!UICONTROL Programmteilnehmer“ &#x200B;]. Sie können sie jedoch nach der Überprüfung dem neuen Feld zuordnen.

## Zuordnung von Salesforce-Feldern zu benutzerdefinierten Programmteilnehmerfeldern aufheben {#unmap-salesforce-fields-from-program-member-custom-fields}

Wenn Sie ein Feld freigeben möchten, um es zu ersetzen, oder nur eine allgemeine Änderung vornehmen möchten, müssen Sie zuerst eine Aufhebung der Zuordnung durchführen. Und so geht das.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Klicken Sie auf **[!DNL Salesforce]** und dann auf **[!UICONTROL Bearbeiten]** neben „Programmteilnehmer - Benutzerdefiniertes Feld synchronisieren“.

   ![](assets/program-member-custom-field-sync-8.png)

1. Verwenden Sie das Suchfeld, um die Felder zu suchen, deren Zuordnung Sie aufheben möchten. In diesem Beispiel verwenden wir „Nicht aufrufen“.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >Sie können das Kontrollkästchen **[!UICONTROL Zugeordnet]** aktivieren, um nur zugeordnete Felder anzuzeigen.

1. Heben Sie die Zuordnung auf, indem Sie auf **X** neben dem Feld klicken.

   ![](assets/program-member-custom-field-sync-10.png)

1. Die Zuordnung wird jetzt entfernt. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/program-member-custom-field-sync-11.png)

## Datentypzuordnung {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>SFDC-Datentyp</th>
      <th>Datentyp des benutzerdefinierten Feldes des Programmmitglieds</th>
    </tr>
    <tr>
      <td>Text</td>
      <td>String</td>
    </tr>
    <tr>
      <td>Auswahlliste</td>
      <td>String</td>
    </tr>
    <tr>
      <td>Auswahlliste mit Mehrfachauswahl</td>
      <td>String</td>
    </tr>
    <tr>
      <td>Telefon</td>
      <td>String</td>
    </tr>
    <tr>
      <td>E-Mail</td>
      <td>String</td>
    </tr>
    <tr>
      <td>Zahl(m)</td>
      <td>Ganzzahl</td>
    </tr>
    <tr>
      <td>Zahl (m,n)</td>
      <td>Gleitkomma</td>
    </tr>
    <tr>
      <td>Kontrollkästchen</td>
      <td>Boolesch</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>Datum</td>
      <td>Datum</td>
    </tr>
    <tr>
      <td>Datum/Uhrzeit</td>
      <td>Datum/Uhrzeit</td>
    </tr>
    <tr>
      <td>Lookup (Referenz)</td>
      <td>String</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>String</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [Ändern der Daten von Programmmitgliedern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [Zeigen Sie Daten im Raster „Programmteilnehmer“ an](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [SFDC-Synchronisierung - Kampagnensynchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
