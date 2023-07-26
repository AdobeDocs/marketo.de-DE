---
description: Globale Formularvalidierungsregeln - Marketo-Dokumente - Produktdokumentation
title: Globale Formularvalidierungsregeln
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Globale Formularvalidierungsregeln {#global-form-validation-rules}

Mit dieser Funktion können Sie verhindern, dass bestimmte Domänen an Marketo Engage-Formulare gesendet werden.

## Aktivieren des Zugriffs {#how-to-enable-access}

Bevor Sie diese Funktion verwenden können, müssen Sie ihre Berechtigung für jede gewünschte Rolle aktivieren.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Klicks **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/global-form-validation-rules-2.png)

1. Klicken Sie auf **[!UICONTROL Rollen]** Registerkarte.

   ![](assets/global-form-validation-rules-3.png)

1. Doppelklicken Sie auf die Rolle, der Sie Berechtigungen gewähren möchten.

   ![](assets/global-form-validation-rules-4.png)

1. Klicken Sie auf **+** neben Zugriff auf Admin.

   ![](assets/global-form-validation-rules-5.png)

1. Scrollen Sie nach unten und wählen Sie **[!UICONTROL Auf Formularvalidierungsregeln zugreifen]** und klicken **[!UICONTROL Speichern]**.

   ![](assets/global-form-validation-rules-6.png)

## Neue Formularvalidierungsregel erstellen {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Diese Regeln gelten für alle Formulare in Ihren Marketo Engage-Abonnements.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Klicks **[!UICONTROL Regel für globale Formularüberprüfung]**.

   ![](assets/global-form-validation-rules-8.png)

1. Klicks **[!UICONTROL Neue Formularvalidierungsregel]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >In der Dropdown-Liste Aktionen für Formularvalidierungsregeln können Sie vorhandene Regeln löschen oder bearbeiten.

1. Benennen Sie Ihre Regel, geben Sie ihr eine optionale Beschreibung und geben Sie die Fehlermeldung ein, die Ihre Formular-Besucher sehen sollen. Geben Sie die Domäne(n) ein, die blockiert werden sollen, und wählen Sie **[!UICONTROL Regel aktivieren]** und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage verfügt über eine definierte Blockierungsliste kostenloser E-Mail-Domains für Verbraucher, die blockiert werden, wenn die Regel &quot;KundenE-Mail-Domain-Vorabregistrierung&quot;verwendet wird. [Liste hier anzeigen](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Deaktivieren des Zugriffs pro Formular{#how-to-disable-access-per-form}

Nach der Aktivierung gelten Regeln für alle Formulare. Wenn Sie jedoch ein Formular mit bestimmten Anforderungen haben und nichts zurückgewiesen werden soll, können Sie [!UICONTROL Globale Formularvalidierungsregeln] in den Einstellungen des Formulars.

1. Klicken Sie in dem gewünschten Formular auf **[!UICONTROL Formulareinstellungen]**, dann **[!UICONTROL Einstellungen]**.

   ![](assets/global-form-validation-rules-11.png)

1. Klicken Sie auf **[!UICONTROL Globale Formularvalidierungsregeln]** und wählen Sie **[!UICONTROL Behinderte]**.

   ![](assets/global-form-validation-rules-12.png)

Wenn Sie Ihr Formular genehmigen und posten, wird es Ihre [!UICONTROL Globale Formularvalidierungsregeln].
