---
unique-page-id: 11372975
description: Schritt 1 von 3 - Hinzufügen Marketo Fields to Salesforce (Professional) - Marketing Docs - Produktdokumentation
title: Schritt 1 von 3 - Hinzufügen Marketo Fields to Salesforce (Professional)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---


# Schritt 1 von 3: hinzufügen Marketo Fields to Salesforce (Professional) {#step-of-add-marketo-fields-to-salesforce-professional}

>[!NOTE]
>
>**Voraussetzungen**
>
>Ihre Salesforce-Instanz muss Zugriff auf die Salesforce-APIs haben, um Daten zwischen Marketo und Salesforce zu synchronisieren.

Marketo verwendet eine Reihe von Feldern, um bestimmte Arten von Marketinginformationen zu erfassen. Wenn Sie diese Daten in Salesforce haben möchten, befolgen Sie bitte die unten stehende Anleitung.

1. Erstellen Sie drei benutzerdefinierte Felder in Salesforce auf den Interessenten- und Kontaktobjekten: Ergebnis, Akquise-Programm und Akquise-Datum.
1. Ordnen Sie diese benutzerdefinierten Felder zwischen Interessenten und Kontakten zu, damit die Werte bei der Konvertierung in Salesforce übernommen werden.
1. Sie können bei Bedarf weitere Felder erstellen (siehe Tabelle unten).

Alle diese benutzerdefinierten Felder sind optional und müssen nicht synchronisiert werden. Als Best Practice empfehlen wir, Felder für Score, Akquise-Programm und Akquise-Datum zu erstellen.

## hinzufügen von Marketo-Feldern in Salesforce {#add-marketo-fields-to-salesforce}

hinzufügen drei benutzerdefinierte Felder auf den oben aufgeführten Interessenten- und Kontaktobjekten in Salesforce. Wenn Sie weitere hinzufügen möchten, sehen Sie sich die Tabelle der verfügbaren Felder am Ende dieses Abschnitts an.

Führen Sie die folgenden Schritte für jedes der drei benutzerdefinierten Felder aus, um sie hinzuzufügen. Beginn mit **Ergebnis**.

1. Melden Sie sich bei Salesforce an und klicken Sie auf **Setup.**

   ** ![](assets/image2016-5-23-13-3a15-3a21.png)

   **

