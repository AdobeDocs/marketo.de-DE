---
unique-page-id: 2949711
description: Installieren des Marketo-E-Mail-Add-ins für Outlook mit einem Registrierungs-Code - Marketo Docs - Produktdokumentation
title: Installieren des Marketo-E-Mail-Add-ins für Outlook mit einem Registrierungs-Code
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 0dec1dc142a7296ce9d5db91493f654dbe7ee99a
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Installieren des Marketo-E-Mail-Add-ins für Outlook mit einem Registrierungs-Code {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Wenn Benutzer auf die Admin-Einstellungen auf ihren Laptops zugreifen können, können Sie ihnen direkt einen Registrierungs-Code senden.

Wenn Sie keine Einladungs-E-Mail erhalten haben, bitten Sie Ihren Marketo-Administrator, Sie einzuladen.

>[!PREREQUISITES]
>
>Du musst [hat eine Marketo Email Add-In-Lizenz ausgestellt](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>Die Installation wird nicht auf PCs unterstützt, auf denen der Ordner Windows-Benutzer nicht englische Zeichen enthält. Dieser Ordner wird automatisch von Windows unter <System Root>\Benutzer\ basierend auf dem Windows-Benutzernamen und kann nicht englische Zeichen enthalten, wenn der Windows-Benutzername ein nicht englischer Name ist. Wenden Sie sich an Ihr IT-Team, um festzustellen, ob bei der Installation Probleme auftreten.

>[!NOTE]
>
>Am 20.1.2010 stellte die neueste Version des Outlook-Plug-ins die Unterstützung des Offline-Modus ein.

## Installationsprogramm herunterladen {#download-installer}

1. Identifizieren Sie Ihre [Microsoft Outlook-Version](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)

1. Klicken Sie auf den Link, um das Installationsprogramm herunterzuladen, das für Ihre Version von Microsoft Outlook geeignet ist.

   >[!NOTE]
   >
   >Derzeit funktionieren die folgenden Links nur in Microsoft Edge oder durch Rechtsklick in Chrome. Entschuldigung für eventuelle Unannehmlichkeiten.

   | Outlook-Version | 32-Bit-Outlook | 64-Bit-Outlook |
   |---|---|---|
   | Outlook 2000 | Nicht unterstützt | n.z |
   | Outlook 2003 | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | n.z |
   | Outlook 2007 | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | n.z |
   | Outlook 2010 | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook für Mac | Nicht unterstützt | Nicht unterstützt |
   | Outlook Web App | Nicht unterstützt | Nicht unterstützt |
   | Office 365* | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Herunterladen](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365-Version: Nur Windows-Client (unter Windows 10, Enterprise oder Pro).

## Registrierungscode kopieren {#copy-your-registration-code}

1. Kopieren Sie den Registrierungs-Code aus der Einladungs-E-Mail, die Sie erhalten haben.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Schließen Sie Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Installieren {#install}

1. Führen Sie das Installationsprogramm aus.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Wenn du eine Sicherheitswarnung bekommst, mach dir keine Sorgen! Klicken Sie einfach auf **Ausführen**.

1. Klicken **Nächste**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Ausfüllen **Vorname**, **Nachname**, **Email-Adresse**, kopieren und fügen Sie die **Registrierungs-Code** aus der E-Mail in das Formular und klicken Sie auf **Nächste**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Wenn die Installation fehlschlägt, wenden Sie sich an Ihre IT-Abteilung, um sicherzustellen, dass der HTTPS-Traffic nicht blockiert wird. Für das Installationsprogramm muss HTTPS-Traffic geöffnet sein.

1. Klicken **Nächste** , um die Installation am Standardspeicherort durchzuführen.

   ![](assets/select-installation-folder-hand.png)

1. Klicken **Nächste**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Wenn Sie eine Sicherheitsaufforderung bezüglich eines unbekannten Herausgebers erhalten, klicken Sie auf **Ja**.

1. Die Installation ist jetzt abgeschlossen. Klicken Sie auf **Schließen**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Öffnen Sie jetzt Microsoft Outlook und sehen Sie sich die Marketo-Schaltflächen an.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Ausgezeichnet! Jetzt sind die Marketo-Schaltflächen an einem besseren Ort.

Erfahren Sie mehr über die Verwendung der Aktionen &quot;Marketo Message&quot;und &quot;Log With Marketo&quot;.

>[!MORELIKETHIS]
>
>* [Senden und Verfolgen einer E-Mail mit dem Marketo E-Mail-Add-in für Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Senden und Verfolgen aus Outlook mit einer Marketo-Vorlage](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

