---
unique-page-id: 10099389
description: Marketo Plugin Releases für Microsoft Dynamics - Marketo Docs - Produktdokumentation
title: Marketo-Plug-in-Versionen für Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 492a43045bdf77243e4600eeb2223e750a35859b
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Marketo-Plug-in-Versionen für Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Bei der ersten Synchronisierung mit Microsoft Dynamics laden Sie die neueste Version der Plug-ins für Marketo herunter. Marketo aktualisiert diese Plug-ins regelmäßig, sodass Sie zum selben Ort zurückkehren können, um die neue Version herunterzuladen.

[Herunterladen des neuesten Plug-ins](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} entspricht Ihrer Dynamics-Version.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Aktualisieren Ihrer Dynamics-Lösung {#updating-your-dynamics-solution}

1. Importieren Sie die neueste Version der Lösung über die vorhandene Version Ihres Dynamics CRM (z. B. wenn Ihr Dynamics CRM-System über Version 1.4 verfügt und die neueste Version 1.5 ist), importieren Sie _over_ Version 1.4).

1. Das folgende Popup wird angezeigt. Auswählen **Aktualisieren** und **Verwalten von Anpassungen** Klicken Sie auf **Import**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Neueste Versionen {#latest-versions}

>[!NOTE]
>
>Diese Versionen funktionieren sowohl für On-Premise- als auch für Online-Versionen von Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th>Version</th> 
   <th>Veröffentlichungsdatum</th> 
   <th>Hinweise</th> 
  </tr>
  <tr> 
   <td>5,0,2,1</td> 
   <td>13.10.23</td> 
   <td>Fehlerbehebung: Es wurden Fehler im Zusammenhang mit der Synchronisierung benutzerdefinierter Entitäten behoben.</td> 
  </tr> 
  <tr> 
   <td>5,0,2,0</td> 
   <td>24.03.23</td> 
   <td>Fehlerbehebung: Es wurden Fehler behoben, die das Zusammenführen von Kontakten in MS Dynamics verhinderten.</td> 
  </tr> 
  <tr> 
   <td>5,0,1,8</td> 
   <td>27.03.23</td> 
   <td>Fehlerbehebung: Verhindert, dass das Plug-in andere Anpassungen an den UI-Elementen in MS Dynamics überschrieben hat.</td> 
  </tr> 
  <tr> 
   <td>5,0,1,1</td> 
   <td>04.02.21</td> 
   <td>Unterstützung für die Synchronisation von Mehrfachauswahl-optionalen Feldern (diese Funktion ist nur für V9.X und höher verfügbar).</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>16.10.20</td> 
   <td>Unterstützung für die Kampagnensynchronisierung mit MS Dynamics hinzugefügt.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>22.08.18</td> 
   <td>Unterstützung für vordefinierten Qualifizierungs-Lead-Kontaktprozess für Microsoft Dynamics Version 9.x hinzugefügt.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>27.06.18</td> 
   <td>Fehlerbehebung: Business Process Error beim Versuch, Marketo Solutions for Dynamics 2013 zu installieren.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>29.09.17</td> 
   <td>Fehlerbehebung: Interne Revision.</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>09.11.16</td> 
   <td>Fehlerbehebung: Das Plug-in hat keine Ereignisse abonniert, die die Statusänderung des benutzerdefinierten Objekts erfassen. Diese Fehlerbehebung betrifft Dynamics CRM On Premise 2011.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>22.07.16</td> 
   <td>Fehlerbehebung: Aktualisierungen der Kontaktrolle "Chancen" wurden nicht vollständig erfasst.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>28.06.16</td> 
   <td>Fehlerbehebung: Bei der Erstellung der Gelegenheit wurde eine unnötige Aktualisierungstransaktion für die Kundenopportunitätsrolle im Marketo-Protokoll vermerkt.<p>Fehlerbehebung: Beim Löschen der Entität "customeropportunityrole"wurde eine zusätzliche Löschtransaktion protokolliert.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>31.05.16</td> 
   <td>Fehlerbehebung: Benutzerdefinierte Objekte wurden asynchron aktualisiert und gelöscht.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>08.04.16</td> 
   <td>Fehlerbehebung: Wenn der Lead einen Synchronisierungsfilter auf "NO"gesetzt hatte und die Opportunity und der Kontakt keinen Synchronisierungsfilter hatten, wurde das Protokoll erstellen nicht für den Kontakt und die Gelegenheit generiert, wenn der Lead qualifiziert wurde.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>29.03.16</td> 
   <td>Fehlerbehebung: Ein Zuweisungsereignis wurde protokolliert, wenn der Synchronisierungsfilter deaktiviert war.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>03.03.16</td> 
   <td>Fehlerbehebung: Der Kunde konnte keinen Lead in CRM erstellen, da der Anmeldename nicht über die Berechtigung Marketo-Konfiguration verfügte.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.14</td> 
   <td>18.01.16</td> 
   <td>Fehlerbehebung: Es wurden Zugriffsbeschränkungen für normale Dynamics-Benutzer erstellt, um Sicherheitsbedenken auszuräumen.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>30.12.15</td> 
   <td>Fehlerbehebung: Aktualisierungen in Dynamics wurden nicht mit Marketo für Schritte und Bilder synchronisiert.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>12.11.15</td> 
   <td>Fehlerbehebung: Lead-Datensätze wurden mit Marketo synchronisiert, wenn der Synchronisierungsfilter auf "false"festgelegt war.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Marketo-Lead-Management-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
