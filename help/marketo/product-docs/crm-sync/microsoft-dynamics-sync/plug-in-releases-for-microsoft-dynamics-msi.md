---
unique-page-id: 10099102
description: Plug-in-Versionen für Microsoft Dynamics MSI - Marketo Docs - Produktdokumentation
title: Plug-In-Versionen für Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 5%

---

# Plug-In-Versionen für Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Beim ersten Synchronisieren mit Microsoft Dynamics laden Sie die neueste Version der Plug-ins für Marketo Sales Insight (MSI) herunter und installieren sie. Marketo aktualisiert diese Plug-Ins regelmäßig, damit Sie zum gleichen Speicherort zurückkehren können, um die neue Version herunterzuladen.

Bitte [laden Sie das neueste Plugin](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) für Ihre Dynamics-Version herunter.

>[!NOTE]
>
>Diese Versionen können sowohl für lokale als auch für Online-Versionen von Dynamics verwendet werden.

## Aktualisieren der MSI-Lösung {#upgrading-your-msi-solution}

1. Importieren Sie die neueste Version der Lösung _über die vorhandene Version_ von Dynamics CRM, indem Sie die Schaltfläche **Import** in Dynamics drücken.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Beispiel: Wenn Ihr Dynamics CRM Version 2.0.0.20 und die neueste Version 2.0.0.21 hat, würden Sie _over_ Version 2.0.0.20 importieren.

1. Klicken Sie auf **Weiter**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Wählen Sie **Phase der Aktualisierung** und **Anpassungen beibehalten** und klicken Sie dann auf **Importieren**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Nach einem erfolgreichen Import werden Ihnen zwei MSI-Lösungen angezeigt: MarketoSalesInsight und MarketingSalesInsight_Upgrade. Wählen Sie die ältere Lösung aus und klicken Sie auf Lösungsaktualisierung anwenden.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Und das ist es! Nach der Aktualisierung wird nur eine MSI-Lösung angezeigt.

## Versionsupdates {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Releasedatum</th> 
   <th colspan="1">Version</th> 
   <th colspan="1">Hinweise:</th> 
  </tr> 
  <tr> 
   <td colspan="1">01.10.20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Fehlerbehebung: Zugriff auf MSI API-Konfigurationsfelder für Benutzer mit Sales Insight-Rolle zuweisen</td> 
  </tr> 
  <tr> 
   <td colspan="1">20.07.20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Fehlerbehebung: hinzufügen einer Überprüfungsmeldung für nicht synchronisierte Datensätze</td> 
  </tr> 
  <tr> 
   <td colspan="1">12.06.20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Fehlerbehebung: So blenden Sie das geheime MSI-Kennwort bei der MSD-API-Konfiguration aus</td> 
  </tr> 
  <tr> 
   <td colspan="1">26.05.20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Fehlerbehebung: So ändern Sie die MSI-Rollen-ID-Überprüfung für die Anzeige von MSI-Schaltflächen</td> 
  </tr> 
  <tr> 
   <td colspan="1">21.05.20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Fehlerbehebung: Rückgängigmachen des Ausblendens des Felds "Inhaber"und Nichterfüllung der Felder</td> 
  </tr> 
  <tr> 
   <td colspan="1">28.04.20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Fehlerbehebung: Entfernen der Link-Abhängigkeit für MSD CRM-Sitemap</td> 
  </tr> 
 </tbody> 
</table>
