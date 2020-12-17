---
unique-page-id: 11378713
description: Auslösen benutzerdefinierter Objektänderungen - Marketing to Docs - Produktdokumentation
title: Änderungen am benutzerdefinierten Objekt auslösen
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Auslösen benutzerdefinierter Objektänderungen {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Diese Funktion ist nur verfügbar:
>
>* Für Kunden in der Orion-Infrastruktur
>* Nur zur Verwendung mit benutzerdefinierten Objekten von Marketo, nicht mit benutzerdefinierten Objekten, die über die native Salesforce- oder Microsoft Dynamics-Integration synchronisiert werden
>* Als Auslöser, nicht als Filter

>
>
Wenden Sie sich an den [MarketingTo-Support](http://support.marketo.com), um die Auslöser für benutzerdefinierte Objektänderungen zu aktivieren.

In der intelligenten Liste einer intelligenten Kampagne können Sie eine Flussaktion auslösen, wenn einem Benutzer oder einer Firma ein benutzerdefiniertes Objekt hinzugefügt wird. Sie können auch eine intelligente Liste erstellen, die eine *change* in einem benutzerdefinierten Objekt als Auslöser verwendet. Verwenden Sie diese zum Beispiel, um eine E-Mail zu senden, wenn ein Kursname aktualisiert wird.

>[!NOTE]
>
>Beim Ändern eines benutzerdefinierten Objektdatensatzes wird kein Aktivitäten-Protokolleintrag erstellt.

1. Gehen Sie in Marketo zu **Marketing-Aktivitäten.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Erstellen oder öffnen Sie eine vorhandene intelligente Kampagne und wählen Sie die intelligente Liste aus.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Suchen Sie nach dem benötigten Auslöser und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Wählen Sie das Attribut auslösend.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Legen Sie optional eine Beschränkung fest.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Und da bist du. Die Änderung wird automatisch gespeichert.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >**Verwandte Artikel**
   >
   >    
   >    
   >    * [Erstellen einer intelligenten Liste](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >    * [Erläuterungen zu benutzerdefinierten Objekten](understanding-marketo-custom-objects.md)


