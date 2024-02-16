---
unique-page-id: 10099102
description: Plug-in-Versionen für Microsoft Dynamics MSI - Marketo Docs - Produktdokumentation
title: Plug-in-Versionen für Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6dcda9b86555c17b3492a02f3985db7d2acd8a32
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Plug-in-Versionen für Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Bei der ersten Synchronisierung mit Microsoft Dynamics laden Sie die neueste Version der Plug-ins für Marketo Sales Insight (MSI) herunter und installieren sie. Marketo Engage aktualisiert diese Plug-ins regelmäßig, sodass Sie zum selben Ort zurückkehren können, um die neue Version herunterzuladen.

Wenn Sie die native CRM-Synchronisierungslösung von Marketo mit Dynamics verwenden, [das neueste Plug-in herunterladen](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Diese Versionen funktionieren sowohl für On-Premise- als auch für Online-Versionen von Dynamics.

## Upgrade Ihrer MSI-Lösung {#upgrading-your-msi-solution}

1. Importieren Sie die neueste Version der Lösung _über die vorhandene Version_ Ihres Dynamics CRM durch Drücken der **[!UICONTROL Import]** in Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Beispiel: Wenn Ihr Dynamics CRM-System über Version 2.0.0.20 verfügt und die neueste Version 2.0.0.21 ist, würden Sie importieren _over_ Version 2.0.0.20.

1. Klicks **[!UICONTROL Nächste]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Auswählen **[!UICONTROL Upgrade-Phase]** und **[!UICONTROL Verwalten von Anpassungen]** Klicken Sie auf **[!UICONTROL Import]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Klicks **[!UICONTROL Nächste]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Nach einem erfolgreichen Import sehen Sie zwei MSI-Lösungen: MarketoSalesInsight und MarketoSalesInsight_Upgrade. Wählen Sie die ältere Lösung aus und klicken Sie auf Lösungsaktualisierung anwenden.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Und das ist es! Nach dem Upgrade wird nur eine MSI-Lösung angezeigt.

## Versionsaktualisierungen {#version-updates}

<table> 
 <tbody> 
  <tr> 
   <th>Veröffentlichungsdatum</th> 
   <th>Version</th> 
   <th>Hinweise</th> 
  </tr>
  <tr> 
   <td>14.02.24</td> 
   <td>2,00,31</td> 
   <td>Änderungen an der Paginierung in der anonymen Web-Aktivität.
   <p>
   Verschlüsseln Sie geheime Schlüsselinformationen aus der Benutzeransicht. Das Kennwort muss nach dem Import des neuen Pakets geändert werden, damit eine Verschlüsselung erfolgt.</td> 
  </tr>
  <tr> 
   <td>18.10.23</td> 
   <td>2 00 30</td> 
   <td>Konsolidierung des MSI-Fehlerprotokolls und Entfernen von Info-Benachrichtigungen aus der Anzeige auf der Marketo-Fehlerentität.</td> 
  </tr>
  <tr> 
   <td>19.05.23</td> 
   <td>2,00,29</td> 
   <td>Es wurden Paginierungsprobleme bei Webaktivität und interessanten Momenten im globalen Dashboard behoben.</td> 
  </tr>
  <tr> 
   <td>23.03.23</td> 
   <td>2,00,28</td> 
   <td>Erstellt eine <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">neues Paket</a> für MSI für nicht native Verbindungen mit dem CRM.</td> 
  </tr>
  <tr> 
   <td>03.02.22</td> 
   <td>2.0.0.27</td> 
   <td>Kontolayout für Einblicke: Interessante Momente, Bewertungsänderungen, Web-Aktivitäten, E-Mail-Aktivitäten.</td> 
  </tr>
  <tr> 
   <td>05.01.22</td> 
   <td>2.0.0.26</td> 
   <td>Programmakzeptanzwert für E-Mail-Versand.</td> 
  </tr>
  <tr> 
   <td>28.10.21</td> 
   <td>2.0.0.25</td> 
   <td>Metriken zur Produktakzeptanz, neues globales Dashboard (Web-Aktivität, E-Mail, Best-Bets).</td> 
  </tr>
  <tr> 
   <td>10.02.21</td> 
   <td>2.0.0.22</td> 
   <td>Entfernen Sie die automatische Prüfung aktiviert und Dokumentationsänderungen an der MSI-Lösung.</td> 
  </tr>
  <tr> 
   <td>10.1.20</td> 
   <td>2.0.0.21</td> 
   <td>Fehlerbehebung: Zuweisen des Zugriffs auf MSI-API-Konfigurationsfelder für Benutzer mit der Rolle "Sales Insight".</td> 
  </tr> 
  <tr> 
   <td>20.07.20</td> 
   <td>2.0.0.20</td> 
   <td>Fehlerbehebung: Fügen Sie eine Validierungsmeldung für nicht synchronisierte Datensätze hinzu.</td> 
  </tr> 
  <tr> 
   <td>12.06.20</td> 
   <td>2.0.0.19</td> 
   <td>Fehlerbehebung: Zum Ausblenden des geheimen MSI-Kennworts in der MSD-API-Konfiguration.</td> 
  </tr> 
  <tr> 
   <td>26.05.20</td> 
   <td>2.0.0.18</td> 
   <td>Fehlerbehebung: Zum Ändern der MSI-Rolle-ID-Überprüfung für die Anzeige von MSI-Schaltflächen.</td> 
  </tr> 
  <tr> 
   <td>21.05.20</td> 
   <td>2.0.0.17</td> 
   <td>Fehlerbehebung: Machen Sie das Feld "Inhaber ausblenden"und machen Sie Felder nicht obligatorisch.</td> 
  </tr> 
  <tr> 
   <td>28.04.20</td> 
   <td>2.0.0.16</td> 
   <td>Fehlerbehebung: Entfernen der Link-Abhängigkeit von MSD CRM-Sitemap-Einstellungen.</td> 
  </tr> 
 </tbody> 
</table>
