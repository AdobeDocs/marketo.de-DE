---
unique-page-id: 2949711
description: Installieren des Marketo-E-Mail-Add-ins für Outlook mit einem Registrierungs-Code - Marketo Docs - Produktdokumentation
title: Installieren des Marketo-E-Mail-Add-ins für Outlook mit einem Registrierungs-Code
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 40fe81d465d04be97ae5e216250b7e06e6d3791e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 3%

---

# Installieren des Marketo-E-Mail-Add-ins für Outlook mit einem Registrierungs-Code {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Wenn Benutzer auf die Admin-Einstellungen auf ihren Laptops zugreifen können, können Sie ihnen direkt einen Registrierungs-Code senden.

Wenn Sie keine Einladungs-E-Mail erhalten haben, bitten Sie Ihren Marketo-Administrator, Sie einzuladen.

>[!PREREQUISITES]
>
>Sie müssen [eine Marketo E-Mail-Add-In-Lizenz erhalten](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>Die Installation wird nicht auf PCs unterstützt, auf denen der Ordner Windows-Benutzer nicht englische Zeichen enthält. Dieser Ordner wird automatisch von Windows unter `<System Root>\Users\` basierend auf dem Windows-Benutzernamen generiert und kann nicht englische Zeichen enthalten, wenn der Windows-Benutzername ein nicht englischer Name ist. Wenden Sie sich an Ihr IT-Team, um festzustellen, ob bei der Installation Probleme auftreten.

>[!NOTE]
>
>Die Funktionen von Sales Insight-Aktionen, einschließlich &quot;E-Mail an Vertrieb senden&quot;, &quot;Zu Vertriebskampagne hinzufügen&quot;und &quot;Aufgaben&quot;, sind nicht in den Sales Insight-E-Mail-Plugins für Gmail und Outlook verfügbar. Derzeit können Benutzer von ihrem E-Mail-Client aus nur trackbare E-Mails mit oder ohne Marketo-E-Mail-Vorlage senden, wenn sie die Sales Insight-E-Mail-Plugins verwenden.

## Installationsprogramm herunterladen {#download-installer}

1. Identifizieren Sie Ihre [Microsoft Outlook-Version](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}

1. Klicken Sie auf den Link, um das Installationsprogramm herunterzuladen, das für Ihre Version von Microsoft Outlook geeignet ist.

   >[!NOTE]
   >
   >Derzeit funktionieren die folgenden Links nur in Microsoft Edge oder durch Rechtsklick in Chrome. Entschuldigung für eventuelle Unannehmlichkeiten.

   | Outlook-Version | 32-Bit-Outlook | 64-Bit-Outlook |
   |---|---|---|
   | Outlook 2000 | Nicht unterstützt | Nicht zutreffend |
   | Outlook 2003 | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | Nicht zutreffend |
   | Outlook 2007 | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | Nicht zutreffend |
   | Outlook 2010 | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Download](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Download](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Download](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Download](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook für Mac | Nicht unterstützt | Nicht unterstützt |
   | Outlook Web App | Nicht unterstützt | Nicht unterstützt |
   | Office 365* | [Download](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Download](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365-Version: Nur Windows-Client (unter Windows 10, Enterprise oder Pro).

   >[!IMPORTANT]
   >
   >Microsoft hat eine [neue Version von Outlook für Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"} veröffentlicht. Diese neue Version unterstützt das vorhandene MSI Outlook-Plugin nicht. Das MSI Outlook-Plugin funktioniert weiterhin für Windows-Desktops, die die klassische Version von Outlook ausführen. Um mehr über den neuen Outlook für Windows für Unternehmen zu erfahren, klicken Sie [hier](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}.

## Registrierungscode kopieren {#copy-your-registration-code}

1. Kopieren Sie den Registrierungscode aus der Einladungs-E-Mail, die Sie erhalten haben.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Schließen Sie Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Installieren {#install}

1. Führen Sie das Installationsprogramm aus.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Wenn du eine Sicherheitswarnung bekommst, mach dir keine Sorgen! Klicken Sie einfach auf **Ausführen**.

1. Klicken Sie auf **Weiter**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Füllen Sie **Vorname**, **Nachname**, **E-Mail-Adresse** aus, kopieren Sie den **Registrierungs-Code** aus der E-Mail und klicken Sie auf **Weiter**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Wenn die Installation fehlschlägt, wenden Sie sich an Ihre IT-Abteilung, um sicherzustellen, dass der HTTPS-Traffic nicht blockiert wird. Für das Installationsprogramm muss HTTPS-Traffic geöffnet sein.

1. Klicken Sie auf **Weiter** , um die Installation am Standardspeicherort durchzuführen.

   ![](assets/select-installation-folder-hand.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Wenn Sie eine Sicherheitsaufforderung bezüglich eines unbekannten Herausgebers erhalten, klicken Sie auf **Ja**.

1. Klicken Sie nun auf **Schließen**, um die Installation abzuschließen.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Öffnen Sie jetzt Microsoft Outlook und sehen Sie sich die Marketo-Schaltflächen an.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Ausgezeichnet! Jetzt sind die Marketo-Schaltflächen an einem besseren Ort.

Erfahren Sie mehr über die Verwendung der Aktionen &quot;Marketo Message&quot;und &quot;Log With Marketo&quot;.

>[!MORELIKETHIS]
>
>* [Senden und Verfolgen einer E-Mail mit dem Marketo-E-Mail-Add-in für Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Versand und Tracking aus Outlook mit einer Marketo-Vorlage](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
