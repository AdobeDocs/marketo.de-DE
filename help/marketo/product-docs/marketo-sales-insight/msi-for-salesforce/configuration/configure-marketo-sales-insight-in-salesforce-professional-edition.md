---
unique-page-id: 3571743
description: Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition - Marketo Docs - Produktdokumentation
title: Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: c85f544f2c06a2f5bb92d6e7cad5f801e73fdaed
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 4%

---

# Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Im Folgenden finden Sie die Schritte, die Sie zur Konfiguration von Marketo Sales Insight in Salesforce Professional Edition durchführen müssen. Los geht’s.

>[!PREREQUISITES]
>
>* Installieren Sie Marketo in Ihrer Salesforce Professional Edition.
>
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Konfigurieren von Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Öffnen Sie ein neues Browserfenster, um die Marketo Sales Insight-Anmeldedaten von Ihrem Marketo-Konto abzurufen.
1. Navigieren Sie zum Admin-Bereich und wählen Sie **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Klicks **API-Konfiguration bearbeiten**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Geben Sie einen geheimen API-Schlüssel Ihrer Wahl ein und klicken Sie auf **Speichern**. Verwenden Sie KEIN kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Ihr API-Geheimschlüssel ist wie ein Kennwort für Ihre Organisation und sollte sicher sein.

1. Klicks **Ansicht** im Bedienfeld Rest-API-Konfiguration , um die Anmeldeinformationen zu füllen.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Es wird ein Bestätigungs-Popup angezeigt. Klicks **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Sales Insight in Salesforce konfigurieren {#configure-sales-insight-in-salesforce}

1. Klicken Sie in Salesforce auf **Einrichtung**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und wählen Sie **Remote Site Settings**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Klicks **Neue Remote-Site**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoSoapAPI&quot;). Geben Sie die Remote-Site-URL ein, die Ihre Marketo-Host-URL im Bedienfeld Soap-API-Konfiguration in Marketo ist. Klicks **Speichern**. Sie haben jetzt Remote-Site-Einstellungen für die Soap-API erstellt.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Klicks **Neue Remote-Site** erneut.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoRestAPI&quot;). Geben Sie die Remote-Site-URL ein, die Ihre API-URL aus dem Bedienfeld REST-API-Konfiguration in Marketo ist. Klicks **Speichern**. Sie haben jetzt Remote-Site-Einstellungen für die Rest-API erstellt.

## Einrichten von Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Melden Sie sich bei Ihrer Marketo-Instanz an und klicken Sie auf **Admin**.

   ![](assets/login-admin-1.png)

1. Klicks **Sales Insight**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Klicks **API-Konfiguration bearbeiten**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Geben Sie eine **API-Geheimschlüssel** und klicken **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Lassen Sie dieses Fenster geöffnet. Sie werden diese Informationen später in Salesforce benötigen.

1. Gehen Sie zurück zu Salesforce , klicken Sie auf **Einrichtung**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und klicken Sie auf **Remote Site-Einstellung** under **Sicherheitskontrollen**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Klicks **Neue Remote-Site**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Eingabe **Remote Site Name** und **Remote Site URL** Klicken Sie auf **Speichern**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Sie wählen Ihre **Remote Site Name** (MarketoAPI wird hier verwendet). Die **Remote Site URL** finden Sie im Feld Marketo-Host im Dialogfeld API-Konfiguration bearbeiten in Schritt 4.

## Gewähren von Sales Insight-Benutzerprofilzugriff auf Standard-Salesforce-Objekte {#grant-sales-insight-users-profile-access}

Aufgrund der Verbesserungen der Saleforce-Sicherheit können App Exchange-Pakete keine Berechtigung mehr für Standardobjekte erteilen. Der Zugriff muss den relevanten Salesforce-Objekten aus dem Profil des Salesforce-Benutzers gewährt werden. Gehen Sie wie folgt vor, um die erforderlichen Berechtigungen zu gewähren.

1. Klicks **Einrichtung**.

1. Suchen Sie &quot;Profile&quot; in Schnellsuche.

1. Klicks **Bearbeiten** neben dem Profil, das Ihre Salesforce-Benutzer verwenden.

1. Aktivieren Sie im Bereich &quot;Standardobjektberechtigungen&quot;Lesezugriff für die folgenden Objekte: Lead, Kontakt, Konto und Chancen.

1. Klicks **Speichern**.

## Seitenlayouts anpassen {#customize-page-layouts}

1. Klicks **Einrichtung**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie nach &quot;Seitenlayout&quot;und wählen Sie die **Seitenlayout** under **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Klicks **Visualforce-Seiten** auf der linken Seite. Ziehen **Abschnitt** zum Layout unter dem Abschnitt &quot;Benutzerspezifische Links&quot;.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Geben Sie &quot;Marketo Sales Insight&quot;als **Bereichsname**. Auswählen **1-Spalte** und klicken **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Drag &amp; Drop **Lead** in den neuen Abschnitt ein.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Der Name dieses Felds ändert sich je nach Objekttyp. Wenn Sie beispielsweise das Seitenlayout für Kontakte ändern, wird &quot;Kontakt&quot;angezeigt.

