---
description: Erfahren Sie, wie Sie den Berechtigungssatz „Sales Insight" in Salesforce hinzufügen. Weisen Sie das Set Benutzern zu, die Zugriff auf Marketo Sales Insight benötigen.
title: Hinzufügen eines Sales Insight-Berechtigungssatzes
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/uFyP8aZCuXSPJn5ktZUxmCoVekyw9LN88U3KaY06-do
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 427d3327b9d5641dbc6744ee32ee8803ae76d6fe
workflow-type: tm+mt
source-wordcount: 393
ht-degree: 3%

---

# [!DNL Sales Insight] Berechtigungssatz hinzufügen {#add-sales-insight-permission-set}

Führen Sie die folgenden Schritte aus, um Zugriff auf [!DNL Sales Insight] Funktionen in [!DNL Salesforce] hinzuzufügen. Gilt für [!DNL Salesforce] Classic und Lightning

>[!PREREQUISITES]
>
>[Aktualisieren Sie  [!DNL Sales Insight] [!DNL Salesforce] Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} auf Version 1.8000 oder höher, um diese Funktion zu verwenden.

>[!IMPORTANT]
>
>* Wenn Sie zuvor allen Ihren Benutzern Zugriff auf [!DNL Sales Insight] Profile erteilt und/oder [!DNL Sales Insight] implementiert haben, müssen Sie [Zugriff auf Profilebene entfernen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} um diesen Berechtigungssatz verwenden zu können.
>
>* Die Salesforce-Standardlizenz ist erforderlich, um die volle Funktionalität von MSI nutzen zu können. Benutzende mit der Salesforce Platform-Lizenz (einer eingeschränkten Lizenzklasse) sehen möglicherweise Fehler beim Ausführen bestimmter Aktionen oder beim Zugriff auf einige Registerkarten.

## Überblick {#overview}

Die Berechtigung &quot;Marketo-App“ ist Teil des [!DNL Sales Insight]-[!DNL Salesforce]. Dazu gehört der Zugriff auf die unten genannten Objekte, Apex-Klassen und VisualForce-Seiten. Diese sind erforderlich, um auf alle [!DNL Sales Insight] Funktionen zuzugreifen.

**Objekteinstellungen**

<table>
 <tbody>
 <tr>
   <td>BestBetsCache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>Details zur Ansicht mit vielversprechenden Kontakten</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>Beste Ansichten</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>EmailActivityCache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>GetMethodArgus</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>GroupedWebActivityCache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>InterestingMomentsCache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>Marketo [!DNL Sales Insight] Config</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>Scoring-Cache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>Werte</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
  <tr>
   <td>WebActivityCache</td>
   <td>Lesen, Erstellen, Bearbeiten, Löschen, Alle anzeigen, Alle ändern</td>
  </tr>
 </tbody>
</table>

* Apex Class Access: 159 Apex-Klassen, die mit „mkto_si“ beginnen
* VisualForce Seitenzugriff: 64 VisualForce-Seiten, die mit „mkto_si“ beginnen
* Benutzerdefinierte Einstellungsdefinitionen: mkto_si.Marketo Settings &amp; mkto_si.User Preferences

## Hinzufügen des Marketo-App-Berechtigungssatzes zu Benutzenden {#adding-marketo-app-permission-set-to-users}

1. Melden Sie sich bei Ihrem [!DNL Salesforce] an.

1. Klicken Sie **[!UICONTROL Setup]**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Klicken Sie unter „Administrator“ auf **[!UICONTROL Benutzer verwalten]** und dann auf **[!UICONTROL Benutzer]**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Wählen Sie unter Alle Benutzer den Benutzer aus, dem Sie Zugriff gewähren möchten, und klicken Sie dann auf **[!UICONTROL Zuweisungen für Berechtigungssätze]**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Klicken Sie **[!UICONTROL Zuweisungen bearbeiten]**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Wählen Sie **[!UICONTROL Marketo App Access]** aus den verfügbaren Berechtigungssätzen und **[!UICONTROL Hinzufügen]**. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Wenn Sie nun auf der Seite Benutzerdetails nach unten scrollen, sehen Sie „Zugriff auf Marketo-Mobile-Apps“ unter „Zuweisungen von Berechtigungssätzen“.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Benutzende, die keinen Zugriff auf [!DNL Sales Insight] haben, sehen die folgende Meldung: „Sie verfügen nicht über die erforderlichen Berechtigungen, um auf diese Registerkarte zuzugreifen.“

Das ist alles! Sie haben [!DNL Sales Insight] Zugriff erfolgreich hinzugefügt. Wiederholen Sie die gleichen Schritte für jedes andere Profil, dem Sie Zugriff hinzufügen möchten.
