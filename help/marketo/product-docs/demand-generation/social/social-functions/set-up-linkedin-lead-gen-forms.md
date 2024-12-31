---
unique-page-id: 12976798
description: Einrichten von LinkedIn Lead Gen Forms - Marketo-Dokumente - Produktdokumentation
title: Einrichten von LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Einrichten von LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Verwenden Sie LinkedIn Lead Gen Forms , um Anzeigenkampagnen in LinkedIn auszuführen und Leads für Marketo zu generieren.

>[!IMPORTANT]
>
>LinkedIn aktualisiert seine Marketing-APIs für das Marketo Engage von LinkedIn-Integrationen. Um eine Unterbrechung des Services zu vermeiden, müssen alle LinkedIn LaunchPoint-Services zwischen dem 7 **. Juni und dem 15. Dezember 2024 erneut im Menü** Admin **> LaunchPoint** authentifiziert werden. Weitere Informationen finden Sie unter [Häufig gestellte Fragen zur Migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Ein LinkedIn-Lead wird nicht in Marketo Engage aufgenommen, wenn er mit einem in Marketo vorhandenen Personendatensatz übereinstimmt, der mit einem mit Unternehmens-APIs erstellten Unternehmensdatensatz verknüpft ist, und das Marketo-Abonnement nicht mit einem CRM verbunden ist.

1. Wechseln Sie zu Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gehen Sie zu **LaunchPoint**, klicken Sie auf **Neu** und wählen Sie **Neuer Service** aus.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigenamen** für Ihren Dienst ein, wählen Sie den **LinkedIn Lead Gen**-Dienst aus der Dropdown-Liste aus und klicken Sie auf **Weiter**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo öffnet eine neue Registerkarte im selben Browser unter [linkedin.com](https://www.linkedin.com). Melden Sie sich bei LinkedIn mit dem Konto an, das Sie für die Integration verwenden möchten.

   >[!NOTE]
   >
   >Das LinkedIn-Konto benötigt Zugriff auf alle LinkedIn-Geschäftskonten, für die Sie gesponserte Kampagnen erstellen.

   ![](assets/linkedin-login.png)

1. Kehren Sie nach der Anmeldung bei LinkedIn zu Marketo zurück und klicken Sie auf **Autorisieren**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Klicken Sie auf **Zulassen**, um die Installation der Marketo-App in LinkedIn zu akzeptieren.

   ![](assets/linkedin-marketo-allow.png)

1. Sie werden feststellen, dass Sie jetzt autorisiert sind. Klicken Sie auf **Weiter**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Der Dienst läuft automatisch ein Jahr nach der Autorisierung ab. Um den Zugriff wiederherzustellen, klicken Sie einfach **Erneut autorisieren**. Abhängig von Ihren Browsereinstellungen müssen Sie Ihr LinkedIn-Kennwort möglicherweise erneut eingeben.

1. Wählen Sie die Konten aus, von denen aus LinkedIn Lead Gen-Leads in Marketo eingehen sollen, und klicken Sie auf **Weiter**.

   >[!TIP]
   >
   >Wenn Sie die erwarteten Geschäftskonten nicht sehen, stellen Sie sicher, dass das autorisierte LinkedIn-Konto des Benutzers über Lead-Gen-Formular-Manager-Berechtigungen für das Geschäftskonto in LinkedIn verfügt.

   ![](assets/linkedin-pages-to-capture.png)

1. Um standardmäßige Feldzuordnungen von LinkedIn zu Marketo zu akzeptieren, klicken Sie einfach auf **Erstellen**. Wenn Sie die standardmäßige Feldzuordnung ändern, eine Feldzuordnung entfernen oder eine neue Feldzuordnung hinzufügen möchten, können Sie dies für jedes Feld über das unten stehende Modal tun.

   >[!CAUTION]
   >
   >Marketo unterstützt die Zuordnung von zwei LinkedIn-Feldern zu einem einzigen Marketo-Feld **jedoch nur, wenn** beiden LinkedIn-Felder sich nicht im selben Formular befinden. Wenn Sie zwei Felder aus demselben LinkedIn-Formular einem einzigen Marketo-Feld zuordnen, können Personen Ihre Marketo-Datenbank möglicherweise nicht eingeben.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Nur LinkedIn-Felder, die bereits in [Formularvorlage“ ](https://www.linkedin.com/help/lms/answer/79634) LinkedIn Campaign Manager gespeichert wurden, werden als LinkedIn-Felder angezeigt, die Marketo-Feldern zugeordnet werden können.

   ![](assets/linkedin-installed-services.png)

Gut gemacht! Personen, die LinkedIn-Lead-Gen-Formulare senden, gelangen während der Durchführung erfolgreicher Kampagnen auf LinkedIn in Marketo.

>[!NOTE]
>
>Sie können nur ein einziges LinkedIn-Benutzerkonto autorisieren. Wenn Sie mehrere Geschäftskonten haben, die Sie mit Marketo verknüpfen möchten, stellen Sie sicher, dass das autorisierte LinkedIn-Konto des Benutzers über Lead-Gen-Formular-Manager-Berechtigungen für das Geschäftskonto in LinkedIn verfügt.

>[!MORELIKETHIS]
>
>[Verwenden von Formularfiltern und Triggern der LinkedIn-Lead-Generation in einer Smart-Kampagne](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
