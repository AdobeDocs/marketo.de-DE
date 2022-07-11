---
unique-page-id: 12980661
description: Google-Kundenabgleich als LaunchPoint-Dienst hinzufügen - Marketo Docs - Produktdokumentation
title: Google-Kundenabgleich als LaunchPoint-Dienst hinzufügen
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
source-git-commit: fb4e51a45fafaad547a641c6df5bb48cf536490d
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 2%

---

# Google-Kundenabgleich als LaunchPoint-Dienst hinzufügen {#add-google-customer-match-as-a-launchpoint-service}

Mit dieser Integration können Sie eine Marketo-Zielgruppe an Google senden, um mithilfe von Google AdWords Targeting durchzuführen und Zielgruppen in YouTube, Search und Gmail erneut anzusprechen.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Navigieren Sie zu **Admin**.

   ![](assets/admin.png)

1. Klicken **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Auswählen **Neu** then **Neuer Dienst**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. Geben Sie einen **Anzeigename** und wählen Sie **Google-Kundenabgleich** von **Diensleistung** Dropdown-Liste. Klicken Sie auf **Erstellen**.

   ![](assets/chooseservice.png)

1. Um ein Google AdWords-Konto zu verbinden, klicken Sie auf **Autorisieren**.

   ![](assets/authorizeaccount-1.png)

1. Google wird in einer neuen Registerkarte geöffnet. Melden Sie sich von hier aus bei Ihrem Google AdWords-Konto an.

   >[!CAUTION]
   >
   >Damit Marketo Zielgruppen über mehrere AdWords-Konten hinweg senden kann, muss der Google-Benutzer, den Sie in den folgenden Schritten autorisieren, Zugriff auf _all_ dieser Konten.

   ![](assets/chooseaccount.png)

1. Überprüfen Sie die angeforderten Berechtigungen und klicken Sie dann auf **Zulassen**.

   ![](assets/reviewpermissions.png)

1. Ihr Google AdWords-Konto ist jetzt mit Marketo verbunden. Klicken Sie auf **Erstellen**.

   ![](assets/authorizesuccess.png)

   Fantastisch Google Matched Audiences werden jetzt auf der Registerkarte Installierte Dienste als LaunchPoint-Dienst aufgelistet.

>[!NOTE]
>
>Die Google-Kundenabgleich-Integration kann nur ein Managers und alle Unterkonten innerhalb dieses Managers-Kontos aufnehmen. Mehrere Manager-Konten werden nicht unterstützt.
