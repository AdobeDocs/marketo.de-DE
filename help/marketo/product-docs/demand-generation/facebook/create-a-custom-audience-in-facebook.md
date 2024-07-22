---
unique-page-id: 4720275
description: Erstellen einer benutzerdefinierten Zielgruppe in Facebook - Marketo Docs - Produktdokumentation
title: Erstellen einer benutzerdefinierten Zielgruppe in Facebook
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Erstellen einer benutzerdefinierten Zielgruppe in Facebook {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [Fügen Sie benutzerdefinierte Facebook-Zielgruppen als LaunchPoint-Dienst hinzu](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} im Admin-Abschnitt.
>* [Akzeptieren Sie die benutzerdefinierten Zielgruppenbegriffe von Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} in Ihrem Facebook-Konto.

>[!TIP]
>
>Erfahren Sie mehr über [benutzerdefinierte Zielgruppen in Facebook](https://www.facebook.com/help/341425252616329){target="_blank"}.

1. Suchen und wählen Sie die Smart- oder statische Liste mit den Leads aus, aus denen Sie die Zielgruppe erstellen möchten.

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. Wählen Sie die Registerkarte **Leads** aus und klicken Sie dann unten auf das Symbol **Via Ad Bridge senden** .

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. Wählen Sie **Facebook** und klicken Sie auf **Weiter**.

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. Klicken Sie auf die Dropdownliste **Zielgruppe** und wählen Sie **+ Neue Zielgruppe** aus.

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >Die Facebook-API ermöglicht bis zu 500 benutzerdefinierte Zielgruppen pro Facebook-Anzeigenkonto.

1. Geben Sie einen **Zielgruppennamen** ein. Klicken Sie auf **Aktualisieren**.

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >Wenn Sie über mehrere Facebook-Anzeigenkonten verfügen, wird eine zusätzliche Dropdown-Liste angezeigt, in der Sie auswählen können, in welchem Anzeigenkonto diese Zielgruppe erstellt wird.

   >[!TIP]
   >
   >Möchten Sie eine neue Zielgruppe mit einer vorhandenen austauschen, die aktuell mit einem Anzeigenset oder einer Anzeigengruppe verknüpft ist? Aktivieren Sie das Kontrollkästchen **Vorhandene Audience ersetzen** . Dadurch wird die ersetzte Audience **nicht** gelöscht.

1. Nach Abschluss des Vorgangs wird das Statusdialogfeld aktualisiert.

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   Und das ist es! In Facebook wird die neue Zielgruppe unter **Anzeigen-Manager** > **Zielgruppen** angezeigt.

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >Alle Listen, die Sie an Facebook übergeben, werden statisch. Smart-Listen in Marketo aktualisieren die Zielgruppenliste in Facebook nicht automatisch, um Änderungen widerzuspiegeln, die nach der Übertragung vorgenommen wurden.

   >[!TIP]
   >
   >Siehe [Facebook-Lernpfad für Marketo-Kunden](https://facebook.exceedlms.com/student/enrollments/create_enrollment_from_token/BF9TqSaCvM73PP4ScjhCm4fi){target="_blank"}. Es behandelt alles, was Sie wissen müssen, von der Erstellung einer Facebook-Seite bis hin zur Ausrichtung Ihrer Facebook-Anzeigen mithilfe der Werbenetzwerk-Integrationen von Marketo.

   >[!MORELIKETHIS]
   >
   >[Hinzufügen von Leads zu einer benutzerdefinierten Zielgruppe in Facebook](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
