---
unique-page-id: 11382815
description: Marketo [!DNL Outlook] Plug-in-Installation durch IT - Marketo-Dokumentation - Produktdokumentation
title: Marketo [!DNL Outlook] Plug-in-Installation durch IT
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 1%

---

# Installation des Marketo [!DNL Outlook]-Plug-ins durch IT {#marketo-outlook-plugin-installation-by-it}

Manchmal erfordern Unternehmensrichtlinien, dass ihr IT-Team die gesamte Software auf den Computern ihrer Mitarbeiter installiert. In diesen Fällen erledigt die IT dies häufig remote mit ihrer eigenen Bereitstellungssoftware. Dieses Dokument enthält die Befehlszeilen, die Sie während des Bereitstellungsprozesses zur Remote-Installation des Outlook-Plug-ins als Eingaben verwenden würden.

>[!PREREQUISITES]
>
>[Einrichten](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) des Unternehmensschlüssels.

Führen Sie die folgende Befehlszeile als „System“ oder als administratives Benutzerkonto mit dem Schalter /i zur Installation aus.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Zur Fehlerbehebung können Sie die Protokollierung aktivieren, um eine Protokolldatei für die Ausgabe zu erstellen.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Um einen Speicherort für die Protokolldateien anzugeben, können Sie den Dateipfad in der Befehlszeile angeben.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Der Speicherort der Protokolldatei muss vorhanden sein, sonst wird die Installation abgebrochen.

Siehe die vollständige Liste der Schalter von [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) wenn Sie verschiedene Protokollierungsebenen oder Benutzeroberflächenebenen ausprobieren möchten.

>[!MORELIKETHIS]
>
>[Marketo [!DNL Outlook] Plug-in durch IT deinstallieren](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
