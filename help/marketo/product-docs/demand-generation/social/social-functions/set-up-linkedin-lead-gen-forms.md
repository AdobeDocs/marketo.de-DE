---
unique-page-id: 12976798
description: Einrichten von LinkedIn Lead Gen Forms - Marketing Docs - Produktdokumentation
title: Einrichten von LinkedIn Lead Gen Forms
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Einrichten von LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Verwenden Sie LinkedIn Lead Gen Forms, um Anzeigen-Kampagnen in LinkedIn auszuführen und Interessenten für Marketing zu generieren.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Gehen Sie zu Marketing **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gehen Sie zu **LaunchPoint**, klicken Sie auf **New** und wählen Sie **New Service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigenamen** für Ihren Dienst ein, wählen Sie in der Dropdown-Liste den Dienst **LinkedIn Lead Gen **und klicken Sie auf **Weiter**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo öffnet im selben Browser eine neue Registerkarte für [www.linkedin.com](http://www.linkedin.com). Melden Sie sich bei LinkedIn mit dem Konto an, das Sie für die Integration verwenden möchten.

   >[!NOTE]
   >
   >Das LinkedIn-Konto benötigt Zugriff auf alle LinkedIn-Geschäftskonten, für die Sie gesponserte Kampagnen erstellen.

   ![](assets/linkedin-login.png)

1. Nachdem Sie bei LinkedIn angemeldet sind, kehren Sie zu Marketo zurück und klicken Sie auf **Autorisieren**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Klicken Sie bei Aufforderung auf **Zulassen **um die Installation der Marketing-App in LinkedIn zu akzeptieren.

   ![](assets/linkedin-marketo-allow.png)

1. Sie werden feststellen, dass Sie jetzt autorisiert sind. Klicken Sie auf **Weiter**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Der Dienst läuft automatisch ein Jahr nach der Autorisierung ab. Um den Zugriff wiederherzustellen, klicken Sie einfach auf **Erneut autorisieren**. Je nach Browsereinstellungen müssen Sie eventuell Ihr LinkedIn-Kennwort erneut eingeben.

1. Wählen Sie das Konto/die Konten aus, von dem/denen die LinkedIn-Lead-Gen-Interessenten nach Marketo gelangen sollen, und klicken Sie auf **Weiter**.

   >[!TIP]
   >
   >Wenn Ihnen die von Ihnen erwarteten Geschäftskonten nicht angezeigt werden, stellen Sie sicher, dass für das autorisierte LinkedIn-Konto des Benutzers die Berechtigung &quot;Lead Gen Form Manager&quot;für das Geschäftskonto in LinkedIn erteilt wurde.

   ![](assets/linkedin-pages-to-capture.png)

1. Um standardmäßige Feldzuordnungen von LinkedIn zu Marketo zu akzeptieren, klicken Sie einfach auf **Erstellen**. Wenn Sie die Standardfeldzuordnung ändern, eine Feldzuordnung entfernen oder eine neue Feldzuordnung hinzufügen möchten, können Sie dies per Modal unten pro Feld tun.

   >[!CAUTION]
   >
   >Marketo unterstützt die Zuordnung von zwei LinkedIn-Feldern zu einem einzelnen Marker-Feld, **jedoch nur, wenn** sich die beiden LinkedIn-Felder nicht im selben Formular befinden. Wenn Sie zwei Felder aus demselben LinkedIn-Formular einem einzigen Feld &quot;Marketo&quot;zuordnen, wird der Zugriff auf Ihre Marketing-Datenbank eventuell fehlschlagen.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Nur LinkedIn-Felder, die bereits in einer [Formularvorlage](https://www.linkedin.com/help/lms/answer/79634) im LinkedIn-Kampagnen-Manager gespeichert wurden, werden als LinkedIn-Felder angezeigt, die Marketo-Feldern zugeordnet werden können.

   ![](assets/linkedin-installed-services.png)

Gut gemacht! Personen, die LinkedIn-Lead-Gen-Formulare senden, fließen beim Ausführen erfolgreicher Kampagnen auf der LinkedIn-Seite in den Beginn, der nach Marketo fließt.

>[!NOTE]
>
>Sie können nur ein einziges LinkedIn-Benutzerkonto autorisieren. Wenn Sie über mehrere Geschäftskonten verfügen, die Sie mit Marketo verknüpfen möchten, stellen Sie sicher, dass für das autorisierte LinkedIn-Konto des Benutzers die Berechtigung &quot;Lead Gen Form Manager&quot;für das Geschäftskonto in LinkedIn aktiviert ist.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Verwenden Sie die Filter und Auslöser von LinkedIn-Lead-Gen-Formularen in einer intelligenten Kampagne](use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)

>



