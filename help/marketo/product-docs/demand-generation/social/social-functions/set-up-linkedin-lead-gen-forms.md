---
unique-page-id: 12976798
description: Einrichten von LinkedIn Lead Gen Forms - Marketo Docs - Produktdokumentation
title: Einrichten von LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Einrichten von LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Verwenden Sie LinkedIn Lead Gen Forms, um Werbekampagnen in LinkedIn auszuführen und Leads für Marketo zu generieren.

>[!IMPORTANT]
>
>LinkedIn aktualisiert ihre Marketing-APIs, die von Marketo Engage LinkedIn-Integrationen verwendet werden. Diese Änderungen erfordern eine erneute Authentifizierung aller LinkedIn LaunchPoint-Dienste in Ihrem Menü **Admin** > **LaunchPoint** zwischen dem 7. Juni und dem 15. Dezember 2024, um eine Dienstunterbrechung zu vermeiden. Weitere Informationen finden Sie in den [FAQ zur Migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Ein LinkedIn-Lead kommt nicht in die Marketo Engage, wenn er mit einem in Marketo vorhandenen Personendatensatz übereinstimmt, der mit einem mithilfe von Unternehmens-APIs erstellten Firmendatensatz verknüpft ist, und das Marketo-Abonnement nicht mit einem CRM verbunden ist.

1. Navigieren Sie zu Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Wechseln Sie zu **LaunchPoint**, klicken Sie auf **Neu** und wählen Sie **Neuer Dienst** aus.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigenamen** für Ihren Dienst ein, wählen Sie den Dienst **LinkedIn Lead Gen** aus der Dropdown-Liste aus und klicken Sie auf **Weiter**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo öffnet im selben Browser eine neue Registerkarte für [linkedin.com](https://www.linkedin.com). Melden Sie sich mit dem Konto, das Sie für die Integration verwenden möchten, bei LinkedIn an.

   >[!NOTE]
   >
   >Das LinkedIn-Konto muss Zugriff auf alle LinkedIn-Geschäftskonten haben, für die Sie gesponserte Kampagnen erstellen.

   ![](assets/linkedin-login.png)

1. Nachdem Sie bei LinkedIn angemeldet sind, kehren Sie zu Marketo zurück und klicken Sie auf **Autorisieren**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Klicken Sie nach Aufforderung auf **Zulassen** , um die Installation der Marketo-App in LinkedIn zu akzeptieren.

   ![](assets/linkedin-marketo-allow.png)

1. Du wirst feststellen, dass du jetzt autorisiert bist. Klicken Sie auf **Weiter**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Der Dienst läuft automatisch ein Jahr nach der Autorisierung ab. Um wieder Zugriff zu erhalten, klicken Sie einfach auf **Erneut autorisieren**. Je nach Browsereinstellungen müssen Sie möglicherweise Ihr LinkedIn-Kennwort erneut eingeben.

1. Wählen Sie die Konten aus, von denen die Lead-Gen-Leads von LinkedIn in Marketo eingehen sollen, und klicken Sie auf **Weiter**.

   >[!TIP]
   >
   >Wenn die von Ihnen erwarteten Geschäftskonten nicht angezeigt werden, stellen Sie sicher, dass das LinkedIn-Konto des Benutzers, für das die Berechtigung erteilt wurde, über die Berechtigungen des Generatorformularmanagers für das Geschäftskonto in LinkedIn verfügt.

   ![](assets/linkedin-pages-to-capture.png)

1. Um die standardmäßigen LinkedIn- zu Marketo-Feldzuordnungen zu akzeptieren, klicken Sie einfach auf **Erstellen**. Wenn Sie die standardmäßige Feldzuordnung ändern, eine Feldzuordnung entfernen oder ein neues Feld-Mapping hinzufügen möchten, können Sie dies über das nachstehende Modal für jedes Feld tun.

   >[!CAUTION]
   >
   >Marketo unterstützt die Zuordnung von zwei LinkedIn-Feldern zu einem einzelnen Marketo-Feld, **jedoch nur, wenn** die beiden LinkedIn-Felder nicht im selben Formular vorhanden sind. Wenn Sie zwei Felder desselben LinkedIn-Formulars einem einzigen Marketo-Feld zuordnen, können Personen möglicherweise nicht in Ihre Marketo-Datenbank eintreten.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Nur LinkedIn-Felder, die bereits in einer [Formularvorlage](https://www.linkedin.com/help/lms/answer/79634) im LinkedIn Campaign Manager gespeichert wurden, werden als LinkedIn-Felder angezeigt, die Marketo-Feldern zugeordnet werden können.

   ![](assets/linkedin-installed-services.png)

Schön gemacht! Personen, die LinkedIn Lead Gen-Formulare senden, fließen beim Ausführen erfolgreicher Kampagnen auf LinkedIn-Seite in Marketo weiter.

>[!NOTE]
>
>Sie können nur ein einziges LinkedIn-Benutzerkonto autorisieren. Wenn Sie über mehrere Unternehmenskonten verfügen, die Sie mit Marketo verknüpfen möchten, stellen Sie sicher, dass das LinkedIn-Konto des Benutzers, für das die Berechtigung erteilt wurde, über die Berechtigung &quot;Generatorformularmanager&quot;für das Geschäftskonto in LinkedIn verfügt.

>[!MORELIKETHIS]
>
>[Verwenden von LinkedIn Lead Gen-Formularfiltern und -Triggern in einer Smart-Kampagne](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
