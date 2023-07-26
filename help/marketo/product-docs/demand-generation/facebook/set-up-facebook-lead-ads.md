---
unique-page-id: 11379622
description: Einrichten von Facebook-Lead-Anzeigen - Marketo-Dokumente - Produktdokumentation
title: Einrichten von Facebook-Lead-Anzeigen
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Einrichten von Facebook-Lead-Anzeigen {#set-up-facebook-lead-ads}

Verwendung [Facebook Lead Ads](https://www.facebook.com/business/a/lead-ads) , um Anzeigenkampagnen in Facebook auszuführen und Leads für Marketo zu generieren.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!AVAILABILITY]
>
>Wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer), um Facebook Lead Ads zu Ihrer Instanz hinzuzufügen.

1. Navigieren zu Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Navigieren Sie zu **LaunchPoint**, klicken Sie auf **Neu,** und wählen **Neuer Dienst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigename** Wählen Sie für Ihren Dienst die **Facebook Lead Ads** Dienst aus der Dropdown-Liste aus und klicken Sie auf **Erstellen**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Öffnen Sie eine neue Registerkarte im selben Browser und navigieren Sie zu [facebook.com](https://www.facebook.com). Melden Sie sich mit dem Konto, das Sie für die Integration verwenden möchten, bei Facebook an.

   >[!NOTE]
   >
   >Das Facebook-Konto benötigt Zugriff auf alle Facebook-Geschäftsseiten, von denen Sie Lead-Anzeigen abrufen möchten.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Nachdem Sie sich bei Facebook angemeldet haben, kehren Sie zu Marketo zurück und klicken Sie auf **Autorisieren**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Klicken Sie bei entsprechender Aufforderung auf **OK** , um die Installation der Marketo-App in Facebook zu akzeptieren.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du wirst feststellen, dass du jetzt autorisiert bist. Klicks **Nächste**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Wählen Sie die Seiten aus, von denen Marketo Lead-Anzeigen von Facebook abrufen soll, und klicken Sie auf **Nächste**.

   >[!TIP]
   >
   >Wenn keine Seite angezeigt wird, die Sie erwarten, stellen Sie sicher, dass das für die Authentifizierung verwendete Facebook-Konto der Seite in Facebook hinzugefügt wird, und versuchen Sie es erneut.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Um die standardmäßigen Facebook- zu Marketo-Feldzuordnungen zu akzeptieren, klicken Sie einfach auf **Erstellen**.

   >[!TIP]
   >
   >Durch Änderung der Zuordnungen können Sie anpassen, wo die Lead-Anzeigendaten in Marketo gespeichert sind. Sie können auch [Daten aus benutzerdefinierten Fragen zu Lead-Anzeigen abrufen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo unterstützt nicht die Zuordnung von zwei Facebook-Feldern zu einem Marketo-Feld, sondern nur 1 zu 1. Wenn Sie Zuordnung 2 zu 1 vornehmen, können Leads möglicherweise nicht in das Marketo-System gelangen.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   Schön gemacht! Leads fließen in Marketo über erfolgreiche Facebook Lead Ad-Kampagnen.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Berechtigungen in Leads Access Manager (Facebook) zuweisen/entfernen](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Verwenden von Lead-Anzeigenfiltern und -Triggern in einer Smart-Kampagne](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Benutzerdefinierte Felder Marketo zuordnen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)
