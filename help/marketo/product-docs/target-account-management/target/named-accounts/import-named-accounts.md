---
unique-page-id: 12615800
description: Importieren von benannten Konten - Marketo Docs - Produktdokumentation
title: Benannte Konten importieren
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Benannte Konten importieren {#import-named-accounts}

Sie verfügen bereits über eine CSV-Datei mit allen potenziellen Zielkonten? Importieren Sie sie direkt in TAM!

1. Klicken Sie auf **Neu** und wählen Sie **Spezifische Konten importieren**.

   ![](assets/inaone.png)

1. Daraufhin wird ein neues Fenster geöffnet. Klicken **Durchsuchen** und wählen Sie dann die Datei mit den spezifischen Konten aus, die Sie importieren möchten.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Geben Sie in Ihrer Datei [Informationen](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) nach Möglichkeit. Sie können nur firmografische Informationen hinzufügen. nichts, was Marketo berechnet (d. h. Pipeline). Um spezifische, auf CRM-Konten basierende Konten zu erstellen, exportieren Sie einfach den Kontonamen und die CRM-ID aus Ihrem CRM-System in eine CSV-Datei, verwenden Sie die Option Kontoname und ordnen Sie die CRM-ID während des Importvorgangs zu. Um ein CRM-Konto ordnungsgemäß mit einem benannten Konto zu verknüpfen, müssen Sie den genauen Namen des CRM-Kontos angeben.

1. Wählen Sie aus zwei Deduplizierungsmodi: Kontoname oder Domänenname. In diesem Beispiel wählen wir Konto. Klicken Sie auf **Modi** und wählen Sie **Nach Kontoname**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Wenn Sie **Nach Domain-Modus**, müssen sowohl die Felder für das benannte Konto als auch die Domäne enthalten sein.

1. Klicken Sie auf die Schaltfläche **Kontoliste** und wählen Sie aus.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Sie können auch eine ganz neue Kontoliste erstellen, indem Sie einfach ihren Namen in das Dropdown-Feld eingeben.

1. Um eine Importbenachrichtigung zu versenden, klicken Sie auf die Schaltfläche **Warnhinweis senden an** und wählen Sie einen Marketo-Benutzer aus. You _cannot_ eine E-Mail-Adresse manuell eingeben.

   ![](assets/inafive-2.png)

1. Klicken **Nächste**.

   ![](assets/inasix-2.png)

1. Ordnen Sie jedes Feld zu, indem Sie auf die **Marketo Field** und wählen Sie das entsprechende Feld aus. Klicken **Nächste** wann geschehen.

   ![](assets/inaseven.png)

   Erfolg!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Importstatus überprüfen&quot;zeigt nur die letzten drei Aktivitätstage an.

Szenarien, in denen die Deduplizierung nach Kontoname erfolgt:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Import von Datensätzen mit vorhandenem Namen des benannten Kontos</strong></td> 
   <td><p>Wir werden den vorhandenen Datensatz aktualisieren</p></td> 
  </tr> 
  <tr> 
   <td><strong>Datensatz mit neuem Namen für ein benanntes Konto importieren</strong></td> 
   <td>Wir werden einen neuen Datensatz erstellen</td> 
  </tr> 
 </tbody> 
</table>

Szenarien, in denen die Deduplizierung nach Domänenname erfolgt:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Datensatz mit einem neuen Kontonamen und neuen Domänennamen importieren</strong></td> 
   <td>Wir erstellen ein neues benanntes Konto mit den bereitgestellten Informationen.</td> 
  </tr> 
  <tr> 
   <td><strong>Import von Datensätzen mit einem vorhandenen Kontonamen und einem vorhandenen Domänennamen</strong></td> 
   <td>Wir aktualisieren das vorhandene spezifische Konto.</td> 
  </tr> 
   <tr> 
   <td><strong>Datensatz mit einem neuen Kontonamen und einem vorhandenen Domänennamen importieren</strong></td> 
   <td>Wir hängen den neuen Kontonamen an das vorhandene benannte Konto an, das dem Domänennamen entspricht, und aktualisieren andere Informationen (z. B. Branche, Bundesland usw.)</td> 
  </tr> 
  <tr> 
   <td><strong>Datensatz mit vorhandenem Namen und neuem Domänennamen importieren</strong></td> 
   <td>Wir hängen den neuen Domänennamen an das vorhandene benannte Konto an, das dem Kontonamen entspricht, und aktualisieren andere Informationen (z. B. Branche, Bundesland usw.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn Marketo ein benanntes Konto anhängt, aktualisieren wir eine Regel (hinter den Kulissen), die es uns ermöglicht, Personen zu identifizieren, die Teil des benannten Kontos sein sollten. Beispiel: Wenn Sie &quot;IBM&quot;auf &quot;IBM, USA&quot;aktualisieren, werden Personen mit beiden Unternehmensnamen dem benannten Konto zugeordnet.

Wenn Marketo Datensätze findet, die wir als Duplikate betrachten, werden wir nur die erste verarbeiten.
