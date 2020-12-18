---
unique-page-id: 4720125
description: RTP in Google Universal Analytics integrieren - Marketing Docs - Produktdokumentation
title: RTP in Google Universal Analytics integrieren
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# RTP in Google Universal Analytics integrieren {#integrate-rtp-with-google-universal-analytics}

## Intro {#intro}

Nutzen Sie Google Universal Analytics (GUA) mit den firmografischen Daten und Personalisierungsdaten von Marketo Real-Time Personalization (RTP), um Ihre Online-Marketingbemühungen besser zu messen und zu analysieren.

In diesem Beitrag wird beschrieben, wie Sie die Marketing Real-Time Personalization-Plattform (RTP) mit Google Universal Analytics-Konten (GUA) einrichten und integrieren. RTP-Daten können an Ihr GUA-Konto angehängt werden, sodass Sie die Ansicht und Performance von Unternehmen, Branchen, firmographischen Bereichen und RTP-Segmenten, die Ihre Website besuchen, sehen können.

**Google Universal Analytics**

Google Universal Analytics mit RTP-Daten bietet Ihnen ein besseres Verständnis, wie B2B-Benutzer mit Ihren Online-Inhalten interagieren, und hilft Ihnen, Ihre Personalisierungs-Kampagnen zu messen und bessere Ergebnisse zu erzielen. [Mehr über Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**`For Google Tag Manager Users Only`**
>
>Es muss keine Kodierung oder spezielle Konfiguration durchgeführt werden. Vergewissern Sie sich, dass Sie die folgende Checkliste ausfüllen:
>
>* `RTP dimensions are created in Google Universal Analytics`
>* [RTP-Tag ordnungsgemäß im Google Tag-Manager installiert](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* `Google Universal Analytics Integration is enabled in the RTP's Account Settings`
>* [Google Universal Analytics-Tag wurde im Google Tag Manager ordnungsgemäß konfiguriert](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag-Manager-Tag ordnungsgemäß auf Ihrer Website installiert ist](https://developers.google.com/tag-manager/quickstart)

>



## Benutzerdefinierte Dimensionen in GUA {#set-up-custom-dimensions-in-gua} einrichten

1. In Google Analytics

   1. Gehen Sie zu **Admin**
   1. Wählen Sie das **Konto**
   1. Wählen Sie die **Eigenschaft.**
   1. Wählen Sie **Benutzerdefinierte Dimensionen **und **Benutzerspezifische Definitionen.**

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. hinzufügen eine neue benutzerdefinierte Dimension. Klicken Sie auf **+Neue benutzerspezifische Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. hinzufügen Sie die folgenden **Benutzerspezifische Dimensionen:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Name der benutzerspezifischen Dimension</strong></p></td> 
   <td><p><strong>Einzugsbereich</strong></p></td> 
   <td><p><strong>Aktiv</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organisation</strong></p></td> 
   <td><p>Sitzung</p></td> 
   <td><p align="center">they</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Branche</strong></p></td> 
   <td><p>Sitzung</p></td> 
   <td><p align="center">they</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Kategorie</strong></p></td> 
   <td><p>Sitzung</p></td> 
   <td><p align="center">they</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Gruppe</strong></p></td> 
   <td><p>Sitzung</p></td> 
   <td><p align="center">they</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Die** Namen der benutzerdefinierten Dimension müssen exakt den in der obigen Tabelle definierten Namen entsprechen (ansonsten werden benutzerdefinierte RTP-Dashboard und Berichte in GUA nicht korrekt angezeigt).

1. hinzufügen **Name. **Wählen Sie den Bereich als **Sitzung aus.** Klicken Sie auf  **Erstellen.**

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Die Liste Ihrer benutzerspezifischen Dimension sollte wie folgt aussehen.

![](assets/image2014-11-29-11-36-50-version-2.png)

Nachdem Sie die benutzerdefinierten Dimensionen in GUA aktiviert haben, gehen Sie zur RTP-Plattform, um diese Dimensionen in RTP zu aktivieren.

## Aktivieren Sie die GUA-Integration in Ihrem RTP-Konto {#activate-the-gua-integration-in-your-rtp-account}

1. Wechseln Sie auf der RTP-Plattform zu **Kontoeinstellungen.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Klicken Sie unter **Kontoeinstellungen** auf **Domäne.**
1. Klicken Sie unter **Analytics **auf **Google Universal Analytics**.
1. Aktivieren Sie **Aktivieren Sie** die entsprechenden benutzerspezifischen Dimensionen und Ereignis, um diese Daten von RTP an Google Universal Analytics anzuhängen.
1. Geben Sie die **Indexnummer** der Dimension ein, die an der Indexnummer in GUA ausgerichtet ist.
1. Klicken Sie auf **Speichern**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Die Indexnummer für die benutzerdefinierte Dimension finden Sie in der GUA unter Benutzerdefinierte Dimensionen.
>
>Beispiel: RTP-Industry Index Number = 1, RTP-Organization Index Number = 2.

## Alte Dashboard in Google Analytics {#remove-old-dashboards-in-google-analytics} entfernen

1. In Google Analytics. Gehen Sie zu **Berichte.**
1. Klicken Sie auf **Dashboard.**
1. Wählen Sie ein **Dashboard **(RTP B2B oder RTP Performance)
1. Klicken Sie auf **Dashboard** löschen.

![](assets/image2014-11-29-11-3a42-3a55.png)

