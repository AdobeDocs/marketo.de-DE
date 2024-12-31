---
unique-page-id: 11379622
description: Einrichten von Facebook-Lead-Anzeigen - Marketo-Dokumente - Produktdokumentation
title: Einrichten von Facebook-Lead-Anzeigen
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Einrichten von Facebook-Lead-Anzeigen {#set-up-facebook-lead-ads}

Verwenden Sie [Facebook-Lead](https://www.facebook.com/business/a/lead-ads)Anzeigen, um Anzeigenkampagnen in Facebook auszuführen und Leads für Marketo zu generieren.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!AVAILABILITY]
>
>Um Facebook-Lead-Anzeigen zu Ihrer Instanz hinzufügen zu lassen, wenden Sie sich bitte an das Adobe-Account-Team (Ihren Account Manager).

1. Wechseln Sie zu Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gehen Sie zu **LaunchPoint**, klicken Sie auf **Neu** und wählen Sie **Neuer Service** aus.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigenamen** für Ihren Dienst ein, wählen Sie den **Facebook-** aus der Dropdown-Liste und klicken Sie auf **Erstellen**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Öffnen Sie eine neue Registerkarte im selben Browser und navigieren Sie zu [facebook.com](https://www.facebook.com). Melden Sie sich bei Facebook mit dem Konto an, das Sie für die Integration verwenden möchten.

   >[!NOTE]
   >
   >Das Facebook-Konto benötigt Zugriff auf alle Facebook-Geschäftsseiten, von denen Sie Lead-Anzeigen abrufen möchten.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Kehren Sie nach der Anmeldung bei Facebook zu Marketo zurück und klicken Sie auf **Autorisieren**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Klicken Sie auf **OK**, um die Installation der Marketo-App in Facebook zu akzeptieren.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Sie werden feststellen, dass Sie jetzt autorisiert sind. Klicken Sie auf **Weiter**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Wählen Sie die Seite(n) aus, von der/denen Marketo Facebook Lead-Anzeigen abrufen soll, und klicken Sie auf **Weiter**.

   >[!TIP]
   >
   >Wenn eine erwartete Seite nicht angezeigt wird, stellen Sie sicher, dass das für die Authentifizierung verwendete Facebook-Konto zur Seite in Facebook hinzugefügt wird, und versuchen Sie es erneut.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Um standardmäßige Feldzuordnungen von Facebook zu Marketo zu akzeptieren, klicken Sie einfach auf **Erstellen**.

   >[!TIP]
   >
   >Durch Ändern der Zuordnungen können Sie anpassen, wo die Lead-Anzeigen-Daten in Marketo gespeichert werden. Sie können auch [Daten aus benutzerdefinierten Fragen zu Lead-Anzeigen abrufen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo unterstützt nicht die Zuordnung von zwei Facebook-Feldern zu einem einzigen Marketo-Feld, nur 1 zu 1. Wenn Sie 2 zu 1 zuordnen, gelangen Leads möglicherweise nicht in das Marketo-System.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   Gut gemacht! Leads fließen bei der Ausführung erfolgreicher Facebook-Lead-Anzeigenkampagnen in Marketo ein.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Berechtigungen in Lead-Zugriffs-Manager (Facebook) zuweisen/entfernen](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Verwenden von Lead-Anzeigen-Filtern und -Triggern in einer Smart-Kampagne](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Zuordnen benutzerdefinierter Felder zu Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)
