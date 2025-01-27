---
title: Arbeiten mit Experience Manager Assets
description: Erfahren Sie, wie Sie Bild-Assets aus einem verbundenen AEM Assets-Repository beim Erstellen von Inhalten in Adobe Marketo Engage verwenden.
hide: true
hidefromtoc: true
source-git-commit: 723caafc41da6d4aeb9101bb6f9a999b45d72dd9
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Arbeiten mit Experience Manager-Assets {#work-with-experience-manager-assets}

Wenn _Adobe Experience Manager Assets as a Cloud Service_ mit Adobe Marketo Engage integriert ist, können Sie einfach auf digitale Assets zugreifen, um sie für Ihre Marketing-Inhalte zu verwenden. Während Sie Ihre Inhalte erstellen, können Sie über das Element _[!UICONTROL Assets]_ im linken Navigationsbereich und beim Erstellen von E-Mail-Inhalten auf die Assets zugreifen. Sie können Assets auch direkt von der Marketo Engage in das verbundene _AEM Assets as a Cloud Service_-Repository hochladen. &lt;------- NILESH WIRD FOLGENDES PRÜFEN

>[!NOTE]
>
>Derzeit werden nur Bild-Assets von _Adobe Experience Manager Assets_ in Marketo Engage unterstützt. &lt;---- NILESH WIRD ÜBERPRÜFEN - Änderungen an den Assets müssen über das Adobe Experience Manager Assets Central Repository vorgenommen werden. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

Wenn Sie diese digitalen Assets verwenden, werden die neuesten Änderungen in _Assets as a Cloud Service_ über verknüpfte Verweise automatisch an Live-E-Mail-Kampagnen weitergegeben. Wenn Bilder in _Adobe Experience Manager Assets as a Cloud Service_ gelöscht werden, werden sie in den E-Mails mit einer beschädigten Referenz angezeigt. Wenn Assets, die derzeit auf dem Marketo Engage verwendet werden, geändert oder gelöscht werden, werden die E-Mail-Autoren über die Bildänderungen benachrichtigt. Alle Änderungen an den Assets müssen im Adobe Experience Manager Assets Central Repository vorgenommen werden.

## Verwenden von AEM Assets als Bildquelle {#use-aem-assets-as-the-image-source}

Wenn Ihre Umgebung über eine oder mehrere Assets-Repository-Verbindungen verfügt, können Sie AEM Assets als Quelle für Assets festlegen, wenn Sie Details für eine E-Mail, E-Mail-Vorlage oder ein visuelles Fragment erstellen oder anzeigen.

* Wählen Sie beim Erstellen neuer Inhalte `AEM Assets` als **[!UICONTROL Image Source]**-Element im Dialogfeld aus.

![Wählen Sie AEM Assets als Bildquelle im Dialogfeld „Erstellen“](assets/work-with-experience-manager-assets-1.png){width="400"}

* Wählen Sie beim Öffnen einer vorhandenen Inhaltsressource `AEM Assets` im Bereich _[!UICONTROL Hauptteil]_ auf der rechten Seite.

![Wählen Sie AEM Assets als Bildquelle in den Eigenschaften aus](assets/work-with-experience-manager-assets-2.png){width="700" zoomable="yes"}

## Zugriff auf Assets für das Authoring

>[!IMPORTANT]
>
>Ein Administrator muss Benutzer, die Zugriff auf Assets benötigen, zu den Produktprofilen &quot;Assets Consumer Users“ und/oder &quot;Assets Users“ hinzufügen. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

Klicken Sie im visuellen Inhaltseditor auf das Symbol _Asset-Auswahl_ in der linken Seitenleiste. Dadurch wird das Bedienfeld „Tools“ in eine Liste der verfügbaren Assets im ausgewählten Repository geändert.

![Klicken Sie auf das Symbol Assets-Selektor , um auf die Bild-Assets zuzugreifen](assets/work-with-experience-manager-assets-3.png){width="700" zoomable="yes"}

Wenn Sie über mehr als ein verbundenes AEM-Repository verfügen, klicken Sie auf den Menüpfeil für **[!UICONTROL Repository]**, um das Repository auszuwählen, das Sie verwenden möchten.

![Wählen Sie ein AEM Assets-Repository, um auf die Bild-Assets zuzugreifen](assets/work-with-experience-manager-assets-4.png){width="700" zoomable="yes"}

Es gibt mehrere Methoden zum Hinzufügen eines Bild-Assets zur visuellen Arbeitsfläche:

* Ziehen Sie eine Miniaturansicht per Drag-and-Drop aus dem linken Navigationsbereich.

![Wählen Sie ein AEM Assets-Repository, um auf die Bild-Assets zuzugreifen](assets/work-with-experience-manager-assets-5.png){width="700" zoomable="yes"}

* Fügen Sie der Arbeitsfläche eine Bildkomponente hinzu und klicken Sie auf **[!UICONTROL Durchsuchen]**, um das Dialogfeld _[!UICONTROL Assets auswählen]_ zu öffnen.

  Im Dialogfeld können Sie ein Bild aus dem ausgewählten Repository auswählen.

  Es stehen mehrere Tools zur Verfügung, mit denen Sie das benötigte Asset finden können.

![Verwenden Sie das Tool im Dialogfeld &quot;Assets auswählen“, um ein Bild-Asset zu suchen und auszuwählen](assets/work-with-experience-manager-assets-6.png){width="700" zoomable="yes"}

* Ändern Sie **[!UICONTROL Repository]** oben rechts.

* Klicken Sie **[!UICONTROL oben rechts auf]** Assets verwalten“, um das Assets-Repository in einer anderen Browser-Registerkarte zu öffnen und AEM Assets-Verwaltungstools zu verwenden.

* Klicken Sie oben rechts auf _Ansichtstyp_, um die Anzeige in **[!UICONTROL Listenansicht]**, **[!UICONTROL Rasteransicht]**, **[!UICONTROL Galerieansicht]** oder **[!UICONTROL Wasserfallansicht]** zu ändern.

* Klicken Sie auf _Symbol „Sortierreihenfolge_, um die Sortierreihenfolge zwischen aufsteigender und absteigender Reihenfolge zu ändern.

* Klicken Sie auf **[!UICONTROL Menüpfeil]** Sortieren nach“, um die Sortierkriterien in **[!UICONTROL Name]**, **[!UICONTROL Size]** oder **[!UICONTROL Modified]** zu ändern.

* Klicken Sie _oben links auf_ Filter), um die angezeigten Elemente nach Ihren Kriterien zu filtern.

* Geben Sie im Suchfeld Text ein, um die angezeigten Elemente nach einer Übereinstimmung mit dem Asset-Namen zu filtern.

![Verwenden Sie das Filter- und Suchfeld, um das Asset zu finden](assets/work-with-experience-manager-assets-7.png){width="700" zoomable="yes"}
