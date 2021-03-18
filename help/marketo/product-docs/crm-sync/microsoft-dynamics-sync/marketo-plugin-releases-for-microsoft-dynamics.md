---
unique-page-id: 10099389
description: Marketo Plugin Releases for Microsoft Dynamics - Marketing Docs - Produktdokumentation
title: Marketo Plugin Releases for Microsoft Dynamics
translation-type: tm+mt
source-git-commit: d1d74e24c07578b1b0c2696c08fe5a5be543cce8
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 6%

---


# Marketo Plugin Releases for Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Beim ersten Synchronisieren mit Microsoft Dynamics laden Sie die neueste Version der Plugins für Marketo herunter. Marketo aktualisiert diese Plugins regelmäßig, sodass Sie zum selben Ort zurückkehren können, um die neue Version herunterzuladen.

[Laden Sie das neueste ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Plugin herunter, das Ihrem Dynamics Release entspricht.

![](assets/lead-management-solution.png)

## Aktualisieren der Dynamics Solution {#updating-your-dynamics-solution}

1. Importieren Sie die neueste Version der Lösung über die vorhandene Version Ihres Dynamics CRM (z. B.: Wenn Ihr Dynamics CRM Version 1.4 und die neueste Version 1.5 besitzt, würden Sie _over_ Version 1.4 importieren.

1. Das folgende Popup wird angezeigt. Wählen Sie **Aktualisieren** und **Anpassungen beibehalten** und klicken Sie dann auf **Importieren**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Neueste Versionen {#latest-versions}

>[!NOTE]
>
>Diese Versionen können sowohl für lokale als auch für Online-Versionen von Dynamics verwendet werden.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Version</th> 
   <th colspan="1">Releasedatum</th> 
   <th>Hinweise</th> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.0</td> 
   <td colspan="1">16.10.20</td> 
   <td colspan="1">Unterstützung für die Synchronisierung von Kampagnen mit MS Dynamics hinzugefügt.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">22.08.18</td> 
   <td colspan="1">Die Unterstützung für vordefinierte Qualifizierungen führt jetzt zum Kontaktprozess für Microsoft Dynamics Version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">27.06.18</td> 
   <td colspan="1">Fehlerbehebung: Business Process Error beim Versuch, die Marketing Solutions for Dynamics 2013 zu installieren.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">29.09.17</td> 
   <td colspan="1">Fehlerbehebung: Interne Revision.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">09.11.16</td> 
   <td colspan="1">Fehlerbehebung: Das Zusatzmodul hat keine Ereignis abonniert, die die Statusänderung des benutzerdefinierten Objekts erfassen. Diese Fehlerbehebung ist spezifisch für Dynamics CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">22.07.16</td> 
   <td colspan="1">Fehlerbehebung: Aktualisierungen der Kontaktrolle "Chancen"wurden nicht vollständig erfasst.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4,0,0,19</td> 
   <td colspan="1">28.06.16</td> 
   <td colspan="1"><p>Fehlerbehebung: Bei der Erstellung der Gelegenheit wurde eine unnötige Updatetransaktion zur Rolle "Customer Opportunity"im Marketing zur Kenntnis genommen. </p><p>Fehlerbehebung: Beim Löschen der Entität für die Kundenberechtigung wurde eine zusätzliche Löschtransaktion protokolliert.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">31.05.16</td> 
   <td colspan="1">Fehlerbehebung:  Aktualisierung und Löschen von benutzerdefinierten Objekten asynchron.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">08.04.16</td> 
   <td colspan="1">Fehlerbehebung: Wenn für den Interessenten ein Synchronisierungsfilter auf "NO"festgelegt war und die Gelegenheit und der Kontakt keinen Synchronisierungsfilter hatten, wurde das Protokoll "Erstellen"nicht für Kontakt und Gelegenheit generiert, wenn der Interessent qualifiziert war.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">29.03.16</td> 
   <td>Fehlerbehebung: Ein Assign-Ereignis wurde protokolliert, wenn der Synchronisierungsfilter deaktiviert wurde.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">03.03.16</td> 
   <td colspan="1">Fehlerbehebung: Der Kunde konnte keinen Interessenten in CRM erstellen, da der Anmeldename-Benutzer nicht über die Berechtigung "Marketing-Konfiguration"verfügte.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">18.01.16</td> 
   <td colspan="1">Fehlerbehebung: Erstellt Zugriffsbeschränkungen für normale Dynamics Benutzer, um Sicherheitsbedenken auszuräumen.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">30.12.15</td> 
   <td>Fehlerbehebung: Aktualisierungen in Dynamics wurden nicht mit Marketo synchronisiert, um Schritte und Bilder zu erhalten.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">12.11.15</td> 
   <td colspan="1">Fehlerbehebung: Interessentendatensätze wurden mit Marketo synchronisiert, wenn der Synchronisierungsfilter auf "false"festgelegt war.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Laden Sie die Marketing-Interessentenverwaltungslösung herunter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
