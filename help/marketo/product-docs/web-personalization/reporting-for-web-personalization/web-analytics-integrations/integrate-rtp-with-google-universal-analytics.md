---
unique-page-id: 4720125
description: Integrieren von RTP mit Google Universal Analytics - Marketo-Dokumente - Produktdokumentation
title: Integrieren von RTP mit Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# Integrieren von RTP mit [!DNL Google Universal Analytics] {#integrate-rtp-with-google-universal-analytics}

## Einführung {#intro}

Nutzen Sie [!DNL Google Universal Analytics] (GUA) mit den Firmographie- und Personalisierungsdaten von [!DNL Marketo Real-Time Personalization] (RTP), um Ihre Online-Marketing-Maßnahmen besser zu messen und zu analysieren.

In diesem Beitrag wird erläutert, wie Sie die [!DNL Marketo Real-Time Personalization] (RTP)-Plattform mit [!DNL Google Universal Analytics] (GUA)-Konten einrichten und integrieren. RTP-Daten können an Ihr GUA-Konto angehängt werden, sodass Sie die Leistung von Organisationen, Branchen, Unternehmensgrafiken und RTP-Segmenten, die Ihre Website besuchen, anzeigen und anzeigen können.

**[!DNL Google Universal Analytics]**

[!DNL Google Universal Analytics] der RTP-Daten erhalten Sie ein besseres Verständnis dafür, wie B2B-Benutzer mit Ihren Online-Inhalten interagieren, und helfen Ihnen, Ihre Personalisierungskampagnen zu messen und bessere Ergebnisse zu erzielen. [Weitere Informationen über [!DNL Google Universal Analytics]](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1).

>[!NOTE]
>
>**Nur für Benutzende von Google Tag Manager**
>
>Es ist keine Codierung oder spezielle Konfiguration erforderlich. Stellen Sie sicher, dass Sie die folgende Checkliste ausfüllen:
>
>* RTP-Dimensionen werden in [!DNL Google Universal Analytics] erstellt
>* [RTP-Tag wird ordnungsgemäß im Google Tag Manager installiert](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* [!DNL Google Universal Analytics] Integration ist in den Kontoeinstellungen des RTP aktiviert
>* [[!DNL Google Universal Analytics] Tag ist im Google Tag Manager ordnungsgemäß konfiguriert](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Tag des Google-Tag-Managers ist ordnungsgemäß auf Ihrer Website installiert](https://developers.google.com/tag-manager/quickstart)

## Einrichten benutzerdefinierter Dimensionen in GUA {#set-up-custom-dimensions-in-gua}

1. In Google Analytics

   1. Wechseln Sie zu **[!UICONTROL Admin]**
   1. Wählen Sie die **[!UICONTROL Konto].**
   1. Wählen Sie die **[!UICONTROL Eigenschaft].**
   1. Wählen Sie **[!UICONTROL Benutzerdefinierte Definitionen]** und **[!UICONTROL Benutzerdefinierte Dimensionen]** aus.

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Eine neue benutzerdefinierte Dimension hinzufügen. Klicken Sie auf **[!UICONTROL +Neue benutzerdefinierte Dimension]**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Fügen Sie die folgenden **[!UICONTROL benutzerdefinierten Dimensionen] hinzu:**

<table>
 <tbody>
  <tr>
   <td><p><strong>Benutzerdefinierter Dimension-Name</strong></p></td>
   <td><p><strong>Umfang</strong></p></td>
   <td><p><strong>Aktiv</strong></p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Organisation</strong></p></td>
   <td><p>Sitzung</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Industry</strong></p></td>
   <td><p>Sitzung</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Kategorie</strong></p></td>
   <td><p>Sitzung</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Gruppe</strong></p></td>
   <td><p>Sitzung</p></td>
   <td><p align="center">✓</p></td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>**Benutzerdefinierte Dimension-Namen** müssen genau wie in der obigen Tabelle definiert sein (andernfalls werden benutzerdefinierte RTP-Dashboards und -Berichte in der GUA nicht korrekt angezeigt)

1. Fügen Sie den **[!UICONTROL Name]** hinzu. Wählen Sie den Bereich als &quot;**[!UICONTROL &quot;]**. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Ihre benutzerdefinierte Dimension-Liste sollte wie folgt aussehen.

![](assets/image2014-11-29-11-36-50-version-2.png)

Nachdem Sie die benutzerdefinierten Dimensionen in GUA aktiviert haben, wechseln Sie zur RTP-Plattform, um diese Dimensionen in RTP zu aktivieren.

## Aktivieren der GUA-Integration in Ihrem RTP-Konto {#activate-the-gua-integration-in-your-rtp-account}

1. Navigieren Sie in der RTP-Plattform zu **[!UICONTROL Kontoeinstellungen].**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Domain]**.
1. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Google Universal Analytics]**.
1. Aktivieren **[!UICONTROL die]** benutzerdefinierten Dimensionen und Ereignisse, um diese Daten von RTP an [!DNL Google Universal Analytics] anzuhängen.
1. Geben Sie die **[!UICONTROL Indexnummer]** der Dimension ein, die mit der Indexnummer in GUA ausgerichtet ist.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Die Indexnummer für die benutzerdefinierte Dimension finden Sie in der GUA unter Benutzerdefinierte Dimensionen.
>
>Beispiel: RTP-Industry Index Number ist gleich 1, RTP-Organization Index Number ist gleich 2.

## Alte Dashboards in Google Analytics entfernen {#remove-old-dashboards-in-google-analytics}

1. In Google Analytics. Navigieren Sie zu **[!UICONTROL Reporting].**
1. Klicken Sie auf **[!UICONTROL Dashboards].**
1. Wählen Sie ein **[!UICONTROL Dashboard]** aus (RTP B2B- oder RTP-Leistung)
1. Klicken Sie **[!UICONTROL Dashboard löschen]**.

![](assets/image2014-11-29-11-3a42-3a55.png)
