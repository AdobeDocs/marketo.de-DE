---
unique-page-id: 12615800
description: Benannte Konten importieren - Marketing-Dokumente - Produktdokumentation
title: Benannte Konten importieren
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---


# Benannte Konten importieren {#import-named-accounts}

Sie haben bereits eine CSV voll von potenziellen Zielgruppen Konten? Importieren Sie sie direkt in ABM!

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Benannte Konten** importieren.

   ![](assets/inaone.png)

1. Daraufhin wird ein neues Fenster geöffnet. Klicken Sie auf **Durchsuchen** und wählen Sie dann die Datei mit den benannten Konten aus, die Sie importieren möchten.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Geben Sie in Ihrer Datei [so viele Informationen](http://docs.marketo.com/display/DOCS/Named+Account+Overview#NamedAccountOverview-NamedAccountAttributes) wie möglich ein. Sie können nur firmografische Informationen hinzufügen. Keine Berechnung von Marketo (d.h. Pipeline). Um benannte Konten basierend auf CRM-Konten zu erstellen, exportieren Sie einfach den Kontonamen und die CRM-ID aus Ihrem CRM-System in eine CSV-Datei, verwenden Sie die Option Kontoname und ordnen Sie die CRM-ID während des Importvorgangs zu. Um ein CRM-Konto ordnungsgemäß mit einem benannten Konto zu verknüpfen, müssen Sie den genauen Namen des CRM-Kontos angeben.

1. Wählen Sie aus zwei Deduplizierungsmodi: Kontoname oder Domänenname. In diesem Beispiel wählen wir Konto. Klicken Sie auf die Dropdownliste **Modi** und wählen Sie **Nach Kontoname**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Wenn Sie &quot; **Nach Domänenmodus**&quot;wählen, müssen sowohl die Felder &quot;Benanntes Konto&quot;als auch &quot;Domäne&quot;einbezogen werden.

1. Klicken Sie zur Auswahl der Liste, zu der Ihr benanntes Konto hinzugefügt wird, auf die Dropdownliste **Kontoeinstellungen** , und wählen Sie aus.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Sie können auch eine ganz neue Account-Liste erstellen, indem Sie einfach ihren Namen in das Dropdown-Feld eingeben.

1. Um eine Benachrichtigung über den Import zu senden, klicken Sie auf die Dropdownliste Warnung **senden an** und wählen Sie einen Benutzer aus. Sie *können* keine E-Mail-Adresse manuell eingeben.

   ![](assets/inafive-2.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/inasix-2.png)

1. Ordnen Sie die einzelnen Felder zu, indem Sie mit der Dublette auf die Dropdown-Liste &quot; **Feld** markieren&quot;klicken und das entsprechende Feld auswählen. Klicken Sie abschließend auf **Weiter** .

   ![](assets/inaseven.png)

   Erfolg!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Importstatus überprüfen&quot;zeigt nur die letzten drei Tage der Aktivität an.

<table> 
 <tbody> 
  <tr> 
   <td>Importieren von Datensätzen mit vorhandenem Namen des benannten Kontos</td> 
   <td><p>Wir werden den vorhandenen Datensatz aktualisieren</p></td> 
  </tr> 
  <tr> 
   <td>Importieren von Datensätzen mit dem neuen Namen des benannten Kontos</td> 
   <td>Wir werden einen neuen Datensatz erstellen</td> 
  </tr> 
 </tbody> 
</table>

Szenarien, in denen Sie nach Domänennamen deduplizieren:

| **Importieren von Datensätzen mit einem neuen Kontonamen und einem neuen Domänennamen** | Wir erstellen ein neues benanntes Konto mit den bereitgestellten Informationen |
|---|---|
| **Importieren von Datensätzen mit einem vorhandenen Kontonamen und einem vorhandenen Domänennamen** | Wir werden das vorhandene benannte Konto aktualisieren |
| **Importieren von Datensätzen mit einem neuen Kontonamen und einem vorhandenen Domänennamen** | Wir hängen den neuen Kontonamen an das vorhandene benannte Konto an, das mit dem Domänennamen übereinstimmt, und aktualisieren andere Informationen (z.B. Industrie, Staat usw.) |
| **Importieren von Datensätzen mit vorhandenem Namen des benannten Kontos und neuem Domänennamen** | Wir hängen den neuen Domänennamen an das vorhandene benannte Konto an, das mit dem Kontonamen übereinstimmt, und aktualisieren andere Informationen (z.B. Industrie, Staat usw.) |

>[!NOTE]
>
>Wenn Marketo ein benanntes Konto anhängt, aktualisieren wir eine Regel (hinter den Kulissen), die es uns ermöglicht, Personen zu identifizieren, die Teil des benannten Kontos sein sollten. Beispiel: Wenn Sie &quot;IBM&quot;auf &quot;IBM, USA&quot;aktualisieren, werden Personen mit beiden Firmen mit dem benannten Konto verknüpft.

Wenn Marketo Datensätze findet, die wir als Duplikate ansehen, werden wir nur das erste verarbeiten.

Szenarien, in denen Sie nach Kontoname deduplizieren: