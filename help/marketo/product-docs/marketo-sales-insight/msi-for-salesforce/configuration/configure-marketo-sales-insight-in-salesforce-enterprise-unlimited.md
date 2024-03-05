---
unique-page-id: 2360368
description: Erfahren Sie, wie Sie Marketo Sales Insight in Salesforce Enterprise/Unlimited-Editionen konfigurieren.
title: Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 4%

---

# Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Konfigurieren Sie Marketo Sales Insight in Salesforce Enterprise/Unlimited-Editionen, indem Sie die folgenden Schritte ausführen.

>[!PREREQUISITES]
>
>[Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Administratorberechtigungen sind erforderlich.**

## Sales Insight in Marketo Engage konfigurieren {#configure-sales-insight-in-marketo}

1. Um Ihre Marketo Sales Insight-Anmeldeinformationen in Marketo Engage zu erhalten, navigieren Sie zum **[!UICONTROL Admin]** Bereich und wählen Sie **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Klicks **[!UICONTROL API-Konfiguration bearbeiten]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Geben Sie einen geheimen API-Schlüssel Ihrer Wahl ein und klicken Sie auf **[!UICONTROL Speichern]**. Verwenden Sie KEIN Und-Zeichen (`&`) in Ihrem API-geheimen Schlüssel.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Ihr API-geheimer Schlüssel ist wie ein Kennwort für Ihre Organisation und sollte sicher sein.

1. Um die Anmeldeinformationen einzutragen, klicken Sie auf **[!UICONTROL Ansicht]** im _[!UICONTROL Rest-API-Konfiguration]_ Bedienfeld.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Wenn ein Bestätigungsdialogfeld angezeigt wird, klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Lassen Sie dieses Fenster geöffnet. Sie benötigen diese Informationen später für die Salesforce-Konfiguration.

## Sales Insight in Salesforce konfigurieren {#configure-sales-insight-in-salesforce}

1. Klicken Sie in Salesforce auf **[!UICONTROL Einrichtung]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und wählen Sie **[!UICONTROL Remote Site Settings]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Klicks **[!UICONTROL Neue Remote-Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Geben Sie den Remote-Site-Namen ein (dieser kann in etwa so aussehen wie `MarketoSoapAPI`). Geben Sie die Remote-Site-URL ein, d. h. Ihre Marketo-Host-URL aus dem _[!UICONTROL Soap-API-Konfiguration]_ -Bedienfeld in Marketo Engage. Klicken Sie auf **[!UICONTROL Speichern]**. Sie haben jetzt Remote-Site-Einstellungen für die Soap-API erstellt.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Klicks **[!UICONTROL Neue Remote-Site]** erneut.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Geben Sie den Remote-Site-Namen ein (dieser kann in etwa so aussehen wie `MarketoAPI`). Geben Sie die Remote-Site-URL ein, die Ihre API-URL ist von _[!UICONTROL Rest-API-Konfiguration]_ -Bedienfeld in Marketo Engage. Klicken Sie auf **[!UICONTROL Speichern]**. Sie haben jetzt Remote-Site-Einstellungen für die Rest-API erstellt.

   >[!NOTE]
   >
   >_You_ Wählen Sie Ihre **[!UICONTROL Remote Site Name]** (`MarketoAPI` wird hier verwendet). Die **[!UICONTROL Remote Site URL]** finden Sie im Feld Marketo-Host des Dialogfelds API-Konfiguration bearbeiten in Schritt 3 im Abschnitt &quot;Configure Sales Insight in Marketo&quot;.

## Gewähren Sie Benutzern von Sales Insight Profilzugriff auf standardmäßige Salesforce-Objekte. {#grant-sales-insight-users-profile-access}

Aufgrund von Salesforce-Sicherheitsverbesserungen können AppExchange-Packages keine Berechtigung mehr für Standardobjekte erteilen. Der Zugriff auf die entsprechenden Salesforce-Objekte aus dem Salesforce-Benutzerprofil muss gewährt werden. Gehen Sie wie folgt vor, um die erforderlichen Berechtigungen zu gewähren.

1. Klicks **[!UICONTROL Einrichtung]**.

1. Suchen Sie &quot;Profile&quot; in Schnellsuche.

1. Klicks **[!UICONTROL Bearbeiten]** neben dem Profil, das Ihre Salesforce-Benutzer verwenden.

1. Unter dem _[!UICONTROL Standardobjektberechtigungen]_ Abschnitt aktivieren **[!UICONTROL Lesen]** Zugriff auf die folgenden Objekte: [!UICONTROL Lead], [!UICONTROL Kontakt], [!UICONTROL Konto], und [!UICONTROL Chancen].

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Seitenlayouts anpassen {#customize-page-layouts}

1. Klicks **[!UICONTROL Einrichtung]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Suchen Sie nach &quot;Seitenlayout&quot;und wählen Sie die **[!UICONTROL Seitenlayout]** under **[!UICONTROL Leads]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Klicks **[!UICONTROL Visualforce-Seiten]** auf der linken Seite. Ziehen **[!UICONTROL Abschnitt]** zum Layout unter dem _[!UICONTROL Benutzerspezifische Links]_ Abschnitt.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Geben Sie &quot;Marketo Sales Insight&quot;als **[!UICONTROL Bereichsname]** auswählen **[!UICONTROL 1-Spalte]** und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Drag &amp; Drop **[!UICONTROL Lead]** in den neuen Abschnitt ein.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Der Name dieses Felds ändert sich je nach Objekttyp. Wenn Sie beispielsweise das Seitenlayout für Kontakte ändern, wird &quot;Kontakt&quot;angezeigt.

1. Doppelklicken Sie auf die **[!UICONTROL Lead]** -Block, den Sie gerade hinzugefügt haben.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Höhe bearbeiten auf **450** Pixel und Klicken **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Überprüfen **[!UICONTROL Bildlaufleisten anzeigen]** , wenn Sie Zugriff auf Bildlaufaktivitäten benötigen.

   >[!TIP]
   >
   >Die empfohlene Höhe für die Objekte Konten und Chancen beträgt 410 Pixel.

1. Klicks **[!UICONTROL Felder]** auf der linken Seite. Suchen und ziehen Sie dann die **[!UICONTROL Dringlichkeit]** in die **[!UICONTROL Marketo Sales Insight]** Layout.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Wiederholen Sie den obigen Schritt auch für diese Felder.

   * Letzter interessanter Moment
   * Datum des letzten interessanten Moments
   * Beschreibung des letzten interessanten Moments
   * Quelle des letzten interessanten Moments
   * Typ des letzten interessanten Moments
   * Letzte Aktivität nach Vertrieb
   * Letzte Interaktion durch Verkäufe
   * MSI-Kontaktkennung
   * Relative Bewertung
   * Wert für Relativergebnis
   * Dringlichkeit
   * Wert für Wichtigkeit
   * In Marketo anzeigen

1. Klicks **[!UICONTROL Speichern]** wenn fertig.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Wiederholen Sie die Schritte 5 bis 7, um visuelle Force-Seitenabschnitte und Sales Insight-Felder für hinzuzufügen. **[!UICONTROL Kontakt]**, **[!UICONTROL Konto]**, und **[!UICONTROL Chancen]**.

1. Wiederholen Sie die Schritte 8 bis 10, um diese Sales Insight-Felder für hinzuzufügen. **[!UICONTROL Kontakt]**. Achten Sie darauf, alle Änderungen zu speichern.

   * Letzter interessanter Moment
   * Datum des letzten interessanten Moments
   * [!UICONTROL Letzter interessanter Moment Desc]
   * [!UICONTROL Letzte interessante Moment-Quelle]
   * [!UICONTROL Letzter interessanter Moment-Typ]
   * [!UICONTROL Letzte Marketo-Aktivität nach Vertrieb]
   * [!UICONTROL Letzte Marketo-Interaktion durch Vertrieb]
   * [!UICONTROL MKTO-Lead-Ergebnis]
   * [!UICONTROL Relative Punktzahl]
   * [!UICONTROL Relativer Score-Wert]
   * [!UICONTROL Sales Insight] - Öffnet die Seite &quot;Kontaktliste&quot;
   * [!UICONTROL Dringlichkeit]
   * [!UICONTROL Dringlichkeitswert]

## Benutzerdefinierte Personenfelder zuordnen {#map-custom-person-fields}

Marketo-Personenfelder müssen Salesforce-Kontaktfeldern zugeordnet werden, um sicherzustellen, dass die Konvertierung ordnungsgemäß funktioniert. Führen Sie diese Schritte aus, um sie zuzuordnen.

1. Klicks **[!UICONTROL Einrichtung]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Suchen Sie in der Suchleiste nach &quot;fields&quot;und klicken Sie auf **[!UICONTROL Felder]** under **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Klicks **[!UICONTROL Lead-Felder zuordnen]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Klicken Sie auf das Dropdown-Menü rechts für **[!UICONTROL Interaktion]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Auswählen **[!UICONTROL Contact.Engagement]** in der Liste.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Wiederholen Sie diese Schritte und ordnen Sie sie zu.

   | Benutzerdefiniertes Feld für Marketo-Person | Salesforce Contact Custom Field |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

1. Klicks **[!UICONTROL Speichern]** wenn Sie fertig sind.

## Marketo Sales Insight-Konfigurationsregisterkarte {#marketo-sales-insight-configuration-tab}

1. Klicken Sie in Salesforce auf die **+** Klicken Sie am Ende der Registerkartenleiste auf **[!UICONTROL Marketo Sales Insight-Konfiguration]**.

1. Kopieren Sie die Anmeldeinformationen aus dem Soap-API-Bedienfeld in [Admin-Seite von Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} und fügen Sie sie in den Abschnitt Soap-API der Salesforce Sales Insight-Konfigurationsseite ein.

1. Kopieren Sie die Anmeldeinformationen aus dem Bedienfeld &quot;Rest-API&quot;in [Admin-Seite von Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} und fügen Sie sie in den Rest-API-Abschnitt der Salesforce Sales Insight-Konfigurationsseite ein.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Sie sollten die Marketo Sales Insight -Felder für Leads, Kontakte, Konten und Chancen sehen können.

>[!NOTE]
>
>Wenn der Diagnosetest fehlgeschlagen ist, [Hinzufügen von mehr Feldern zum Seitenlayout](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} kann das Problem beheben.

>[!NOTE]
>
>Bei Konten umfasst Sales Insight alle E-Mails, jedoch nur die neuesten interessanten Momente, Web-Aktivitäten und Bewertungsänderungen.

>[!MORELIKETHIS]
>
>* [Priorität, Dringlichkeit, relatives Ergebnis und beste Beta](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Hinzufügen der Marketo-Registerkarte zu Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Hinzufügen von Sales Insight-Zugriff zu Profilen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
