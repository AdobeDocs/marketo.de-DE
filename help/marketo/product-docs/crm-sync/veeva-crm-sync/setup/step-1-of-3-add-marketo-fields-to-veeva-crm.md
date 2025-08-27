---
description: 'Schritt 1 von 3: Hinzufügen von Marketo-Feldern  [!DNL Veeva]  CRM - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 1 von 3: Marketo-Felder zu  [!DNL Veeva]  hinzufügen'
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# Schritt 1 von 3: Marketo-Felder zu [!DNL Veeva] CRM hinzufügen {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>Ihre [!DNL Veeva] CRM-Instanz muss Zugriff auf Salesforce-APIs haben, um Daten zwischen Marketo Engage und [!DNL Veeva] CRM zu synchronisieren.

Marketo Engage verwendet einen Satz von Feldern, um bestimmte Arten von Marketing-bezogenen Informationen zu erfassen. Wenn Sie diese Daten in [!DNL Veeva] CRM benötigen, befolgen Sie bitte die folgenden Anweisungen.

1. Benutzerdefiniertes Feld in [!DNL Veeva] CRM für Kontaktobjekte erstellen: Score
1. Sie können bei Bedarf zusätzliche Felder erstellen (siehe Tabelle unten).

Alle diese benutzerdefinierten Felder sind optional und müssen nicht zur Synchronisierung von Marketo Engage und [!DNL Veeva] CRM verwendet werden.

## Marketo-Felder zu [!DNL Veeva] CRM hinzufügen {#add-marketo-fields-to-veeva-crm}

Fügen Sie ein benutzerdefiniertes Feld für die Lead- und Kontaktobjekte in [!DNL Veeva] oben aufgeführten CRM hinzu. Weitere Informationen finden Sie in der Tabelle mit den verfügbaren Feldern am Ende dieses Abschnitts.

Führen Sie die folgenden Schritte für das Feld Score aus, um es hinzuzufügen.

1. Melden Sie sich beim [!DNL Veeva] CRM an und klicken Sie auf **[!UICONTROL Setup]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Klicken Sie auf **[!UICONTROL Objekte und Felder]** und wählen Sie **[!UICONTROL Objekt-Manager]**.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Suchen Sie in der Suchleiste nach „Kontakt“.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Klicken Sie auf das **[!UICONTROL Kontakt]**-Objekt.

1. Wählen Sie **[!UICONTROL Felder und Beziehungen]** aus.

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Wählen Sie den entsprechenden Feldtyp aus (für Bewertung - Zahl).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Geben Sie **[!UICONTROL Feldbezeichnung]**, **[!UICONTROL Länge]** und **[!UICONTROL Feldname]** für das Feld ein, wie in der folgenden Tabelle dargestellt.

<table>
 <tbody>
  <tr>
   <th>Feldbezeichnung
   <th>Feldname
   <th>Datentyp
   <th>Feldattribute
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td>mkto71_lead_score</td>
   <td>Zahl</td>
   <td>Länge 10<br/>
Dezimalstellen 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>[!DNL Veeva] CRM hängt __c an Feldnamen an, wenn es sie zum Erstellen von API-Namen verwendet.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Text- und Zahlenfelder erfordern eine Länge, Datums-/Uhrzeitfelder jedoch nicht. Eine Beschreibung ist optional.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Legen Sie die Zugriffseinstellungen fest und klicken Sie auf **[!UICONTROL Weiter]**.

1. Legen Sie alle Rollen auf **[!UICONTROL Sichtbar]** und **[!UICONTROL Schreibgeschützt]** fest.

1. Deaktivieren Sie das **[!UICONTROL Schreibgeschützt]** für das Profil Ihres Synchronisierungsbenutzers:

* Wenn Sie einen Benutzer mit dem Profil eines Systemadministrators als Synchronisierungsbenutzer haben, deaktivieren [!UICONTROL &#x200B; das Kontrollkästchen „Schreibgeschützt] für das Systemadministratorprofil (wie unten dargestellt).
* Wenn Sie ein benutzerdefiniertes Profil für den Synchronisierungsbenutzer erstellt haben, deaktivieren [!UICONTROL &#x200B; das Kontrollkästchen „Schreibgeschützt] für dieses benutzerdefinierte Profil.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Wählen Sie die Seiten-Layouts aus, in denen das Feld angezeigt werden soll.

1. Klicken Sie **[!UICONTROL Speichern und neu]**, um zurückzugehen und jedes der beiden anderen benutzerdefinierten Felder zu erstellen.

1. Klicken Sie **[!UICONTROL Speichern]** wenn Sie alle drei abgeschlossen haben.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Durch das Hinzufügen des Felds zum Kontaktobjekt werden sie auch zum Objekt Personenkonto hinzugefügt.

OPTIONAL: Verwenden Sie das obige Verfahren für alle zusätzlichen benutzerdefinierten Felder aus der folgenden Tabelle.

<table>
 <tbody>
  <tr>
   <th>Feldbezeichnung
   <th>Feldname
   <th>Datentyp
   <th>Feldattribute
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
>Werte in Feldern, die von Marketo automatisch zugewiesen werden, stehen nach der Erstellung [!DNL Veeva] neuen Felds nicht sofort im CRM zur Verfügung. Marketo synchronisiert die Daten mit [!DNL Veeva] CRM, sobald der Datensatz auf einem der Systeme das nächste Mal aktualisiert wird (d. h. eine Aktualisierung eines der Felder, die zwischen Marketo und [!DNL Veeva] CRM synchronisiert werden).
