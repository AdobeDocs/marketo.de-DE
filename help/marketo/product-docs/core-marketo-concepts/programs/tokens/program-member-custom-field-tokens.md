---
unique-page-id: 1147114
description: Benutzerdefinierte Feld-Token für Programmteilnehmer - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Feld-Token für Programmteilnehmer
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---

# Benutzerdefinierte Feld-Token für Programmteilnehmer {#program-member-custom-field-tokens}

## Token-Unterstützung für benutzerdefinierte Felder von Programmmitgliedern {#token-support-for-program-member-custom-fields}

Auf der Rückseite der Funktionen für benutzerdefinierte Felder von Programmmitgliedern wird die Unterstützung für benutzerdefinierte Felder von Programmmitgliedern in Token-Frameworks erweitert.

Die PMCF-Token werden unter der Mitglieddomäne der Token-Familie unterstützt.

Mitglieder-Token werden für Felder verwendet, die in den Bereich „Programmteilnehmer“ fallen. Ab dem aktuellen Status werden Mitglieder-Token auch verwendet, um eindeutige Werte von integrierten Service-Partnern einzufügen. `{{member.webinar url}}` Token löst automatisch die eindeutige Bestätigungs-URL der Person auf, die vom Dienstleister generiert wurde. {{member.registration code}} wird zum Registrierungs-Code aufgelöst, der vom Dienstleister bereitgestellt wird.

>[!NOTE]
>
>* Benutzerdefinierte Felder für Programmteilnehmer können nur im Kontext eines Programms verwendet werden.
>* Benutzerdefinierte Felder für Programmteilnehmer können nicht in folgenden Bereichen verwendet werden: E-Mail-Preheader, Datums-Token in Warteschritten oder Snippets.
>* Der Status des Programmmitglieds wird in Mitglieds-Token nicht unterstützt.

## Verwenden der benutzerdefinierten Feld-Token für Programmteilnehmer in Assets {#using-program-member-custom-field-tokens-in-assets}

Benutzerdefinierte Felder für Programmteilnehmer können in E-Mails, Landingpages, SMS, Push-Benachrichtigungen und Webhooks eingefügt werden.

**E-Mails**

1. Wählen Sie die gewünschte E-Mail aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Klicken Sie auf das Symbol Token einfügen .

   ![](assets/program-member-custom-field-tokens-2.png)

1. Suchen Sie das gewünschte Token im Feld Benutzerdefiniertes Programmmitglied, wählen Sie es aus, geben Sie einen Standardwert ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Vergessen Sie nicht, Ihre E-Mail zu genehmigen.

**Landingpages**

1. Wählen Sie Ihre Landingpage aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >Der Landingpage-Designer wird in einem neuen Fenster geöffnet.

1. Doppelklicken Sie auf das Rich-Text-Feld, dem Sie das Token hinzufügen möchten.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Klicken Sie an die Stelle, an der das Token sein soll, und klicken Sie dann auf das Symbol Token einfügen .

   ![](assets/program-member-custom-field-tokens-7.png)

1. Suchen und wählen Sie das gewünschte Token aus.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Geben Sie einen Standardwert ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Wählen Sie die gewünschte SMS aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Klicken Sie auf die Schaltfläche **`{{ Token`** .

   ![](assets/program-member-custom-field-tokens-12.png)

1. Suchen Sie das gewünschte Token für das benutzerdefinierte Feld Programmteilnehmer und wählen Sie es aus. Geben Sie einen [!UICONTROL Standardwert“ ein ] klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Klicken Sie auf die Dropdown-Liste SMS-Aktionen und wählen Sie **[!UICONTROL Genehmigen und schließen]**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Push-Benachrichtigungen**

1. Wählen Sie die gewünschte Push-Benachrichtigung aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Klicken Sie auf **[!UICONTROL Push-Benachrichtigung]**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Klicken Sie im Editor auf die Nachricht und dann auf die Schaltfläche `{{` , um die Token-Auswahl aufzurufen.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Suchen Sie das gewünschte Token für das benutzerdefinierte Feld Programmteilnehmer und wählen Sie es aus. Geben Sie einen Standardwert ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Klicken Sie auf **[!UICONTROL Beenden]**, um zu speichern und zu beenden (oder **[!UICONTROL Weiter]**, um zuerst zu überprüfen).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Wenn das benutzerdefinierte Feld Programmteilnehmer für ein Programmmitglied keinen Wert hat, wird das Token durch den Standardwert ersetzt, sofern dieser angegeben wurde.

## Verwenden der Token für benutzerdefinierte Felder von Programmmitgliedern in Kampagnen {#using-program-member-custom-field-tokens-in-campaigns}

Benutzerdefinierte Feld-Token für Programmteilnehmer können in folgenden Bereichen verwendet werden:

* Aufgabe erstellen
* Aufgabe in Microsoft erstellen
* Interessante Momente
* Fluss-Aktionen für Datenwerte ändern
* Webhooks
