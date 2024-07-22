---
unique-page-id: 4720125
description: Integrieren von RTP in Google Universal Analytics - Marketo Docs - Produktdokumentation
title: RTP in Google Universal Analytics integrieren
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

---

# RTP in Google Universal Analytics integrieren {#integrate-rtp-with-google-universal-analytics}

## Einführung {#intro}

Nutzen Sie Google Universal Analytics (GUA) mit den firmografischen und Personalisierungsdaten von Marketo Real-Time Personalization (RTP), um Ihre Online-Marketingbemühungen besser zu messen und zu analysieren.

In diesem Beitrag wird beschrieben, wie Sie die Marketo Real-Time Personalization (RTP)-Plattform mit GUA-Konten (Google Universal Analytics) einrichten und integrieren. RTP-Daten können an Ihr GUA-Konto angehängt werden, damit Sie die Leistung von Organisationen, Branchen, firmographischen Systemen und RTP-Segmenten, die Ihre Website besuchen, anzeigen und sehen können.

**Google Universal Analytics**

Google Universal Analytics mit RTP-Daten liefert Ihnen ein besseres Verständnis davon, wie B2B-Benutzer mit Ihren Online-Inhalten interagieren, und hilft Ihnen, Ihre Personalisierungskampagnen zu messen und bessere Ergebnisse zu erzielen. [Mehr über Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Nur für Google Tag Manager-Benutzer**
>
>Es ist keine Kodierung oder spezielle Konfiguration erforderlich. Vergewissern Sie sich, dass Sie die folgende Checkliste abgeschlossen haben:
>
>* RTP-Dimensionen werden in Google Universal Analytics erstellt
>* [RTP-Tag ist ordnungsgemäß im Google Tag Manager installiert](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* Die Integration von Google Universal Analytics ist in den RTP-Kontoeinstellungen aktiviert.
>* [Google Universal Analytics-Tag ist ordnungsgemäß im Google Tag Manager konfiguriert](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Das Tag &quot;Google Tag Manager&quot;ist ordnungsgemäß auf Ihrer Website installiert](https://developers.google.com/tag-manager/quickstart)

## Einrichten benutzerdefinierter Dimensionen in der GUA {#set-up-custom-dimensions-in-gua}

1. in Google Analytics

   1. Wechseln Sie zu **Admin** .
   1. Wählen Sie das **Konto.**
   1. Wählen Sie die Eigenschaft **aus.**
   1. Wählen Sie **Benutzerdefinierte Definitionen** und **Benutzerdefinierte Dimensionen** aus.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Fügen Sie eine neue benutzerdefinierte Dimension hinzu. Klicken Sie auf **+Neue benutzerdefinierte Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Fügen Sie die folgenden **benutzerdefinierten Dimensionen hinzu:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Benutzerspezifischer Dimension-Name</strong></p></td> 
   <td><p><strong>Geltungsbereich</strong></p></td> 
   <td><p><strong>Aktiv</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organisation</strong></p></td> 
   <td><p>Sitzung</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Branche</strong></p></td> 
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
>**Benutzerdefinierte Dimension-Namen** müssen genau wie in der obigen Tabelle definiert sein (ansonsten werden benutzerdefinierte RTP-Dashboards und -Berichte in GUA nicht korrekt angezeigt)

1. Fügen Sie den **Namen** hinzu. Wählen Sie unter Perimeter den Wert **Sitzung** aus. Klicken Sie auf **Erstellen**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Die Liste der benutzerdefinierten Dimensionen sollte wie folgt aussehen:

![](assets/image2014-11-29-11-36-50-version-2.png)

Nachdem Sie die benutzerdefinierten Dimensionen in GUA aktiviert haben, gehen Sie zur RTP-Plattform, um diese Dimensionen in RTP zu aktivieren.

## Aktivieren der GUA-Integration in Ihrem RTP-Konto {#activate-the-gua-integration-in-your-rtp-account}

1. Wechseln Sie in der RTP-Plattform zu **Kontoeinstellungen**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Klicken Sie unter **Kontoeinstellungen** auf **Domäne**.
1. Klicken Sie unter &quot;**Analytics**&quot;auf &quot;**Google Universal Analytics**&quot;.
1. Aktivieren Sie **die entsprechenden benutzerdefinierten Dimensionen und Ereignisse, um diese Daten von RTP an Google Universal Analytics anzuhängen.**
1. Geben Sie die **Indexnummer** der Dimension ein, die mit der Indexnummer in GUA ausgerichtet ist.
1. Klicken Sie auf **Speichern**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Die Indexnummer für die benutzerdefinierte Dimension finden Sie in der GUA unter Benutzerdefinierte Dimensionen.
>
>Beispiel: RTP-Industry Index Number = 1, RTP-Organization Index Number = 2.

## Alte Dashboards in Google Analytics entfernen {#remove-old-dashboards-in-google-analytics}

1. In Google Analytics. Wechseln Sie zu **Berichterstellung**.
1. Klicken Sie auf **Dashboards**.
1. Wählen Sie ein **Dashboard** aus (RTP B2B- oder RTP-Leistung)
1. Klicken Sie auf **Dashboard löschen**.

![](assets/image2014-11-29-11-3a42-3a55.png)
