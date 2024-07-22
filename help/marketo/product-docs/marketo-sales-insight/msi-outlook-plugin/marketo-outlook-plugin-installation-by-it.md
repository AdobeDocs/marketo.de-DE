---
unique-page-id: 11382815
description: Marketo Outlook-Plugin-Installation durch IT - Marketo Docs - Produktdokumentation
title: Marketo Outlook-Plugin-Installation durch IT
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---

# Marketo Outlook-Plugin-Installation durch IT {#marketo-outlook-plugin-installation-by-it}

Manchmal erfordern Unternehmensrichtlinien, dass das IT-Team alle Software auf den Computern seiner Mitarbeiter installiert. In diesen Fällen führt die IT dies häufig remote mit ihrer eigenen Software durch. Dieses Dokument enthält die Befehlszeilen, die Sie während des Bereitstellungsprozesses als Eingaben verwenden würden, um das Outlook-Plug-in remote zu installieren.

>[!PREREQUISITES]
>
>[Richten Sie ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) den Unternehmensschlüssel ein.

Führen Sie die folgende Befehlszeile als &quot;System&quot;oder als Administrator-Benutzerkonto mit dem /i-Switch aus, um zu installieren.

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
>Der Speicherort der Protokolldatei muss vorhanden sein oder die Installation wird abgebrochen.

Wenn Sie verschiedene Protokollierungsstufen oder Benutzeroberflächenebenen ausprobieren möchten, lesen Sie bitte die vollständige Liste der Switches von [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6).

>[!MORELIKETHIS]
>
>[Marketo Outlook-Plugin deinstallieren von IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
