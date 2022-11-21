---
description: Globale Formularvalidierungsregeln - Marketo-Dokumente - Produktdokumentation
title: Globale Formularvalidierungsregeln
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: 2736e8a0456de76b9894312c26f6ba9c0345daee
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Globale Formularvalidierungsregeln {#global-form-validation-rules}

Mit dieser Funktion können Sie verhindern, dass bestimmte Domänen an Marketo Engage-Formulare gesendet werden.

## Aktivieren des Zugriffs {#how-to-enable-access}

Bevor Sie diese Funktion verwenden können, müssen Sie ihre Berechtigung für jede gewünschte Rolle aktivieren.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/global-form-validation-rules-1.png)

1. Klicken **Benutzer und Rollen**.

   ![](assets/global-form-validation-rules-2.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/global-form-validation-rules-3.png)

1. Doppelklicken Sie auf die Rolle, der Sie Berechtigungen gewähren möchten.

   ![](assets/global-form-validation-rules-4.png)

1. Klicken Sie auf **+** neben Zugriff auf Admin.

   ![](assets/global-form-validation-rules-5.png)

1. Scrollen Sie nach unten und wählen Sie **Auf Formularvalidierungsregeln zugreifen** und klicken Sie auf **Speichern**.

   ![](assets/global-form-validation-rules-6.png)

## Neue Formularvalidierungsregel erstellen {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Diese Regeln gelten für alle Formulare in Ihren Marketo Engage-Abonnements.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/global-form-validation-rules-7.png)

1. Klicken **Regel für globale Formularüberprüfung**.

   ![](assets/global-form-validation-rules-8.png)

1. Klicken **Neue Formularvalidierungsregel**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >In der Dropdown-Liste Aktionen für Formularvalidierungsregeln können Sie vorhandene Regeln löschen oder bearbeiten.

1. Benennen Sie Ihre Regel, geben Sie ihr eine optionale Beschreibung und geben Sie die Fehlermeldung ein, die Ihre Formular-Besucher sehen sollen. Geben Sie die Domäne(n) ein, die blockiert werden sollen, und wählen Sie **Regel aktivieren** und klicken Sie auf **Erstellen**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage verfügt über eine definierte Blockierungsliste kostenloser E-Mail-Domains für Verbraucher, die blockiert werden, wenn die Regel &quot;KundenE-Mail-Domain-Vorabregistrierung&quot;verwendet wird. [Liste hier anzeigen](/help/marketo/product-docs/administration/settings/assets/freemaildomains_2023.csv).

## Deaktivieren des Zugriffs pro Formular{#how-to-disable-access-per-form}

Nach der Aktivierung gelten Regeln für alle Formulare. Wenn Sie jedoch ein Formular mit bestimmten Anforderungen haben und nichts zurückgewiesen werden soll, können Sie die globalen Regeln zur Formularüberprüfung in den Einstellungen des Formulars deaktivieren.

1. Klicken Sie in dem gewünschten Formular auf **Formulareinstellungen**, dann **Einstellungen**.

   ![](assets/global-form-validation-rules-11.png)

1. Klicken Sie auf die Dropdown-Liste Globale Formularvalidierungsregeln und wählen Sie **Behinderte**.

   ![](assets/global-form-validation-rules-12.png)

Wenn Sie Ihr Formular genehmigen und posten, werden Ihre Regeln zur globalen Formularüberprüfung ignoriert.
