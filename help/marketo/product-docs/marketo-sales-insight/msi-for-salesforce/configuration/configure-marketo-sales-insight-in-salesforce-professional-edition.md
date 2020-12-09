---
unique-page-id: 3571743
description: Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition - Marketing Docs - Produktdokumentation
title: Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---


# Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Hier finden Sie die Schritte, die Sie zur Konfiguration von Marketo Sales Insight in Salesforce Professional Edition unternehmen müssen. Fangen wir an!

>[!PREREQUISITES]
>
>[Installieren Sie Marketo in Ihrer Salesforce Professional Edition](http://docs.marketo.com/display/docs/professional+edition)
>
>[Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Sales Insight in Marketing konfigurieren {#configure-sales-insight-in-marketo}

1. Öffnen Sie ein neues Browserfenster, um die Anmeldeinformationen von MarketingTo Sales Insight von Ihrem Marketing-Konto abzurufen.
1. Gehen Sie zum Admin-Bereich und wählen Sie **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Klicken Sie auf API-Konfiguration **bearbeiten**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Geben Sie einen geheimen API-Schlüssel Ihrer Wahl ein und klicken Sie auf **Speichern**. Verwenden Sie KEIN kaufmännisches Und (&amp;) im geheimen Schlüssel Ihrer API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Ihr geheimer API-Schlüssel ist wie ein Kennwort für Ihr Unternehmen und sollte sicher sein.

1. Klicken Sie im Bedienfeld &quot;Rest-API-Konfiguration&quot;auf **Ansicht** , um die Anmeldeinformationen auszufüllen.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Es wird ein Bestätigungs-Popup angezeigt. Klicken Sie auf **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Sales Insight in Salesforce konfigurieren {#configure-sales-insight-in-salesforce}

1. Klicken Sie in Salesforce auf **Setup**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und wählen Sie **Remote-Site-Einstellungen**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Klicken Sie auf **Neue Remote-Site**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoSoapAPI&quot;). Geben Sie die Remote-Site-URL ein, d. h. Ihre MarketingTo-Host-URL aus dem Bedienfeld &quot;Soap-API-Konfiguration&quot;in Marketing. Klicken Sie auf **Speichern**. Sie haben jetzt Remote-Site-Einstellungen für die Soap-API erstellt.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Klicken Sie erneut auf **Neue Remote-Site** .

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoRestAPI&quot;). Geben Sie die Remote-Site-URL ein, die Ihre API-URL aus dem Bedienfeld &quot;Rest-API-Konfiguration&quot;in Marketing ist. Klicken Sie auf **Speichern**. Sie haben jetzt Einstellungen für die Remote-Site für die Rest-API erstellt.

## Einrichten von MarketingTo Sales Insight {#set-up-marketo-sales-insight}

1. Melden Sie sich bei Ihrer Marketing-Instanz an und klicken Sie auf **Admin**.

   ![](assets/login-admin-1.png)

1. Klicken Sie auf** Sales Insight**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Klicken Sie auf API-Konfiguration **bearbeiten**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Geben Sie einen geheimen **API-Schlüssel** ein und klicken Sie auf **Speichern**.

   >[!CAUTION]
   >
   >Verwenden Sie kein kaufmännisches Und-Zeichen (&amp;) in Ihrem API-geheimen Schlüssel.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Lassen Sie dieses Fenster geöffnet. Sie benötigen diese Informationen später in Salesforce.

1. Gehen Sie zurück zu Salesforce und klicken Sie auf **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und klicken Sie unter &quot; **Sicherheitseinstellungen&quot;auf** Remote-Site-Einstellung ****.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Klicken Sie auf **Neue Remote-Site**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Geben Sie **Remote-Site-Namen** und **Remote-Site-URL** ein und klicken Sie dann auf **Speichern**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Sie wählen Ihren **Remote-Site-Namen** aus (hier wird MarketoAPI verwendet). Die **Remote-Site-URL** befindet sich in Schritt 4 im Feld &quot;Marketo-Host&quot;des Dialogfelds &quot;API-Konfiguration bearbeiten&quot;.

## Seitenlayouts anpassen {#customize-page-layouts}

1. Klicken Sie auf **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie nach &quot;Seitenlayout&quot;und wählen Sie das **Seitenlayout** unter &quot; **Interessenten**&quot;aus.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Klicken Sie auf **Visualforce-Seiten **links. Ziehen Sie **Abschnitt** in das Layout unter dem Abschnitt Benutzerspezifische Links.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Geben Sie als **Abschnittsnamen**&quot;Marketing to Sales Insight&quot;ein. Wählen Sie **1-Spalte** und klicken Sie auf **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Ziehen Sie **Interessenten** per Drag &amp; Drop in den neuen Abschnitt.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Der Name dieses Felds ändert sich je nach Objekttyp. Wenn Sie z. B. das Seitenlayout für Kontakte ändern, wird &quot;Kontakt&quot;angezeigt.

1. Klicken Sie mit der Dublette auf den soeben hinzugefügten **Interessentenblock** .

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Bearbeiten Sie die Höhe auf **450** Pixel und klicken Sie auf **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >Für die Objekte &quot;Konten und Chancen&quot;wird eine Höhe von 410 Pixel empfohlen.

1. Klicken Sie auf **Felder **links. Suchen Sie dann nach der **Interaktionsbeschriftung** und ziehen Sie sie in das Layout **Marketing to Sales Insight** .

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Wiederholen Sie den obigen Schritt auch für diese Felder.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Interaktion</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>relativer Score-Wert</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dringlichkeitswert</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Datum des letzten interessanten Moments</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Letzter interessanter Moment Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Letzter interessanter Moment Quelle</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Letzter interessanter Moment-Typ</p></td> 
  </tr> 
 </tbody> 
</table>

1. Klicken Sie abschließend auf **Speichern** .

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Wiederholen Sie diesen Vorgang, um Visualforce-Seitenabschnitte und Sales Insight-Felder für **Kontakt**, **Konto** und **Möglichkeiten** hinzuzufügen.
1. Wiederholen Sie die Schritte 5 bis 7, um Visualforce-Seitenabschnitte für Kontakt, Konto und Chancen hinzuzufügen. Wiederholen Sie dann die Schritte 8-10, um Sales Insight-Felder für **Kontakt** hinzuzufügen. Achten Sie darauf, nach jeder Änderung zu speichern.

## Benutzerdefinierte Benutzerfelder zuordnen {#map-custom-person-fields}

Marketo-Personenfelder müssen Salesforce-Kontaktfeldern zugeordnet werden, um sicherzustellen, dass die Konvertierung ordnungsgemäß funktioniert. So geht es.

1. Klicken Sie auf **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie in der Suchleiste nach &quot;Feldern&quot;und klicken Sie auf **Felder** unter **Interessenten**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Klicken Sie auf **Lead-Felder** zuordnen.

   ** ![](assets/image2015-6-1-9-3a58-3a48-1.png)

   **

1. Klicken Sie auf das Dropdown-Menü rechts für **Interaktion**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Wählen Sie **Kontakt.Interaktion **in der Liste aus.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Wiederholen Sie diese Schritte und ordnen Sie sie auch zu.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Benutzerdefiniertes Feld "markieren"</th> 
   <th colspan="1" rowspan="1">Salesforce - Benutzerdefiniertes Feld kontaktieren</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Interaktion</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>relativer Score-Wert</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Relativer Score-Wert</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dringlichkeitswert</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Ursprünglicher Wert</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Datum des letzten interessanten Moments</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last interessant moment Date</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Letzter interessanter Moment Desc</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last interessant Moment Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Letzter interessanter Moment Quelle</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Source</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Letzter interessanter Moment-Typ</p></td> 
   <td colspan="1" rowspan="1"><p>Kontakt.Letzter interessanter Moment-Typ</p></td> 
  </tr> 
 </tbody> 
</table>

1. Klicken Sie auf **Speichern **nach Abschluss des Vorgangs.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketing-Sales Insight-Konfiguration {#marketo-sales-insight-config}

1. Klicken Sie auf **+ **und wählen Sie dann **Marketo Sales Insight Config**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Markieren Sie **Markieren-API** aktivieren. Geben Sie dann die [API-Konfigurationsinformationen in Marketing Admin](http://docs.marketo.com/display/DOCS/Configure+Marketo+Sales+Insight+in+Salesforce+Professional+Edition#ConfigureMarketoSalesInsightinSalesforceProfessionalEdition-SetupMarketoSalesInsight)ein. Klicken Sie auf **Änderungen speichern **nach Abschluss des Vorgangs.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Wenn der Diagnosetest fehlgeschlagen ist, müssen Sie eventuell weitere Felder zum Seitenlayout [hinzufügen](http://nation.marketo.com/docs/DOC-1115).

Und das ist es! Sie sollten in der Lage sein, die Marketing Sales Insight-Felder für Interessenten, Kontakte, Konten und Chancen anzuzeigen.

![](assets/twenty-six-1.png)

>[!NOTE]
>
>Bei Konten umfasst Sales Insight alle E-Mails, jedoch nur die neuesten interessanten Momente, Web-Aktivitäten und Ergebnisänderungen.

## Zugriff auf Marketing zu Sales Insight {#access-marketo-sales-insight}

1. Klicken Sie in Salesforce auf das **+** -Zeichen am Ende der Registerkartenleiste und klicken Sie auf **MarketingTo Sales Insight Config**.
1. Aktivieren Sie das Kontrollkästchen Markieren-API **aktivieren** .
1. Kopieren Sie die Anmeldeinformationen aus dem Bedienfeld &quot;SOAP-API&quot;auf der Marketing Sales Insight-Administrationsseite und fügen Sie sie in den Abschnitt &quot;SOAP-API&quot;auf der Seite &quot;Salesforce Sales Insight-Konfiguration&quot;ein.
1. Kopieren Sie die Anmeldeinformationen aus dem Bedienfeld &quot;Rest-API&quot;auf der Marketing Sales Insight-Administrationsseite und fügen Sie sie in den Abschnitt &quot;Rest-API&quot;der Seite &quot;Salesforce Sales Insight-Konfiguration&quot;ein.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Priorität, Dringlichkeit, relatives Ergebnis und beste Einsätze](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [hinzufügen Marketo Sales Insight-Registerkarte und Schaltflächen zu Salesforce](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

>



hhh