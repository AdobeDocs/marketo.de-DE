---
unique-page-id: 1147114
description: Benutzerdefinierte Feld-Token für Programmteilnehmer - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Feld-Token für Programmteilnehmer
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: b21f955bf98063e11f8ed3fdc6f164134ee4f5aa
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---

# Benutzerdefinierte Feld-Token für Programmteilnehmer {#program-member-custom-field-tokens}

## Token-Unterstützung für benutzerdefinierte Felder für Programmmitglieder {#token-support-for-program-member-custom-fields}

Auf der Rückseite der Funktionen für benutzerdefinierte Felder des Programmmitglieds wird die Unterstützung für benutzerdefinierte Felder des Programmmitglieds in Token-Frameworks erweitert.

Die PMCF-Token werden unter der Mitgliederdomäne der Token-Familie unterstützt.

Mitglieder-Token werden für Felder verwendet, die unter den Geltungsbereich des Programmmitglieds fallen. Ab dem aktuellen Status werden Member Tokens auch verwendet, um eindeutige Werte von integrierten Servicepartnern einzufügen. `{{member.webinar url}}` -Token löst automatisch die eindeutige Bestätigungs-URL der Person auf, die vom Dienstleister generiert wurde. {{member.registration code}} wird in den vom Dienstleister bereitgestellten Registrierungs-Code aufgelöst.

>[!NOTE]
>
>* Benutzerdefinierte Felder für Programmmitglieder können nur im Kontext eines Programms verwendet werden.
>* Benutzerdefinierte Felder des Programmmitglieds können nicht in verwendet werden: E-Mail-Preheader, Datum-Token in Warteschritten oder Snippets.
>* Der Status der Programmteilnehmer wird in den Mitglieds-Token nicht unterstützt.

## Verwenden von benutzerdefinierten Feld-Token für Programmteilnehmer in Assets {#using-program-member-custom-field-tokens-in-assets}

Sie können Token für benutzerdefinierte Felder des Programmmitglieds in E-Mails, Landingpages, SMS, Push-Benachrichtigungen und Webhooks einfügen.

**E-Mails**

1. Wählen Sie die gewünschte E-Mail aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Klicken Sie auf das Symbol Token einfügen .

   ![](assets/program-member-custom-field-tokens-2.png)

1. Suchen und wählen Sie das gewünschte benutzerdefinierte Feld-Token für Programmteilnehmer aus, geben Sie einen Standardwert ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Vergessen Sie nicht, Ihre E-Mail zu genehmigen.

**Einstiegsseiten**

1. Wählen Sie Ihre Landingpage aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >Der Landingpage-Designer wird in einem neuen Fenster geöffnet.

1. Doppelklicken Sie auf das Rich-Text-Feld, dem Sie das Token hinzufügen möchten.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Klicken Sie auf die Stelle, an der das Token platziert werden soll, und klicken Sie dann auf das Symbol Token einfügen .

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

1. Suchen und wählen Sie das gewünschte benutzerdefinierte Feld-Token für Programmteilnehmer aus. Geben Sie einen Standardwert ein und klicken Sie auf Einfügen.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Klicken Sie auf das Dropdown-Menü SMS-Aktionen und wählen Sie **[!UICONTROL Genehmigen und schließen]** aus.

   ![](assets/program-member-custom-field-tokens-14.png)

**Push-Benachrichtigungen**

1. Wählen Sie die gewünschte Push-Benachrichtigung aus und klicken Sie auf **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Klicken Sie auf **[!UICONTROL Push Notification]**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Klicken Sie auf die Nachricht im Editor und klicken Sie auf die Schaltfläche `{{` , um die Token-Auswahl abzurufen.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Suchen und wählen Sie das gewünschte benutzerdefinierte Feld-Token für Programmteilnehmer aus. Geben Sie einen Standardwert ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Klicken Sie auf **[!UICONTROL Beenden]** , um zu speichern und zu beenden (oder auf **[!UICONTROL Weiter]** , um zuerst zu überprüfen).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Wenn das benutzerdefinierte Feld &quot;Programmteilnehmer&quot;für ein Programmmitglied keinen Wert aufweist, wird das Token durch den Standardwert ersetzt, sofern er angegeben wurde.

## Verwenden von benutzerdefinierten Feld-Token für Programmteilnehmer in Kampagnen {#using-program-member-custom-field-tokens-in-campaigns}

Benutzerdefinierte Feld-Token für Programmmitglieder können in folgenden Bereichen verwendet werden:

* Aufgabe erstellen
* Aufgabe in Microsoft erstellen
* Interessante Momente
* Fluss-Aktionen für Datenwerte ändern
* Webhooks
