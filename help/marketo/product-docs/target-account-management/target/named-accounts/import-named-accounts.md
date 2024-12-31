---
unique-page-id: 12615800
description: Spezifische Konten importieren - Marketo-Dokumente - Produktdokumentation
title: Benannte Konten importieren
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Benannte Konten importieren {#import-named-accounts}

Haben Sie bereits eine CSV voller potenzieller Zielkonten? Importieren Sie sie direkt in TAM!

1. Klicken Sie auf **Neu** und wählen Sie **Benannte Konten importieren**.

   ![](assets/inaone.png)

1. Ein neues Fenster wird geöffnet. Klicken Sie **Durchsuchen** und wählen Sie dann die Datei mit den benannten Konten aus, die Sie importieren möchten.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Geben Sie in Ihrer Datei [so viele Informationen](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) wie möglich an. Sie können nur firmografische Informationen hinzufügen. Marketo berechnet nichts (d. h. Pipeline). Um benannte Konten auf der Grundlage von CRM-Konten zu erstellen, exportieren Sie einfach den Kontonamen und die CRM-ID aus Ihrem CRM in eine CSV-Datei, verwenden Sie die Option Kontoname und ordnen Sie die CRM-ID während des Importvorgangs zu. Um ein CRM-Konto ordnungsgemäß mit einem benannten Konto zu verknüpfen, müssen Sie den genauen Namen des CRM-Kontos angeben.

1. Wählen Sie aus zwei Deduplizierungsmodi: Kontoname oder Domain-Name. In diesem Beispiel wählen wir Konto. Klicken Sie auf **Modi** und wählen Sie **Nach Kontoname** aus.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Wenn Sie **Nach Domain-Modus** auswählen, müssen sowohl das Feld „Benanntes Konto“ als auch das Feld „Domain“ einbezogen werden.

1. Um auszuwählen, welcher Kontoliste Ihr benanntes Konto hinzugefügt wird, klicken Sie auf die **Kontoliste** und wählen Sie diese aus.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Sie können auch eine brandneue Kontoliste erstellen, indem Sie einfach ihren Namen in die Dropdown-Liste eingeben.

1. Um eine Benachrichtigung über den Import zu senden, klicken Sie auf die **Warnhinweis senden an** und wählen Sie einen Marketo-Benutzer aus. E _Mail-Adresse kann_ manuell eingegeben werden.

   ![](assets/inafive-2.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/inasix-2.png)

1. Ordnen Sie jedes Feld zu, indem Sie auf die Dropdown-Liste **Marketo** doppelklicken und das entsprechende Feld auswählen. Klicken Sie abschließend **Weiter**.

   ![](assets/inaseven.png)

   Erfolg!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >„Importstatus überprüfen“ zeigt nur die letzten drei Tage der Aktivität an.

Szenarien, in denen die Deduplizierung nach Kontoname erfolgt:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Datensatz mit vorhandenem Namen eines benannten Kontos wird importiert</strong></td> 
   <td><p>Der vorhandene Datensatz wird aktualisiert.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Datensatz mit neuem benannten Kontonamen importieren</strong></td> 
   <td>Wir werden einen neuen Datensatz erstellen</td> 
  </tr> 
 </tbody> 
</table>

Szenarien, in denen die Deduplizierung nach Domain-Namen erfolgt:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importieren eines Datensatzes mit einem neuen Kontonamen und einem neuen Domain-Namen</strong></td> 
   <td>Wir werden ein neues benanntes Konto mit den angegebenen Informationen erstellen</td> 
  </tr> 
  <tr> 
   <td><strong>Importieren eines Datensatzes mit einem vorhandenen Kontonamen und einem vorhandenen Domain-Namen</strong></td> 
   <td>Wir werden das vorhandene benannte Konto aktualisieren</td> 
  </tr> 
   <tr> 
   <td><strong>Importieren eines Datensatzes mit einem neuen Kontonamen und einem vorhandenen Domain-Namen</strong></td> 
   <td>Wir hängen den neuen Kontonamen an das vorhandene benannte Konto an, das dem Domain-Namen entspricht, und aktualisieren andere Informationen (z. B. Branche, Bundesland usw.)</td> 
  </tr> 
  <tr> 
   <td><strong>Datensatz mit vorhandenem Namen des Kontos und neuem Domain-Namen wird importiert</strong></td> 
   <td>Wir hängen den neuen Domain-Namen an das vorhandene benannte Konto an, das mit dem Kontonamen übereinstimmt, und aktualisieren andere Informationen (z. B. Branche, Bundesland usw.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn Marketo ein benanntes Konto anhängt, aktualisieren wir eine Regel (hinter den Kulissen), mit der wir Personen identifizieren können, die Teil des benannten Kontos sein sollten. Beispiel: Wenn Sie &quot;IBM&quot; in &quot;IBM, USA“ aktualisieren, werden Personen mit einem der Firmennamen mit dem benannten Konto verknüpft.

Wenn Marketo Datensätze findet, die wir als Duplikate sehen, wird nur der erste verarbeitet.
