---
description: Eine Marketing-Kampagne in der Benutzeroberfläche „Sales Insight-Aktionen“ sichtbar machen - Marketo-Dokumente - Produktdokumentation
title: Marketing-Kampagnen in der Benutzeroberfläche „Sales Insight-Aktionen“ anzeigen
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: b037057cb37c830760a5d5bc24591f85ad306ae8
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Marketing-Kampagnen in der Benutzeroberfläche „Sales Insight-Aktionen“ anzeigen {#make-a-marketing-campaign-visible-in-the-sales-insight-actions-ui}

Kampagnen können nur freigegeben werden, wenn sie sichtbar gemacht werden.

Mit Sales Insight-Aktionen haben Benutzer Zugriff auf eine neue Verkaufs-App namens toutapp.com. Diese App bietet neue Aktionsfunktionen, übernimmt aber auch die Funktion _Zu Marketing-Kampagne hinzufügen_, die in der Kernversion von Sales Insights verfügbar ist. Dies sollten Sie beachten, da Ihre Marketo-Kampagnen je nachdem, wo Benutzerinnen und Benutzer auf die Funktion Zu Marketing-Kampagne hinzufügen zugreifen sollen (toutapp.com oder das MSI SFDC-Paketerlebnis), anders konfiguriert werden müssen. Weitere Informationen finden Sie im Hinweis in Schritt 4 .

1. Wählen (oder erstellen) Sie die Kampagne, die Sie freigeben möchten.

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. Klicken Sie auf **Registerkarte** Smart-Liste“.

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. Fügen Sie den Trigger Kampagne wird angefordert hinzu.

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. Wählen Sie für die Quelle „is“ **Webservice-API**.

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >Wenn Sie die Marketing-Kampagne Benutzern anzeigen möchten, die _Zur Marketing-Kampagne hinzufügen_ aus der Web-Anwendung toutapp.com verwenden (dies gilt auch, wenn die Web-Anwendung über das Marketo-Verkaufs-Postausgangsobjekt in das CRM eingebettet ist), setzen Sie sie auf „Web-Service-API“. Wenn die Marketing-Kampagne angezeigt werden soll, wenn Benutzende die Aktionen des MSI-Bedienfelds in Salesforce für den Lead, den Kontakt, die Kontoseite oder die Massenaktionsschaltflächen in den Lead- und Kontaktlistenansichten verwenden, aktualisieren Sie sie auf „Verkaufsinsights“

1. Klicken Sie auf **Registerkarte** Fluss“.

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. Fügen Sie die Aktion Interessanter Momentfluss hinzu.

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. Wählen Sie für Typ die Option **Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. Schreiben Sie im Feld Beschreibung eine Nachricht an Ihr Vertriebsteam. In diesem Beispiel verwenden wir Token, um das ausgefüllte Formular anzugeben.

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. Klicken Sie auf **Registerkarte** und **Aktivieren** die Kampagne.

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
