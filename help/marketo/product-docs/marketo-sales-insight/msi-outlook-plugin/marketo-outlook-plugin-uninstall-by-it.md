---
unique-page-id: 11382829
description: Marketo Outlook Plugin Uninstall by IT - Marketing Docs - Produktdokumentation
title: Marketo Outlook Plugin Uninstall by IT
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Marketo Outlook Plugin Uninstall by IT {#marketo-outlook-plugin-uninstall-by-it}

So kann IT das Marketo Outlook Plugin remote deinstallieren.

Führen Sie die folgende Befehlszeile als &quot;System&quot;oder als ein Administratorkonto mit dem /x-Switch aus, um die Deinstallation durchzuführen.
`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Beispiel**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Zur Fehlerbehebung können Sie die Protokollierung aktivieren, um eine Ausgabsprotokolldatei zu erstellen.  `<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Beispiel**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Um einen Speicherort für die Protokolldateien anzugeben, können Sie den Dateipfad in der Befehlszeile angeben.  `<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Beispiel**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Durch die entfernte Deinstallation des Plug-Ins wird Outlook auf dem Computer des Benutzers erzwungen.

Bitte lesen Sie die vollständige Liste der Switches[ von Microsoft, wenn Sie verschiedene Protokollierungsstufen oder Benutzeroberflächenebenen ausprobieren möchten.](https://support.microsoft.com/en-us/kb/227091)