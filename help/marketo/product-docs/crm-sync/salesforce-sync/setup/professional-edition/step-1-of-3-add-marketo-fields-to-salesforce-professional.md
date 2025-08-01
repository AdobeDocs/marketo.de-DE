---
unique-page-id: 11372975
description: Schritt 1 von 3 - Marketo-Felder zu Salesforce hinzufügen (Professional) - Marketo-Dokumente - Produktdokumentation
title: Schritt 1 von 3 - Marketo-Felder zu Salesforce hinzufügen (Professional)
exl-id: 1b52825e-201d-4b55-8edf-444b1653d591
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 9%

---

# Schritt 1 von 3: Marketo-Felder zu [!DNL Salesforce] hinzufügen (Professional) {#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>Ihre Salesforce-Instanz muss Zugriff auf Salesforce-APIs haben, um Daten zwischen Marketo Engage und Salesforce zu synchronisieren.

Marketo verwendet einen Satz von Feldern, um bestimmte Arten von Marketing-bezogenen Informationen zu erfassen. Wenn Sie diese Daten in [!DNL Salesforce] benötigen, befolgen Sie bitte die folgenden Anweisungen.

1. Erstellen Sie drei benutzerdefinierte Felder in [!DNL Salesforce] für die Lead- und Kontaktobjekte: Bewertung, Akquiseprogramm und Akquisedatum.
1. Ordnen Sie diese benutzerdefinierten Felder den Leads und Kontakten zu, sodass bei der Konvertierung in [!DNL Salesforce] die Werte übernommen werden.
1. Sie können bei Bedarf weitere Felder erstellen (siehe Tabelle unten).

Alle diese benutzerdefinierten Felder sind optional und müssen nicht zum Synchronisieren von Marketo und [!DNL Salesforce] verwendet werden. Als Best Practice empfehlen wir, Felder für Score, Akquise-Programm und Akquise-Datum zu erstellen.

## Marketo-Felder zu [!DNL Salesforce] hinzufügen {#add-marketo-fields-to-salesforce}

Fügen Sie drei benutzerdefinierte Felder zu den Lead- und Kontaktobjekten in den oben aufgeführten [!DNL Salesforce] hinzu. Weitere Informationen finden Sie in der Tabelle mit den verfügbaren Feldern am Ende dieses Abschnitts.

Führen Sie die folgenden Schritte für jedes der drei benutzerdefinierten Felder aus, um sie hinzuzufügen. Beginnen Sie mit **[!UICONTROL Score]**.

1. Melden Sie sich bei Salesforce an und klicken Sie auf **[!UICONTROL Setup]**.

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. Klicken Sie im Menü Erstellen auf der linken Seite auf **[!UICONTROL Anpassen]** und wählen Sie **[!UICONTROL Leads]**. Klicken Sie auf **[!UICONTROL Felder]**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Klicken **[!UICONTROL im]** „Benutzerdefinierte Felder und Beziehungen“ unten auf der Seite auf „Neu“.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Wählen Sie den entsprechenden Feldtyp aus (für Score **[!UICONTROL Zahl]**; Akquise-Programm **[!UICONTROL Text]**; Akquise-Datum **Datum/Uhrzeit**).

   ![](assets/choose-field-type-2-hand.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Geben Sie [!UICONTROL Feldbezeichnung], [!UICONTROL Länge] und [!UICONTROL Feldname] für das Feld ein, wie in der folgenden Tabelle dargestellt.

<table>
 <thead>
  <tr>
   <th>
    <div>
      Feldbezeichnung
    </div></th>
   <th>
    <div>
      Feldname
    </div></th>
   <th>
    <div>
      Datentyp
    </div></th>
   <th>
    <div>
      Feldattribute
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Ergebnis</td>
   <td>mkto71_lead_score</td>
   <td>Zahl</td>
   <td>Länge 10<br>Dezimalstellen 0 </td>
  </tr>
  <tr>
   <td>Akquisitionsdatum</td>
   <td>mkto71_Acquisition_Date</td>
   <td>Datum/Uhrzeit</td>
   <td> </td>
  </tr>
  <tr>
   <td>Akquirierungsprogramm</td>
   <td>mkto71_Acquisition_Program</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Salesforce] hängt __c an Feldnamen an, wenn es sie zum Erstellen von API-Namen verwendet.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>Text- und Zahlenfelder erfordern eine Länge, Datums-/Uhrzeitfelder jedoch nicht. Eine Beschreibung ist optional.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Legen Sie die Zugriffseinstellungen fest und klicken Sie auf **[!UICONTROL Weiter]**:

   * Legen Sie alle Rollen auf **[!UICONTROL Sichtbar]** und **[!UICONTROL Schreibgeschützt]**

   * Deaktivieren Sie das **[!UICONTROL Schreibgeschützt]** für das Profil Ihres Synchronisierungsbenutzers:

      * Wenn Sie als Synchronisierungsbenutzer das Profil eines _Systemadministrators_ verwenden, deaktivieren Sie das Kontrollkästchen **[!UICONTROL Schreibgeschützt]** für das Systemadministratorprofil (wie unten dargestellt)

      * Wenn Sie ein _benutzerdefiniertes Profil_ für den Synchronisierungsbenutzer erstellt haben, deaktivieren Sie das **[!UICONTROL Schreibgeschützt]**-Kontrollkästchen für dieses benutzerdefinierte Profil

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Wählen Sie die Seiten-Layouts aus, in denen das Feld angezeigt werden soll.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Klicken Sie **[!UICONTROL Speichern und neu]**, um zurückzugehen und jedes der beiden anderen benutzerdefinierten Felder zu erstellen. Klicken Sie **[!UICONTROL Speichern]**, wenn Sie alle drei abgeschlossen haben.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Klicken Sie im Menü Erstellen auf der linken Seite auf **[!UICONTROL Anpassen]** und wählen Sie **[!UICONTROL Kontakte]**. Klicken Sie auf **[!UICONTROL Felder]**.
1. Führen Sie die Schritte 3 bis 10 für die Felder Score, Akquisitionsdatum und Akquise-Programm im Kontaktobjekt aus, genau wie Sie es für das Lead-Objekt getan haben.
1. Optional können Sie das obige Verfahren für alle zusätzlichen benutzerdefinierten Felder aus dieser Tabelle verwenden.

