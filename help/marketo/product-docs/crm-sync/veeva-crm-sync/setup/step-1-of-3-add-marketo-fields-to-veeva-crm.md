---
description: 'Schritt 1 von 3: Hinzufügen von Marketo-Feldern zum VEC CRM - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 1 von 3: Hinzufügen von Marketo-Feldern zum VEC CRM'
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 7%

---

# Schritt 1 von 3: Hinzufügen von Marketo-Feldern zum VEC CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>Ihre VEE-CRM-Instanz muss Zugriff auf Salesforce-APIs haben, um Daten zwischen Marketo Engage und VEeva CRM zu synchronisieren.

Marketo Engage verwendet eine Reihe von Feldern, um bestimmte Arten von Marketinginformationen zu erfassen. Wenn Sie diese Daten im Vevar CRM wünschen, folgen Sie bitte den unten stehenden Anweisungen.

`1.` Erstellen Sie ein benutzerdefiniertes Feld in VEE CRM für die Kontaktobjekte: Punktzahl

`2.` Sie können bei Bedarf zusätzliche Felder erstellen (siehe Tabelle unten).

Alle diese benutzerdefinierten Felder sind optional und müssen nicht mit Marketo Engage und VEE CRM synchronisiert werden.

## Hinzufügen von Marketo-Feldern zum VEC-CRM {#add-marketo-fields-to-veeva-crm}

Fügen Sie ein benutzerdefiniertes Feld zu den Lead- und Kontaktobjekten im oben aufgelisteten Vevar CRM hinzu. Weitere Informationen finden Sie in der Tabelle der verfügbaren Felder am Ende dieses Abschnitts.

Führen Sie die folgenden Schritte aus, um das Feld Punktzahl hinzuzufügen.

1. Melden Sie sich beim VEA-CRM an und klicken Sie auf **[!UICONTROL Einrichten]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Klicken Sie auf **[!UICONTROL Objekte und Felder]** und wählen Sie **[!UICONTROL Objektmanager]** aus.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Suchen Sie in der Suchleiste nach &quot;Kontakt&quot;.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Klicken Sie auf das Objekt **[!UICONTROL Kontakt]** .

1. Wählen Sie **[!UICONTROL Felder und Beziehungen]** aus.

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Wählen Sie den entsprechenden Feldtyp aus (für Punktzahl - Zahl).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Geben Sie die **[!UICONTROL Feldbezeichnung]**, die **[!UICONTROL Länge]** und den **[!UICONTROL Feldnamen]** für das Feld ein, wie in der folgenden Tabelle dargestellt.

<table>
 <tbody>
  <tr>
   <th>Feldbezeichnung
   <th>Feldname
   <th>Datentyp
   <th>Feldattribute
  </tr>
  <tr>
   <td>Bewertung</td>
   <td>mkto71_Lead_Score</td>
   <td>Zahl</td>
   <td>Länge 10<br/>
Dezimalstellen 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Veeva CRM hängt __c an Feldnamen an, wenn diese zum Erstellen von API-Namen verwendet werden.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Text- und Zahlenfelder erfordern eine Länge, Datums-/Uhrzeitfelder jedoch nicht. Eine Beschreibung ist optional.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Geben Sie die Zugriffseinstellungen an und klicken Sie auf **[!UICONTROL Weiter]**.

1. Setzen Sie alle Rollen auf &quot;Sichtbar&quot;und &quot;Schreibgeschützt&quot;.

1. Deaktivieren Sie das Kontrollkästchen Schreibgeschützt für das Profil Ihres Synchronisierungsbenutzers:

* Wenn Sie einen Benutzer mit dem Profil eines Systemadministrators als Synchronisierungsbenutzer haben, deaktivieren Sie das Kontrollkästchen Schreibgeschützt für das Profil &quot;Systemadministrator&quot;(wie unten dargestellt).
* Wenn Sie ein benutzerdefiniertes Profil für den Synchronisierungsbenutzer erstellt haben, deaktivieren Sie das Kontrollkästchen Schreibgeschützt für dieses benutzerdefinierte Profil.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Wählen Sie die Seitenlayouts aus, die das Feld anzeigen sollen.

1. Klicken Sie auf **[!UICONTROL Speichern und Neu]** , um zurück zu gehen und die beiden anderen benutzerdefinierten Felder zu erstellen.

1. Klicken Sie auf **[!UICONTROL Speichern]** , wenn Sie mit allen drei Schritten fertig sind.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Durch Hinzufügen des Felds zum Kontaktobjekt werden sie auch zum Objekt &quot;Personenkonto&quot;hinzugefügt.

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
   <td>mkto71_intenred_country</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgeleiteter Stadtbereich</td>
   <td>mkto71_inferred_Metropolitan_Area</td>
   <td>Text</td>
   <td>Länge 255</td>
  </tr>
  <tr>
   <td>Abgleitete Vorwahl</td>
   <td>mkto71_inferred_Phone_Area_Code</td>
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
>Die Werte in den von Marketo automatisch zugewiesenen Feldern sind nicht sofort im VEE-CRM verfügbar, wenn das neue Feld erstellt wurde. Marketo synchronisiert die Daten nach der nächsten Aktualisierung des Datensatzes auf beiden Systemen mit dem VEE-CRM (d. h. bei Aktualisierung auf eines der Felder, die zwischen Marketo und VEE CRM synchronisiert werden).
