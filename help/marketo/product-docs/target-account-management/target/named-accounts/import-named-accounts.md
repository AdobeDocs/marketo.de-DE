---
unique-page-id: 12615800
description: Importieren [!UICONTROL benannten Konten] - Marketo-Dokumente - Produktdokumentation
title: Importieren [!UICONTROL benannte Konten]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Importieren [!UICONTROL benannte Konten] {#import-named-accounts}

Haben Sie bereits eine CSV voller potenzieller Zielkonten? Importieren Sie sie direkt in TAM!

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Benannte Konten importieren]**.

   ![](assets/inaone.png)

1. Ein neues Fenster wird geöffnet. Klicken Sie **[!UICONTROL Durchsuchen]** und wählen Sie dann die Datei mit den benannten Konten aus, die Sie importieren möchten.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Geben Sie in Ihrer Datei [so viele Informationen](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) wie möglich an. Sie können nur firmografische Informationen hinzufügen. Marketo berechnet nichts (d. h. Pipeline). Um benannte Konten auf der Grundlage von CRM-Konten zu erstellen, exportieren Sie einfach den Kontonamen und die CRM-ID aus Ihrem CRM in eine CSV-Datei, verwenden Sie die Option Kontoname und ordnen Sie die CRM-ID während des Importvorgangs zu. Um ein CRM-Konto ordnungsgemäß mit einem benannten Konto zu verknüpfen, müssen Sie den genauen Namen des CRM-Kontos angeben.

1. Wählen Sie aus zwei Deduplizierungsmodi: Kontoname oder Domain-Name. In diesem Beispiel wählen wir Konto. Klicken Sie auf **[!UICONTROL Modi]** und wählen Sie **[!UICONTROL Nach Kontoname]** aus.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Wenn Sie **[!UICONTROL Nach Domain-Name]** auswählen, müssen sowohl das Feld „Benanntes Konto“ als auch das Feld „Domain“ einbezogen werden.

1. Um auszuwählen, welcher Kontoliste Ihr benanntes Konto hinzugefügt wird, klicken Sie auf die **[!UICONTROL Kontoliste]** und wählen Sie diese aus.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Sie können auch eine brandneue [!UICONTROL Kontoliste“ erstellen] indem Sie einfach ihren Namen in die Dropdown-Liste eingeben.

1. Um eine Benachrichtigung über den Import zu senden, klicken Sie auf die **[!UICONTROL Warnhinweis senden an]** und wählen Sie einen Marketo-Benutzer aus. E _Mail-Adresse kann_ manuell eingegeben werden.

   ![](assets/inafive-2.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/inasix-2.png)

1. Ordnen Sie jedes Feld zu, indem Sie auf die Dropdown-Liste **[!UICONTROL Marketo]** doppelklicken und das entsprechende Feld auswählen. Klicken Sie abschließend **[!UICONTROL Weiter]**.

   ![](assets/inaseven.png)

   Erfolg!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >„Importstatus überprüfen“ zeigt nur die letzten drei Tage der Aktivität an.

Szenarien bei der Deduplizierung [!UICONTROL nach Kontoname]:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Datensatz mit vorhandenem Namen <span class="uicontrol">Benanntes Konto</span> importieren</strong></td> 
   <td><p>Der vorhandene Datensatz wird aktualisiert.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Datensatz mit neuem Namen <span class="uicontrol">Benanntes Konto</span> wird importiert</strong></td> 
   <td>Wir werden einen neuen Datensatz erstellen</td> 
  </tr> 
 </tbody> 
</table>

Szenarien bei der Deduplizierung [!UICONTROL nach Domain-Name]:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importieren eines Datensatzes mit einem neuen Kontonamen und einem neuen Domain-Namen</strong></td> 
   <td>Wir erstellen ein neues <span class="uicontrol">Benanntes Konto</span> mit den angegebenen Informationen</td> 
  </tr> 
  <tr> 
   <td><strong>Importieren eines Datensatzes mit einem vorhandenen Kontonamen und einem vorhandenen Domain-Namen</strong></td> 
   <td>Wir werden das vorhandene <span class="uicontrol">Benannte Konto</span> aktualisieren</td> 
  </tr> 
   <tr> 
   <td><strong>Importieren eines Datensatzes mit einem neuen Kontonamen und einem vorhandenen Domain-Namen</strong></td> 
   <td>Wir hängen den neuen Kontonamen an das vorhandene <span class="uicontrol">Benannte Konto</span> an, das mit dem Domain-Namen übereinstimmt, und aktualisieren andere Informationen (z. B. Branche, Bundesland usw.)</td> 
  </tr> 
  <tr> 
   <td><strong>Datensatz mit vorhandenem Namen <span class="uicontrol">Benanntes Konto</span> und neuem Domain-Namen wird importiert</strong></td> 
   <td>Wir hängen den neuen Domain-Namen an das vorhandene <span class="uicontrol">Benanntes Konto</span> an, das mit dem Kontonamen übereinstimmt, und aktualisieren andere Informationen (z. B. Branche, Bundesland usw.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn Marketo ein benanntes Konto anhängt, aktualisieren wir eine Regel (hinter den Kulissen), mit der wir Personen identifizieren können, die Teil des [!UICONTROL benannten Kontos“ sein &#x200B;]. Beispiel: Wenn Sie &quot;IBM&quot; in &quot;IBM, USA“ aktualisieren, werden Personen mit einem der Firmennamen mit dem &quot;[!UICONTROL &#x200B; Konto“ &#x200B;].

Wenn Marketo Datensätze findet, die wir als Duplikate sehen, wird nur der erste verarbeitet.