<table>
 <tbody>
  <tr>
   <th>Feldbezeichnung</th>
   <th>Feldname</th>
   <th>Datentyp</th>
   <th>Feldattribute</th>
  </tr>
  <tr>
   <td>Akquisitionsprogramm-ID</td>
   <td>mkto71_Acquisition_Program_Id</td>
   <td>Zahl</td>
   <td>Länge 18<br>Dezimalstellen 0 </td>
  </tr>
  <tr>
   <td>Ursprünglicher Verweis</td>
   <td>mkto71_Original_Referrer</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Ursprüngliche Such-Engine</td>
   <td>mkto71_original_search_engine</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Ursprünglicher Suchausdruck</td>
   <td>mkto71_Original_Search_Phrase</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Ursprüngliche Quelleninfo</td>
   <td>mkto71_Original_Source_Info</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Ursprünglicher Quellentyp</td>
   <td>mkto71_original_Source_type</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleiteter Ort</td>
   <td>mkto71_inferred_city</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleitetes Unternehmen</td>
   <td>mkto71_inferred_company</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleitetes Land</td>
   <td>mkto71_inferred_country</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleiteter Stadtbereich</td>
   <td>mkto71_inferred_metropolitan_area</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgleitete Vorwahl</td>
   <td>mkto71_inferred_phone_area_code</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleitete Postleitzahl</td>
   <td>mkto71_inferred_postal_code</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleitetes Bundesland/abgeleitete Region</td>
   <td>mkto71_inferred_state_region</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Werte in Feldern, die von Marketo automatisch zugewiesen werden, stehen nach der Erstellung des neuen Felds in [!DNL Salesforce] nicht sofort zur Verfügung. Marketo synchronisiert die Daten mit [!DNL Salesforce] bei der nächsten Aktualisierung des Datensatzes auf einem der Systeme (d. h. eine Aktualisierung eines der Felder, die zwischen Marketo und [!DNL Salesforce] synchronisiert werden).

## Zuordnen benutzerdefinierter Felder für Konversionen  {#map-custom-fields-for-conversions}

Ein benutzerdefiniertes Feld auf dem Lead-Objekt in [!DNL Salesforce] sollte einem Kontaktfeld auf dem Kontaktobjekt zugeordnet werden, damit die Daten übertragen werden, wenn eine Konversion stattfindet.

1. Klicken Sie oben rechts auf **[!UICONTROL Setup]**.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Geben Sie &quot;[!UICONTROL fields] in die Nav-Suche ein, ohne die Eingabetaste zu drücken. Felder werden unter verschiedenen Objekten angezeigt. Klicken Sie **[!UICONTROL Felder]** unter Leads.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Gehen Sie zum Abschnitt „Benutzerdefinierte Lead-Felder und Beziehungen“ und klicken Sie auf **[!UICONTROL Lead-Felder zuordnen]**.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Klicken Sie auf die Dropdown-Liste neben dem Feld, das Sie zuordnen möchten.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Wählen Sie das entsprechende benutzerdefinierte Feld Kontakt aus.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Wiederholen Sie die obigen Schritte für alle anderen Felder, die Sie erstellt haben.
1. Klicken **[!UICONTROL abschließend]** Speichern“.

Ganz einfach, oder?

>[!MORELIKETHIS]
>
>[Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}
