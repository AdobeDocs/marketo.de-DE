---
unique-page-id: 3571743
description: Erfahren Sie, wie Sie Marketo Sales Insight in der Salesforce Professional Edition konfigurieren.
title: Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Konfigurieren von [!DNL Marketo Sales Insight] in [!DNL Salesforce] Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Konfigurieren Sie Marketo Sales Insight in Salesforce Professional Edition, indem Sie die folgenden Schritte ausführen.

>[!PREREQUISITES]
>
>* Installieren Sie Marketo in Ihrer [!DNL Salesforce] Professional Edition.
>
>* [install [!DNL Marketo Sales Insight] package in [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Administratorberechtigungen sind erforderlich.**

## Konfigurieren von Sales Insight in Marketo Engage {#configure-sales-insight-in-marketo}

1. Um die Anmeldedaten für Marketo Sales Insight von Ihrem Marketo-Konto abzurufen, öffnen Sie ein neues Browserfenster.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** und wählen Sie **[!UICONTROL Sales Insight]** aus.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Klicken Sie **[!UICONTROL API-Konfiguration bearbeiten]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Geben Sie einen beliebigen API-Geheimschlüssel ein und klicken Sie auf **[!UICONTROL Speichern]**. Verwenden Sie KEIN kaufmännisches Und-Zeichen (`&`) in Ihrem API-Geheimschlüssel.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Ihr API-Geheimschlüssel ist wie ein Kennwort für Ihre Organisation und sollte sicher sein.

1. Klicken Sie zum Ausfüllen der Anmeldeinformationen auf **[!UICONTROL Anzeigen]** im Bedienfeld _[!UICONTROL REST-API-Konfiguration]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Wenn Sie ein Bestätigungsdialogfeld sehen, klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Konfigurieren von Sales Insight in [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Klicken Sie in Salesforce auf **[!UICONTROL Setup]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Suchen Sie nach „Remote Site“ und wählen Sie **[!UICONTROL Remote Site Settings]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Geben Sie den Namen der Remote-Site ein (dies kann `MarketoSoapAPI` ähneln). Geben Sie die Remote-Site-URL, d. h. Ihre Marketo-Host-URL, über das Bedienfeld „SOAP-API-Konfiguration“ in Marketo Engage ein. Klicken Sie auf **[!UICONTROL Speichern]**. Sie haben jetzt Remote-Site-Einstellungen für die SOAP-API erstellt.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Klicken Sie erneut **[!UICONTROL Neue Remote-Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Geben Sie den Namen der Remote-Site ein (dies kann z. B. „MarketoRestAPI“ sein). Geben Sie die Remote-Site-URL ein, d. h. Ihre API-URL aus dem Bedienfeld „REST-API-Konfiguration“ in Marketo. Klicken Sie auf **[!UICONTROL Speichern]**. Sie haben jetzt Remote-Site-Einstellungen für die Rest-API erstellt.

## Gewähren des Profilzugriffs für Sales Insight-Benutzer auf standardmäßige Salesforce-Objekte {#grant-sales-insight-users-profile-access}

Aufgrund der Salesforce-Sicherheitsverbesserungen können AppExchange-Pakete keine Berechtigungen mehr für Standardobjekte erteilen, und der Zugriff auf die entsprechenden Salesforce-Objekte muss über das Benutzerprofil von Salesforce gewährt werden. Gewähren Sie die erforderlichen Berechtigungen, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie **[!UICONTROL Setup]**.

1. Suchen Sie in der Schnellsuche nach „Profile“.

1. Klicken Sie **[!UICONTROL Bearbeiten]** neben dem Profil, das Ihre Salesforce-Benutzenden verwenden.

1. Aktivieren Sie im Abschnitt Standardobjektberechtigung den Lesezugriff für die folgenden Objekte: Lead, Kontakt, Konto und Opportunity.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Seiten-Layouts anpassen {#customize-page-layouts}

1. Klicken Sie **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie nach „Seiten-Layout“ und wählen Sie **[!UICONTROL Seiten-Layout]** unter **[!UICONTROL Leads]**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Klicken **[!UICONTROL links auf]** VisualForce-Seiten“. Ziehen Sie **[!UICONTROL Abschnitt]** in das Layout unter dem Abschnitt Benutzerdefinierte Links .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Geben Sie als „Abschnittsname **[!UICONTROL &quot;Marketo Sales Insight&quot;]**. Wählen Sie **[!UICONTROL 1-Column]** und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Ziehen Sie **[!UICONTROL Lead]** per Drag-and-Drop in den neuen Abschnitt.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Der Name dieses Feldes ändert sich je nach Objekttyp. Wenn Sie beispielsweise das Seiten-Layout für Kontakte ändern, wird Kontakt angezeigt.

1. Doppelklicken Sie auf den **[!UICONTROL Lead]**-Block, den Sie soeben hinzugefügt haben.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Bearbeiten Sie die Höhe auf 450 Pixel und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Aktivieren Sie **[!UICONTROL Bildlaufleisten anzeigen]**, wenn Sie Zugriff auf Bildlaufaktivitäten benötigen.

   >[!TIP]
   >
   >Die empfohlene Höhe für die Objekte Accounts und Opportunities beträgt 410 Pixel.

1. Klicken Sie **[!UICONTROL der linken]** auf „Felder“. Suchen Sie dann die Beschriftung **[!UICONTROL Interaktion]** und ziehen Sie sie in das Layout **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Wiederholen Sie den vorherigen Schritt für die folgenden Felder:

   * [!UICONTROL Interaktion]
   * [!UICONTROL Relativer Score-Wert]
   * [!UICONTROL Dringlichkeitswert]
   * [!UICONTROL Datum des letzten interessanten Moments]
   * [!UICONTROL Beschreibung des letzten interessanten Moments]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Typ des letzten interessanten Moments]

1. Klicken Sie **[!UICONTROL Speichern]** wenn Sie fertig sind.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Wiederholen Sie die Schritte 5 **[!UICONTROL 7, um die Seitenabschnitte für Kontakt]**, **[!UICONTROL Konto]** und **[!UICONTROL Gelegenheit]** hinzuzufügen.

1. Wiederholen Sie die Schritte 8 bis 10, um Insight-Felder für den Vertrieb (**[!UICONTROL )]**. Denken Sie daran, nach jeder Änderung zu speichern.

## Benutzerdefinierte Personenfelder zuordnen {#map-custom-person-fields}

Personenfelder für Marketo müssen den Salesforce-Kontaktfeldern zugeordnet werden, um sicherzustellen, dass die Konvertierung ordnungsgemäß funktioniert. Führen Sie die folgenden Schritte aus, um sie zuzuordnen.

1. Klicken Sie **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Suchen Sie in der Suchleiste nach „fields“ und klicken Sie unter **[!UICONTROL Leads]** auf **[!UICONTROL Fields]**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Klicken Sie **[!UICONTROL Lead-Felder zuordnen]**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Klicken Sie auf das Dropdown-Menü auf der rechten Seite für **[!UICONTROL Interaktion]**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Wählen **[!UICONTROL Kontakt.Interaktion]** in der Liste aus.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Wiederholen Sie diese Felder und ordnen Sie sie auch zu.

   | Benutzerdefiniertes Feld für Marketo-Person | Benutzerdefiniertes Salesforce-Kontaktfeld |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Registerkarte Marketo Sales Insight-Konfiguration {#marketo-sales-insight-configuration-tab}

1. Klicken Sie in Salesforce auf das **+** am Ende der Registerkartenleiste und dann auf **[!UICONTROL Marketo Sales Insight Config]**.

1. Kopieren Sie die Anmeldeinformationen aus dem SOAP-API-Bedienfeld auf der Admin-Seite von Marketo Insight [0&rbrace; und fügen Sie sie im Abschnitt SOAP-API der Konfigurationsseite von Salesforce Sales Insight ein.](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}

1. Kopieren Sie die Anmeldeinformationen aus dem Bedienfeld **[!UICONTROL REST]** in der [Marketo Sales Insight Admin-](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} und fügen Sie sie im Abschnitt REST-API der Salesforce Sales Insight-Konfigurationsseite ein.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Sie sollten die Marketo Sales Insight-Felder für Leads, Kontakte, Konten und Opportunities sehen können.

>[!NOTE]
>
>Wenn der Diagnosetest fehlgeschlagen ist, kann [&#x200B; Problem möglicherweise durch Hinzufügen weiterer Felder &#x200B;](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} Seiten-Layout behoben werden.

>[!NOTE]
>
>Bei Accounts umfasst Sales Insight alle E-Mails, aber nur die interessantesten Momente, Web-Aktivitäten und Bewertungsänderungen.

>[!MORELIKETHIS]
>
>* [Priorität, Dringlichkeit, relative Punktzahl und Best Bets](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Registerkarte &quot;Marketo hinzufügen“ zu [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Hinzufügen von Sales Insight-Zugriff zu Profilen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