1. Doppelklicken Sie auf die **Lead** -Block, den Sie gerade hinzugefügt haben.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Höhe bearbeiten auf **450** Pixel und Klicken **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Überprüfen **Bildlaufleisten anzeigen** , wenn Sie Zugriff auf Bildlaufaktivitäten benötigen.

   >[!TIP]
   >
   >Es wird empfohlen, eine Höhe von 410 Pixel für die Objekte &quot;Konten und Chancen&quot;zu verwenden.

1. Klicken Sie auf **Felder** auf der linken Seite. Suchen und ziehen Sie dann die **Interaktion** in die **Marketo Sales Insight** Layout.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Wiederholen Sie den obigen Schritt auch für diese Felder.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Interaktion</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Wert für Relativergebnis</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Wert für Wichtigkeit</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Datum des letzten interessanten Moments</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Beschreibung des letzten interessanten Moments</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Quelle des letzten interessanten Moments</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Typ des letzten interessanten Moments</p></td> 
  </tr> 
 </tbody> 
</table>

1. Klicks **Speichern** wenn fertig.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Wiederholen Sie diesen Vorgang, um VisualForce-Seitenabschnitte und Sales Insight-Felder für hinzuzufügen. **Kontakt**, **Konto** und **Chancen**.
1. Wiederholen Sie die Schritte 5 bis 7, um die Visualforce-Seitenabschnitte für Kontakt, Konto und Chancen hinzuzufügen. Wiederholen Sie dann die Schritte 8 bis 10, um Sales Insight-Felder für hinzuzufügen. **Kontakt**. Achten Sie darauf, nach jeder Änderung zu speichern.

## Benutzerdefinierte Personenfelder zuordnen {#map-custom-person-fields}

Marketo-Personenfelder müssen Salesforce-Kontaktfeldern zugeordnet werden, um sicherzustellen, dass die Konvertierung ordnungsgemäß funktioniert. So geht es.

1. Klicks **Einrichtung**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie in der Suchleiste nach &quot;fields&quot;und klicken Sie auf **Felder** under **Leads**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Klicks **Lead-Felder zuordnen**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Klicken Sie auf das Dropdown-Menü rechts für **Interaktion**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Auswählen **Contact.Engagement** in der Liste.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Wiederholen Sie diese Schritte und ordnen Sie sie zu.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Benutzerdefiniertes Feld für Marketo-Person</th> 
   <th colspan="1" rowspan="1">Salesforce Contact Custom Field</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Interaktion</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Wert für Relativergebnis</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Relativer Score-Wert</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Wert für Wichtigkeit</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Urgency value</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Datum des letzten interessanten Moments</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest-Moment-Datum</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Beschreibung des letzten interessanten Moments</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Quelle des letzten interessanten Moments</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Source</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Typ des letzten interessanten Moments</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest-Moment-Typ</p></td> 
  </tr> 
 </tbody> 
</table>

1. Klicks **Speichern** wenn Sie fertig sind.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Registerkarte &quot;Marketo Sales Insight-Konfiguration&quot; {#marketo-sales-insight-configuration-tab}

1. Klicken Sie in Salesforce auf die **+** Klicken Sie am Ende der Registerkartenleiste auf **Marketo Sales Insight-Konfiguration**.

1. Kopieren Sie die Anmeldeinformationen aus dem Soap-API-Bedienfeld in [Admin-Seite von Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} und fügen Sie sie in den Abschnitt Soap-API der Salesforce Sales Insight-Konfigurationsseite ein.

1. Kopieren Sie die Anmeldeinformationen aus dem Bedienfeld &quot;Rest-API&quot;in [Admin-Seite von Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} und fügen Sie sie in den Rest-API-Abschnitt der Salesforce Sales Insight-Konfigurationsseite ein.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Und das ist es! Sie sollten die Marketo Sales Insight -Felder für Leads, Kontakte, Konten und Chancen sehen können.

>[!NOTE]
>
>Wenn der Diagnosetest fehlgeschlagen ist, müssen Sie möglicherweise [Hinzufügen von mehr Feldern zum Seitenlayout](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>Bei Konten umfasst Sales Insight alle E-Mails, jedoch nur die neuesten interessanten Momente, Web-Aktivitäten und Bewertungsänderungen.

>[!MORELIKETHIS]
>
>* [Priorität, Dringlichkeit, relatives Ergebnis und beste Beta](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Hinzufügen der Marketo-Registerkarte zu Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Hinzufügen von Sales Insight-Zugriff zu Profilen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
