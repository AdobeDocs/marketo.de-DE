---
unique-page-id: 10099389
description: Marketo-Plug-in-Versionen für [!DNL Microsoft Dynamics] - Marketo-Dokumente - Produktdokumentation
title: Marketo-Plug-in-Versionen für [!DNL Microsoft Dynamics]
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Marketo-Plug-in-Versionen für [!DNL Microsoft Dynamics] {#marketo-plugin-releases-for-microsoft-dynamics}

Beim ersten Synchronisieren mit [!DNL Microsoft Dynamics] laden Sie die neueste Version der Plug-ins für Marketo herunter. Marketo aktualisiert diese Plug-ins regelmäßig, damit Sie zum Download der neuen Version an denselben Ort zurückkehren können.

[Laden Sie das neueste Plug-](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) herunter, das Ihrer [!DNL Dynamics] Version entspricht.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Aktualisieren der [!DNL Dynamics] {#updating-your-dynamics-solution}

1. Importieren Sie die neueste Version der Lösung über die vorhandene Version Ihres [!DNL Dynamics] CRM (z. B.: Wenn Ihr [!DNL Dynamics] CRM über Version 1.4 verfügt und die neueste Version 1.5 ist, würden Sie _über_ Version 1.4) importieren.

1. Daraufhin wird das folgende Popup angezeigt. Wählen Sie **Aktualisieren** und **Anpassungen beibehalten** und klicken Sie dann auf **Importieren**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Neueste Versionen {#latest-versions}

>[!NOTE]
>
>Diese Versionen funktionieren sowohl für On-Premise- als auch für Online-Versionen von [!DNL Dynamics].

<table>
 <tbody>
  <tr>
   <th style="width:15%">Version</th>
   <th style="width:20%">Veröffentlichungsdatum</th>
   <th style="width:65%">Hinweise</th>
  </tr>
  <tr>
   <td>5.0.2.1</td>
   <td>1/19/24</td>
   <td>Fehlerbehebung: Es wurden Fehler im Zusammenhang mit der Synchronisierung benutzerdefinierter Entitäten behoben.</td>
  </tr>
  <tr>
   <td>5.0.2.0</td>
   <td>03/24/23</td>
   <td>Fehlerbehebung: Fehler behoben, die das Zusammenführen von Kontakten in MS Dynamics verhindert haben.</td>
  </tr>
  <tr>
   <td colspan="1">4.2.0.0</td>
   <td colspan="1">10/16/20</td>
   <td colspan="1">Es wurde Unterstützung für die Kampagnensynchronisierung mit MS [!DNL Dynamics] hinzugefügt.</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.24</td>
   <td colspan="1">8/22/18</td>
   <td colspan="1">Hinzugefügte Unterstützung für vorkonfigurierten qualifizierten Lead-zu-Kontakt-Prozess für [!DNL Microsoft Dynamics] Version 9.x.</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.23</td>
   <td colspan="1">6/27/18</td>
   <td colspan="1">Fehlerbehebung: Geschäftsprozess-Fehler bei der Installation der Marketo-Lösungen für [!DNL Dynamics] 2013.</td>
  </tr>
  <tr>
   <td>4.0.0.24</td>
   <td>8/22/18</td>
   <td>Unterstützung für vorkonfigurierten qualifizierten Lead-zu-Kontakt-Prozess für Microsoft Dynamics Version 9.x wurde hinzugefügt.</td>
  </tr>
  <tr>
   <td colspan="1"><p>4.0.0.21</p></td>
   <td colspan="1">11/9/16</td>
   <td colspan="1">Fehlerbehebung: Das Plug-in hat keine Ereignisse abonniert, die die Statusänderung des benutzerdefinierten Objekts erfassen. Diese Fehlerbehebung gilt speziell für [!DNL Dynamics] CRM On-Premise 2011. </td>
  </tr>
  <tr>
   <td>4.0.0.22</td>
   <td>9/29/17</td>
   <td>Fehlerbehebung: Interne Revision.</td>
  </tr>
  <tr>
   <td><p>4.0.0.21</p></td>
   <td>11/9/16</td>
   <td>Fehlerbehebung: Das Plug-in hat keine Ereignisse abonniert, die die Statusänderung des benutzerdefinierten Objekts erfassen. Diese Fehlerbehebung gilt speziell für Dynamics CRM On Premise 2011.</td>
  </tr>
  <tr>
   <td>4.0.0.20</td>
   <td>7/22/16</td>
   <td>Fehlerbehebung: Aktualisierungen der Rolle des Opportunity-Kontakts wurden nicht vollständig erfasst.</td>
  </tr>
  <tr>
   <td>4.0.0.19</td>
   <td>6/28/16</td>
   <td>Fehlerbehebung: Bei der Erstellung der Opportunity wurde eine unnötige Aktualisierungstransaktion für die Rolle customerOpportunity im Marketo-Protokoll vermerkt.<p>Fehlerbehebung: Beim Löschen der Entität „Rolle des Kunden“ wurde eine zusätzliche Löschtransaktion protokolliert.</td>
  </tr>
  <tr>
   <td>4.0.0.18</td>
   <td>5/31/16</td>
   <td>Fehlerbehebung: Aktualisierung und Löschen von benutzerdefinierten Objekten wurden asynchron durchgeführt.</td>
  </tr>
  <tr>
   <td>4.0.0.17</td>
   <td>4/8/16</td>
   <td>Fehlerbehebung: Wenn für den Lead ein Synchronisierungsfilter auf „NEIN“ festgelegt war und die Opportunity und der Kontakt keinen Synchronisierungsfilter hatten, wurde das Erstellungsprotokoll nicht für den Kontakt und die Opportunity generiert, wenn der Lead qualifiziert wurde.</td>
  </tr>
  <tr>
   <td>4.0.0.16</td>
   <td>3/29/16</td>
   <td>Fehlerbehebung: Ein „Ereignis zuweisen“ wurde protokolliert, wenn der Synchronisierungsfilter deaktiviert wurde.</td>
  </tr>
  <tr>
   <td>4.0.0.15</td>
   <td>3/3/16</td>
   <td>Fehlerbehebung: Der Kunde konnte keinen Lead im CRM erstellen, da der angemeldete Benutzer keine Berechtigung zur Marketo-Konfiguration hatte.</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.14</td>
   <td colspan="1">1/18/16</td>
   <td colspan="1">Fehlerbehebung: Es wurden Zugriffsbeschränkungen für normale Benutzende von [!DNL Dynamics] erstellt, um Sicherheitsbedenken auszuräumen.</td>
  </tr>
  <tr>
   <td colspan="1">4.0.0.13</td>
   <td colspan="1">12/30/15</td>
   <td>Fehlerbehebung: Updates in [!DNL Dynamics] wurden für Schritte und Bilder nicht mit Marketo synchronisiert.</td>
  </tr>
  <tr>
   <td>4.0.0.12</td>
   <td>11/12/15</td>
   <td>Fehlerbehebung: Lead-Datensätze wurden mit Marketo synchronisiert, wenn der Synchronisierungsfilter auf „false“ eingestellt war.</td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Marketo Lead Management-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
