---
unique-page-id: 11382829
description: Erfahren Sie, wie IT das Marketo Outlook-Plug-in deinstallieren kann. Entfernen Sie bei Bedarf das Add-in von Benutzer-Computern.
title: Marketo [!DNL Outlook] Plugin durch IT deinstallieren
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/p2CjKHycrJRHLpphyn2qsUEKP-dWh2OlTezwrOn9Ljw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 2%

---

# Marketo [!DNL Outlook]-Plug-in durch IT deinstallieren {#marketo-outlook-plugin-uninstall-by-it}

So kann die IT das Marketo [!DNL Outlook]-Plug-in remote deinstallieren.

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
>Wenn Sie das Plug-in remote deinstallieren, wird [!DNL Outlook] auf dem Computer des Benutzers erzwungen.

Siehe die vollständige Liste der Schalter von [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) wenn Sie verschiedene Protokollierungsebenen oder Benutzeroberflächenebenen ausprobieren möchten.
