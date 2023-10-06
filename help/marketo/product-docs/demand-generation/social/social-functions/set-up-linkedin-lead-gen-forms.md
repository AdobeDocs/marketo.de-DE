---
unique-page-id: 12976798
description: Einrichten von LinkedIn Lead Gen Forms - Marketo Docs - Produktdokumentation
title: Einrichten von LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: e1254c8156557b27d066a4482076becbd03fc774
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Einrichten von LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Verwenden Sie LinkedIn Lead Gen Forms, um Werbekampagnen in LinkedIn auszuführen und Leads für Marketo zu generieren.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Ein LinkedIn-Lead kommt nicht in die Marketo Engage, wenn er mit einem in Marketo vorhandenen Personendatensatz übereinstimmt, der mit einem mithilfe von Unternehmens-APIs erstellten Firmendatensatz verknüpft ist, und das Marketo-Abonnement nicht mit einem CRM verbunden ist.

1. Navigieren zu Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Navigieren Sie zu **LaunchPoint**, klicken Sie auf **Neu** und wählen **Neuer Dienst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigename** Wählen Sie für Ihren Dienst die **LinkedIn Lead Gen.** Dienst aus der Dropdown-Liste aus und klicken Sie auf **Nächste**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo öffnet eine neue Registerkarte im selben Browser, um [linkedin.com](https://www.linkedin.com). Melden Sie sich mit dem Konto, das Sie für die Integration verwenden möchten, bei LinkedIn an.

   >[!NOTE]
   >
   >Das LinkedIn-Konto muss Zugriff auf alle LinkedIn-Geschäftskonten haben, für die Sie gesponserte Kampagnen erstellen.

   ![](assets/linkedin-login.png)

1. Nachdem Sie sich bei LinkedIn angemeldet haben, kehren Sie zu Marketo zurück und klicken Sie auf **Autorisieren**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Klicken Sie bei Aufforderung auf **Zulassen** , um die Installation der Marketo-App in LinkedIn zu akzeptieren.

   ![](assets/linkedin-marketo-allow.png)

1. Du wirst feststellen, dass du jetzt autorisiert bist. Klicken Sie auf **Weiter**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Der Dienst läuft automatisch ein Jahr nach der Autorisierung ab. Um den Zugriff wiederherzustellen, klicken Sie einfach auf **Erneutes Autorisieren**. Je nach Browsereinstellungen müssen Sie möglicherweise Ihr LinkedIn-Kennwort erneut eingeben.

1. Wählen Sie die Konten aus, von denen die Lead-Gen-Leads von LinkedIn nach Marketo gelangen sollen, und klicken Sie auf **Nächste**.

   >[!TIP]
   >
   >Wenn die von Ihnen erwarteten Geschäftskonten nicht angezeigt werden, stellen Sie sicher, dass das LinkedIn-Konto des Benutzers, für das die Berechtigung erteilt wurde, über die Berechtigungen des Generatorformularmanagers für das Geschäftskonto in LinkedIn verfügt.

   ![](assets/linkedin-pages-to-capture.png)

1. Um die standardmäßigen LinkedIn- zu Marketo-Feldzuordnungen zu akzeptieren, klicken Sie einfach auf **Erstellen**. Wenn Sie die standardmäßige Feldzuordnung ändern, eine Feldzuordnung entfernen oder ein neues Feld-Mapping hinzufügen möchten, können Sie dies über das nachstehende Modal für jedes Feld tun.

   >[!CAUTION]
   >
   >Marketo unterstützt die Zuordnung von zwei LinkedIn-Feldern zu einem einzigen Marketo-Feld. **aber nur, wenn** Die beiden LinkedIn-Felder befinden sich nicht im selben Formular. Wenn Sie zwei Felder desselben LinkedIn-Formulars einem einzigen Marketo-Feld zuordnen, können Personen möglicherweise nicht in Ihre Marketo-Datenbank eintreten.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Nur LinkedIn-Felder, die bereits in einem [Formularvorlage](https://www.linkedin.com/help/lms/answer/79634) wird in LinkedIn Campaign Manager als LinkedIn-Felder angezeigt, die Marketo-Feldern zugeordnet werden können.

   ![](assets/linkedin-installed-services.png)

Schön gemacht! Personen, die LinkedIn Lead Gen-Formulare senden, fließen beim Ausführen erfolgreicher Kampagnen auf LinkedIn-Seite in Marketo weiter.

>[!NOTE]
>
>Sie können nur ein einziges LinkedIn-Benutzerkonto autorisieren. Wenn Sie über mehrere Unternehmenskonten verfügen, die Sie mit Marketo verknüpfen möchten, stellen Sie sicher, dass das LinkedIn-Konto des Benutzers, für das die Berechtigung erteilt wurde, über die Berechtigung &quot;Generatorformularmanager&quot;für das Geschäftskonto in LinkedIn verfügt.

>[!MORELIKETHIS]
>
>[Verwenden von LinkedIn Lead Gen-Formularfiltern und -Triggern in einer Smart-Kampagne](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
