---
description: Globale Formularvalidierungsregeln - Marketo-Dokumente - Produktdokumentation
title: Globale Formularvalidierungsregeln
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 2%

---

# Globale Formularvalidierungsregeln {#global-form-validation-rules}

Mit dieser Funktion können Sie verhindern, dass bestimmte Domains an Marketo Engage-Formulare gesendet werden.

## Aktivieren des Zugriffs {#how-to-enable-access}

Bevor Sie diese Funktion verwenden können, müssen Sie ihre Berechtigung für die gewünschte Rolle aktivieren.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/global-form-validation-rules-2.png)

1. Klicken Sie auf die **[!UICONTROL Rollen]**.

   ![](assets/global-form-validation-rules-3.png)

1. Doppelklicken Sie auf die Rolle, der Sie Berechtigungen erteilen möchten.

   ![](assets/global-form-validation-rules-4.png)

1. Klicken Sie auf das Pluszeichen **+** neben **Zugriff auf Admin**.

   ![](assets/global-form-validation-rules-5.png)

1. Scrollen Sie nach unten, wählen Sie **[!UICONTROL Formularvalidierungsregeln aufrufen]** und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/global-form-validation-rules-6.png)

## Erstellen einer neuen Formularvalidierungsregel {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Diese Regeln gelten für alle Formulare in Ihren Marketo Engage-Abonnements.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Klicken Sie **[!UICONTROL Globale Formularvalidierungsregel]**.

   ![](assets/global-form-validation-rules-8.png)

1. Klicken Sie **[!UICONTROL Neue Formularvalidierungsregel]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >In [!UICONTROL  Dropdown-Liste Formularvalidierungsregelaktionen ] Sie vorhandene Regeln löschen oder bearbeiten.

1. Benennen Sie Ihre Regel, geben Sie ihr eine optionale Beschreibung und geben Sie die Fehlermeldung ein, die den Besuchern des Formulars angezeigt werden soll. Geben Sie im Feld Regeln die Domain(s) ein, die blockiert werden sollen, wählen Sie **[!UICONTROL Regel aktivieren]** und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage verfügt über eine definierte Blockierungsliste von kostenlosen E-Mail-Domains von Privatkund*innen, die bei Verwendung unserer vorab geladenen Regel „Verbraucher-E-Mail-Domain-Blockierungsliste&quot; blockiert werden. [Diese Liste hier anzeigen](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) (Zum Herunterladen stellen Sie sicher, dass Ihr Browser auf dem neuesten Stand ist und Downloads akzeptieren kann).

## Deaktivieren des Zugriffs pro Formular{#how-to-disable-access-per-form}

Nach der Aktivierung gelten die Regeln für alle Formulare. Wenn Sie jedoch ein Formular mit bestimmten Anforderungen haben und Sie keine Zurückweisungen wünschen, können Sie [!UICONTROL Globale Formularvalidierungsregeln] in den Formulareinstellungen deaktivieren.

1. Klicken Sie im gewünschten Formular auf **[!UICONTROL Formulareinstellungen]** und dann auf **[!UICONTROL Einstellungen]**.

   ![](assets/global-form-validation-rules-11.png)

1. Klicken Sie auf die **[!UICONTROL Globale Formularvalidierungsregeln]** und wählen Sie **[!UICONTROL Deaktiviert]**.

   ![](assets/global-form-validation-rules-12.png)

Wenn Sie Ihr Formular genehmigen und senden, werden Ihre [!UICONTROL globalen Formularvalidierungsregeln] ignoriert.
