---
description: Prioritätsüberschreibungen für Trigger-Kampagnen - Marketo-Dokumente - Produktdokumentation
title: Prioritätsüberschreibungen für Trigger-Kampagnen
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 8%

---

# Prioritätsüberschreibungen für Trigger-Kampagnen {#priority-override-for-trigger-campaigns}

AdministratorInnen können die von Marketo festgelegte Priorität für Trigger-Kampagnen außer Kraft setzen, um Prioritäten festzulegen, die besser mit den Geschäftszielen übereinstimmen.

>[!NOTE]
>
>Diese Funktion steht nur Trigger-Kampagnen und Benutzern zur Verfügung, denen die Funktion [Berechtigung &quot;Trigger-Kampagnenpriorität bearbeiten&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>Es wird dringend empfohlen, diese Funktion für eine begrenzte Anzahl geschäftskritischer Kampagnen zu verwenden (25 ist das empfohlene Maximum). Die lockere Verwendung der Funktion auf einer großen Menge kann die Ausführung der Kampagne insgesamt beeinträchtigen.

## Gewähren der Priorität Zugriff überschreiben {#grant-priority-override-access}

>[!NOTE]
>
>Nur Administratoren oder Benutzer mit Administratorrechten sollten über die Kampagnenpriorität verfügen, um den Zugriff zu überschreiben.

1. Im [!UICONTROL Admin] Bereich, klicken Sie **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Klicken Sie auf **[!UICONTROL Rollen]** auf, wählen Sie den Benutzer aus, dem Sie Zugriff gewähren möchten, und klicken Sie auf **[!UICONTROL Rolle bearbeiten]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. under [!UICONTROL Auf Marketing-Aktivitäten zugreifen]auswählen **[!UICONTROL Trigger-Kampagnenpriorität bearbeiten]**. Klicks **[!UICONTROL Speichern]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Priorität aufheben {#override-priority}

1. Suchen Sie die Trigger-Kampagne. Klicken Sie mit der rechten Maustaste darauf und wählen Sie **[!UICONTROL Kampagnenpriorität überschreiben]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Klicken Sie auf **[!UICONTROL Kampagnenpriorität überschreiben]** zu aktivieren. Wählen Sie eine neue Prioritätsstufe aus und klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Die neue Prioritätsstufe wird im Tab Planung angezeigt.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Die Standardpriorität Ihrer Kampagne können Sie im [!UICONTROL Kampagnenwarteschlange] under [!UICONTROL Marketingaktivitäten]. Um die Ausführungsrate zu steigern, empfehlen wir, die Kampagnenpriorität auf eine Ebene zu setzen, die über der Standardeinstellung liegt.
>* Die Priorität des Benutzersatzes gilt nur für neue Personen, die sich für die Kampagne qualifizieren. Personen, die sich bereits in der Warteschlange befinden, sind davon nicht betroffen.
>* Prioritätsüberschreibungen werden in [Audit-Protokoll](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).
