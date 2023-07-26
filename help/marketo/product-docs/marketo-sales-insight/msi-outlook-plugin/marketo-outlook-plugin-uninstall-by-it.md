---
unique-page-id: 11382829
description: Marketo Outlook-Plugin deinstallieren durch IT - Marketo Docs - Produktdokumentation
title: Marketo Outlook-Plug-in-Deinstallation durch IT
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 2%

---

# Marketo Outlook-Plug-in-Deinstallation durch IT {#marketo-outlook-plugin-uninstall-by-it}

So kann IT das Marketo Outlook-Plugin remote deinstallieren.

Führen Sie die folgende Befehlszeile als &quot;System&quot;oder ein Administrator-Benutzerkonto mit dem /x-Switch aus, um es zu deinstallieren.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Zur Fehlerbehebung können Sie die Protokollierung aktivieren, um eine Protokolldatei für die Ausgabe zu erstellen.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Um einen Speicherort für die Protokolldateien anzugeben, können Sie den Dateipfad in der Befehlszeile angeben.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Beispiel**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Durch das Deinstallieren des Plug-ins wird Outlook auf dem Computer des Benutzers erzwungen.

Bitte lesen Sie [Vollständige Liste der Switches von Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) , wenn Sie verschiedene Protokollierungsstufen oder Benutzeroberflächen-Ebenen ausprobieren möchten.
