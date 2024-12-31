---
unique-page-id: 11382829
description: Marketo Outlook-Plug-in durch IT deinstallieren - Marketo-Dokumente - Produktdokumentation
title: Marketo Outlook-Plug-in durch IT deinstallieren
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# Marketo Outlook-Plug-in durch IT deinstallieren {#marketo-outlook-plugin-uninstall-by-it}

So kann die IT das Marketo Outlook-Plug-in remote deinstallieren.

Führen Sie die folgende Befehlszeile als „System“ oder als administratives Benutzerkonto mit dem Schalter /x zur Deinstallation aus.

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
>Wenn Sie das Plug-in remote deinstallieren, wird Outlook auf dem Computer des Benutzers zwangsweise geschlossen.

Siehe die vollständige Liste der Schalter von [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) wenn Sie verschiedene Protokollierungsebenen oder Benutzeroberflächenebenen ausprobieren möchten.
