---
unique-page-id: 2949279
description: Aktualisieren des Marketo-E-Mail-Add-ins  [!DNL Outlook]  Marketo Docs - Produktdokumentation
title: Aktualisieren des Marketo E-Mail-Add-ins für [!DNL Outlook]
exl-id: 079f1142-8062-448c-aa07-59ecd89a718f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 13%

---

# Aktualisieren des Marketo-E-Mail-Add-ins für [!DNL Outlook] {#upgrade-your-marketo-email-add-in-for-outlook}

Wenn eine neue Version des Marketo-E-Mail-Add-ins für [!DNL Outlook] verfügbar ist, befolgen Sie diese Anweisungen zum Upgrade.

>[!NOTE]
>
>Ab dem 10/1/20 unterstützt die neueste Version des [!DNL Outlook]-Plug-ins den Offline-Modus nicht mehr. Dies wird nach der Installation/Aktualisierung am oder nach dem 10/1 wirksam.

## Installationsprogramm herunterladen {#download-installer}

Laden Sie das für Ihre Version von Microsoft [!DNL Outlook] geeignete Installationsprogramm herunter.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th colspan="2">Installation der Einladung für einen Benutzer</th> 
   <th colspan="2">Installation des Unternehmensschlüssels</th> 
  </tr> 
  <tr> 
   <td><strong><span class="dnl">Outlook</span>-Version</strong></td> 
   <td><strong>32-Bit</strong></td> 
   <td><strong>64-Bit</strong></td> 
   <td><strong>32-Bit</strong></td> 
   <td><strong>64-Bit</strong></td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Outlook</span> 2000</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht zutreffend</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht zutreffend</td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Outlook 2003</span></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td>Nicht zutreffend</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht zutreffend</td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Ausblick</span> 2007</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td>Nicht zutreffend</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht zutreffend</td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Ausblick</span> 2010</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Ausblick</span> 2013</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Ausblick</span> 2016</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
  </tr> 
  <tr> 
   <td colspan="1"><span class="dnl">Ausblick</span> 2019</td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
  </tr> 
  <tr> 
   <td><span class="dnl">Outlook</span> für Mac</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht unterstützt</td> 
   <td>Nicht unterstützt</td> 
  </tr> 
  <tr> 
   <td colspan="1"><span class="dnl">Outlook</span> Web-App</td> 
   <td colspan="1">Nicht unterstützt</td> 
   <td colspan="1">Nicht unterstützt</td> 
   <td colspan="1">Nicht unterstützt</td> 
   <td colspan="1">Nicht unterstützt</td> 
  </tr> 
  <tr> 
   <td colspan="1"><span class="dnl">Office</span> 365*</td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Herunterladen</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Herunterladen</a></td> 
  </tr> 
 </tbody> 
</table>

&#42;Office 365-Version: Nur Windows-Client (unter Windows 10, Windows 11, Enterprise oder Pro).

## Upgrade {#upgrade}

1. Identifizieren Sie Ihre [[!DNL Microsoft Outlook] Version](https://support.microsoft.com/en-us/office/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c?ui=en-us&rs=en-us&ad=us).

1. Wählen Sie Ihre Version aus der obigen Liste aus.

1. Führen Sie das Installationsprogramm aus.

   ![](assets/image2014-9-23-16-3a53-3a56.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-9-23-16-3a54-3a8.png)

   >[!NOTE]
   >
   >In bestimmten Fällen fehlen die Daten. Kopieren Sie es aus der Registrierungs-E-Mail und schließen Sie dann [!DNL Outlook].

1. [!DNL Microsoft Outlook] schließen.

   ![](assets/ent-key-close-outlook-hand.png)

1. Sie werden feststellen, dass alle Ihre Informationen vorausgefüllt sind. Klicken Sie einfach **[!UICONTROL Weiter]**.

   ![](assets/image2014-9-23-16-3a54-3a40.png)

   >[!TIP]
   >
   >Wenn die Installation fehlschlägt, wenden Sie sich an Ihre IT-Abteilung, um sicherzustellen, dass der HTTPS-Traffic nicht blockiert wird. Für das Installationsprogramm muss HTTPS-Traffic geöffnet sein.

1. Klicken Sie **[!UICONTROL Weiter]**, um die Installation am Standardspeicherort durchzuführen.

   ![](assets/image2014-9-23-16-3a54-3a55.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2014-9-23-16-3a55-3a20.png)

1. Die Installation ist jetzt abgeschlossen. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2014-9-23-16-3a55-3a34.png)

1. Öffnen Sie jetzt [!UICONTROL Microsoft Outlook], um die neueste Version der Marketo-Schaltflächen anzuzeigen.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

>[!MORELIKETHIS]
>
>* [Senden und Verfolgen einer E-Mail mit dem Marketo E-Mail-Add-in für [!UICONTROL Outlook]](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Senden und Verfolgen aus [!UICONTROL Outlook] mithilfe einer Marketo-Vorlage](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)