1. Klicken Sie im Menü &quot;Erstellen&quot;auf der linken Seite auf **Anpassen** und wählen Sie **Interessenten**. Klicken Sie auf **Felder**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Klicken Sie unten auf der Seite im Abschnitt &quot;Benutzerdefinierte Felder und Beziehungen&quot;auf **Neu** .

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Wählen Sie den entsprechenden Feldtyp aus (für Ergebnis — **Nummer**; Akquise-Programm — **Text**; Akquise-Datum — **Datum/Uhrzeit**).

   ![](assets/choose-field-type-2-hand.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Geben Sie die Feldbeschriftung, -länge und -feldnamen für das Feld ein, wie in der folgenden Tabelle dargestellt.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Feldbeschriftung 
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
   <td>mkto71_Lead_Score</td> 
   <td>Nummer</td> 
   <td>Länge 10<br>Dezimalstellen 0 </td> 
  </tr> 
  <tr> 
   <td>Akquise-Datum</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>Datum/Uhrzeit</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Akquise-Programm</td> 
   <td>mkto71_Acquisition_Programm</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforce fügt den Feldnamen __c hinzu, wenn sie zum Erstellen von API-Namen verwendet werden.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>Text- und Zahlenfelder erfordern eine Länge, Datums-/Uhrzeitfelder jedoch nicht. Eine Beschreibung ist optional.

1. Klicken Sie auf **Weiter**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Legen Sie die Zugriffseinstellungen fest und klicken Sie auf **Weiter**:

   * Legen Sie alle Rollen auf **Sichtbar **und **Schreibgeschützt fest.**

   * Deaktivieren Sie das **Kontrollkästchen &quot;Schreibgeschützt** &quot;für das Profil des Synchronisierungsbenutzers:

      * Wenn Sie einen Benutzer haben, der das Profil eines *Systemadministrators* als Synchronisierungsbenutzer hat, deaktivieren Sie das Kontrollkästchen &quot; **Schreibgeschützt** &quot;für das Profil &quot;Systemadministrator&quot;(wie unten gezeigt).

      * Wenn Sie ein *benutzerdefiniertes Profil* für den Synchronisierungsbenutzer erstellt haben, deaktivieren Sie das Kontrollkästchen **Schreibgeschützt** für dieses benutzerdefinierte Profil

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Wählen Sie die Seitenlayouts aus, die das Feld anzeigen sollen.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Klicken Sie auf **Speichern &amp; Neu** , um zurückzukehren und jedes der beiden anderen benutzerdefinierten Felder zu erstellen. Klicken Sie auf **Speichern** , wenn Sie alle drei Schritte abgeschlossen haben.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Klicken Sie im Menü &quot;Erstellen&quot;auf der linken Seite auf **Anpassen **und wählen Sie **Kontakte**. Klicken Sie auf **Felder**.
1. Führen Sie die Schritte 3 bis 10 für die Felder &quot;Punktzahl&quot;, &quot;Akquise-Programm&quot;und &quot;Akquise-Objekt&quot;auf dem Kontaktobjekt aus, genau wie für das Lead-Objekt.
1. Optional können Sie das obige Verfahren für weitere benutzerdefinierte Felder aus dieser Tabelle verwenden.

<table> 
 <tbody> 
  <tr> 
   <th>Feldbeschriftung</th> 
   <th>Feldname</th> 
   <th>Datentyp</th> 
   <th>Feldattribute</th> 
  </tr> 
  <tr> 
   <td>Akquise-Programm-ID</td> 
   <td>mkto71_Acquisition_Programm_Id</td> 
   <td>Nummer</td> 
   <td>Länge 18<br>Dezimalstellen 0 </td> 
  </tr> 
  <tr> 
   <td>Ursprünglicher Werber</td> 
   <td>mkto71_Original_Werber</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Ursprüngliche Suchmaschine</td> 
   <td>mkto71_Original_Suchmaschine</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Ursprünglicher Suchbegriff</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Ursprüngliche Quellinformationen</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Originalquellentyp</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Inferated City</td> 
   <td>mkto71_Inferred_City</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Vorgestellte Firma</td> 
   <td>mkto71_Inferred_Firma</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Inferiertes Land</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Großraum</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Abgeleiteter Telefonbereichscode</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Postleitzahl</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
  <tr> 
   <td>Inferierte Staatsregion</td> 
   <td>mkto71_Inferred_state_Region</td> 
   <td>Text</td> 
   <td>Länge 255</td> 
  </tr> 
 </tbody> 
</table>

## Benutzerdefinierte Felder für Konvertierungen zuordnen  {#map-custom-fields-for-conversions}

Ein benutzerdefiniertes Feld auf dem Interessentenobjekt in Salesforce sollte einem Kontaktfeld auf dem Kontaktobjekt zugeordnet werden, damit Daten bei einer Konvertierung übertragen werden.

1. Klicken Sie in der oberen rechten Ecke auf Setup.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Geben Sie &quot;Felder&quot;in die Nav-Suche ein, ohne die Eingabetaste zu drücken. Felder werden unter verschiedenen Objekten angezeigt. Klicken Sie unter &quot;Interessenten&quot;auf Felder.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Wechseln Sie zum Abschnitt Lead Custom Fields &amp; Relationships und klicken Sie auf Map Lead Fields.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Klicken Sie auf die Dropdownliste neben dem Feld, das Sie zuordnen möchten.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Wählen Sie das entsprechende benutzerdefinierte Feld für den Kontakt aus.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Wiederholen Sie die oben genannten Schritte für alle anderen von Ihnen erstellten Felder.
1. Klicken Sie auf Speichern, wenn Sie fertig sind.

Einfach genug, nicht wahr?

>[!NOTE]
>
>**Tieftauchen**
>
>Hier ist ein [Video des gesamten Prozesses](https://nation.marketo.com/videos/1475) , der es kristallklar machen sollte!

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketing (Professional)](step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

>



