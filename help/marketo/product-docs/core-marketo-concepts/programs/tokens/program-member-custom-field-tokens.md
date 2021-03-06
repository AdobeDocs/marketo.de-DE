---
unique-page-id: 1147114
description: Benutzerspezifische Feldmarktzeichen für Programm-Mitglieder - MarketingToDocs - Produktdokumentation
title: Benutzerdefinierte FeldToken für Programm-Member
translation-type: tm+mt
source-git-commit: 35e8b41574ebf8aafa27a59440c8ea9cb6413d50
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Benutzerdefinierte FeldToken für Programm-Member {#program-member-custom-field-tokens}

## Token-Unterstützung für benutzerdefinierte Programm-Felder {#token-support-for-program-member-custom-fields}

Auf der Rückseite der Programm Member Custom Fields-Funktionen wird die Unterstützung für benutzerdefinierte Felder von Programmen in Token-Frameworks erweitert.

Die PMCF-Token werden unter der Mitgliederdomäne der Token-Familie unterstützt.

Member Tokens werden für Felder im Rahmen des Programm Member verwendet. Ab dem aktuellen Status werden Member Tokens auch verwendet, um eindeutige Werte von integrierten Servicepartnern einzufügen. `{{member.webinar url}}` -Token löst automatisch die vom Dienstleister generierte eindeutige Bestätigungs-URL der Person auf. {{member.registration code}} wird zum Registrierungscode aufgelöst, der vom Dienstleister bereitgestellt wird.

>[!NOTE]
>
>* Benutzerdefinierte Programm-Member-Felder können nur im Kontext eines Programms verwendet werden.
>* Token für benutzerdefinierte Programm-Member-Felder können nicht verwendet werden in: E-Mail-Skripten, E-Mail-Kopfzeile, Datums-Token in Warteschritten oder Snippets.
>* Programm Member Status wird in Member Tokens nicht unterstützt.


## Verwenden von Programm Member Custom Field Tokens in Assets {#using-program-member-custom-field-tokens-in-assets}

Sie können Token für benutzerdefinierte Programm-Felder in E-Mails, Landingpages, SMS, Push-Benachrichtigungen und Webhooks einfügen.

**E-Mails**

1. Wählen Sie die gewünschte E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Klicken Sie auf das Symbol &quot;Token einfügen&quot;.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Suchen und wählen Sie das gewünschte Programm-Member-Token für benutzerdefinierte Felder aus, geben Sie einen Standardwert ein und klicken Sie auf **Einfügen**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Vergessen Sie nicht, Ihre E-Mail zu genehmigen.

**Landingpages**

1. Wählen Sie Ihre Landingpage aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >Der Landingpages-Designer wird in einem neuen Fenster geöffnet.

1. Klicken Sie bei gedrückter Dublette auf das Rich-Textfeld, dem Sie das Token hinzufügen möchten.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Klicken Sie auf die Stelle, an der das Token eingefügt werden soll, und klicken Sie dann auf das Symbol Token einfügen.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Suchen und wählen Sie das gewünschte Token aus.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Geben Sie einen Standardwert ein und klicken Sie auf **Einfügen**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Wählen Sie die gewünschte SMS aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Klicken Sie auf die Schaltfläche **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Suchen und wählen Sie das gewünschte Programm-Member-Token für benutzerdefinierte Felder aus. Geben Sie einen Standardwert ein und klicken Sie auf &quot;Einfügen&quot;.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Klicken Sie auf die Dropdownliste SMS-Aktionen und wählen Sie **Genehmigen und Schließen**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Push-Benachrichtigungen**

1. Wählen Sie die gewünschte Push-Benachrichtigung aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Klicken Sie auf **Push Notification**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Klicken Sie auf die Nachricht im Editor und klicken Sie auf die Schaltfläche `{{`, um den Token-Selektor abzurufen.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Suchen und wählen Sie das gewünschte Programm-Member-Token für benutzerdefinierte Felder aus. Geben Sie einen Standardwert ein und klicken Sie auf **Einfügen**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Klicken Sie auf **Fertig stellen, um zu speichern und zu beenden (oder** Weiter **, um zuerst zu überprüfen).**

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Wenn das Programm Member Custom Field für ein Member des Programms keinen Wert hat, wird das Token durch den Standardwert ersetzt, wenn dieser bereitgestellt wurde.

## Verwenden von Programm Member Custom Field Tokens in Kampagnen {#using-program-member-custom-field-tokens-in-campaigns}

Benutzerdefinierte FeldToken für Programm-Member können verwendet werden in:

* Aufgabe erstellen
* Aufgabe in Microsoft erstellen
* Interessante Momente
* Datenwertflussaktionen ändern
* Webhooks
