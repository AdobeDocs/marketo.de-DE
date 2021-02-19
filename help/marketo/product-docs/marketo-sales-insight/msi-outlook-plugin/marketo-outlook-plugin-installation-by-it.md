---
unique-page-id: 11382815
description: Installation des Marketo Outlook Plugins durch IT - Marketing Docs - Produktdokumentation
title: Installation des Marketo Outlook Plugins durch IT
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# Marketo Outlook Plugin Installation by IT {#marketo-outlook-plugin-installation-by-it}

Manchmal erfordern die Richtlinien des Unternehmens, dass sein IT-Team alle Software auf den Computern seiner Mitarbeiter installiert. In diesen Fällen erfolgt dies oft remote mithilfe einer eigenen Bereitstellungssoftware. Dieses Dokument enthält die Befehlszeilen, die Sie während des Bereitstellungsprozesses verwenden würden, um das Plugin für Aussichten remote zu installieren.

>[!PREREQUISITES]
>
>[Legen Sie ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) den Enterprise-Schlüssel fest.

Führen Sie die folgende Befehlszeile als &quot;System&quot;oder als Administratorkonto mit dem /i-Switch aus, um die Installation durchzuführen.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Zur Fehlerbehebung können Sie die Protokollierung aktivieren, um eine Ausgabsprotokolldatei zu erstellen.

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
>Der Speicherort der Protokolldatei muss vorhanden sein, damit die Datenspeicherung abgebrochen werden kann.

Bitte lesen Sie die vollständige Liste der Switches](https://support.microsoft.com/en-us/kb/227091) von Microsoft, wenn Sie verschiedene Protokollierungsstufen oder Benutzeroberflächenebenen ausprobieren möchten.[

>[!MORELIKETHIS]
>
>[Marketo Outlook Plugin Uninstall by IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
