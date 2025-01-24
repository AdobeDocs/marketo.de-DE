---
title: Arbeiten mit Experience Manager Assets
description: Erfahren Sie, wie Sie Bild-Assets aus einem verbundenen AEM Assets-Repository beim Erstellen von Inhalten in Adobe Marketo Engage verwenden können.
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Arbeiten mit Experience Manager-Assets

Wenn Adobe Experience Manager Assets as a Cloud Service mit Adobe Marketo Engage integriert ist, können Sie auf einfache Weise digitale Assets für die Verwendung in Ihren Marketing-Inhalten ermitteln und darauf zugreifen. Während Sie Ihre Inhalte erstellen, können Sie über das Element _[!UICONTROL Assets]_ im linken Navigationsbereich und beim Erstellen von E-Mail-Inhalten für eine Konto-Journey auf die Assets zugreifen. Sie können Assets auch direkt aus Adobe Journey Optimizer B2B edition in das verbundene AEM Assets as a Cloud Service-Repository hochladen.

>[!NOTE]
>
>Derzeit werden in Adobe Journey Optimizer B2B edition nur Bild-Assets aus Adobe Experience Manager Assets unterstützt. Änderungen an den Assets müssen über das zentrale Adobe Experience Manager Assets-Repository vorgenommen werden. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

Wenn Sie diese digitalen Assets verwenden, werden die neuesten Änderungen in Assets as a Cloud Service automatisch über verknüpfte Verweise in Live-E-Mail-Kampagnen übertragen. Wenn Bilder in Adobe Experience Manager Assets as a Cloud Service gelöscht werden, werden sie in den E-Mails mit einer beschädigten Referenz angezeigt. Wenn Assets, die derzeit in Account Journey verwendet werden, geändert oder gelöscht werden, werden die Journey-Autoren über die Bildänderungen und die Liste der Journey, die das Image verwenden, benachrichtigt. Alle Änderungen an den Assets müssen im Adobe Experience Manager Assets Central Repository vorgenommen werden.

## Verwenden von AEM Assets als Bildquelle

Wenn Ihre Umgebung über eine oder mehrere Assets-Repository-Verbindungen verfügt, können Sie AEM Assets als Quelle für Assets festlegen, wenn Sie Details für eine E-Mail, E-Mail-Vorlage oder ein visuelles Fragment erstellen oder anzeigen.

* Wählen Sie beim Erstellen eines neuen Inhalts im Dialogfeld `AEM Assets` als **[!UICONTROL Image Source]**-Element aus.

SCREENSHOT

* Wenn Sie eine vorhandene Inhaltsressource öffnen, wählen Sie `AEM Assets` im Bereich _[!UICONTROL Hauptteil]_ auf der rechten Seite.

SCREENSHOT

## Zugriff auf Assets für das Authoring

>[!IMPORTANT]
>
>Ein Administrator muss Benutzende, die Zugriff auf Assets benötigen, zu den Produktprofilen &quot;Assets Consumer Users“ oder/und &quot;Assets Users“ hinzufügen. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

Klicken Sie im visuellen Inhaltseditor auf das Symbol _Asset-Auswahl_ in der linken Seitenleiste. Dadurch wird das Bedienfeld „Tools“ in eine Liste der verfügbaren Assets im ausgewählten Repository geändert.

SCREENSHOT

Wenn Sie über mehr als ein verbundenes AEM-Repository verfügen, klicken Sie auf den Menüpfeil für **[!UICONTROL Repository]**, um das Repository auszuwählen, das Sie verwenden möchten.

SCREENSHOT

Es gibt mehrere Methoden zum Hinzufügen eines Bild-Assets zur visuellen Arbeitsfläche:

* Ziehen Sie eine Miniaturansicht per Drag-and-Drop aus dem linken Navigationsbereich.

SCREENSHOT

* Fügen Sie der Arbeitsfläche eine Bildkomponente hinzu und klicken Sie auf **[!UICONTROL Durchsuchen]**, um das Dialogfeld _[!UICONTROL Assets auswählen]_ zu öffnen.

  Im Dialogfeld können Sie ein Bild aus dem ausgewählten Repository auswählen.

  Es stehen mehrere Tools zur Verfügung, mit denen Sie das benötigte Asset finden können.

SCREENSHOT

* Ändern Sie **[!UICONTROL Repository]** oben rechts.

* Klicken Sie **[!UICONTROL oben rechts auf]** Assets verwalten“, um das Assets-Repository in einer anderen Browser-Registerkarte zu öffnen und AEM Assets-Verwaltungstools zu verwenden.

* Klicken Sie oben rechts auf _Ansichtstyp_, um die Anzeige in **[!UICONTROL Listenansicht]**, **[!UICONTROL Rasteransicht]**, **[!UICONTROL Galerieansicht]** oder **[!UICONTROL Wasserfallansicht]** zu ändern.

* Klicken Sie auf _Symbol „Sortierreihenfolge_, um die Sortierreihenfolge zwischen aufsteigender und absteigender Reihenfolge zu ändern.

* Klicken Sie auf **[!UICONTROL Menüpfeil]** Sortieren nach“, um die Sortierkriterien in **[!UICONTROL Name]**, **[!UICONTROL Size]** oder **[!UICONTROL Modified]** zu ändern.

* Klicken Sie _oben links auf_ Filter), um die angezeigten Elemente nach Ihren Kriterien zu filtern.

* Geben Sie im Suchfeld Text ein, um die angezeigten Elemente nach einer Übereinstimmung mit dem Asset-Namen zu filtern.

SCREENSHOT
