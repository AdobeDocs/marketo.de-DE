---
description: Prioritätsüberschreibungen für Trigger-Kampagnen - Marketo-Dokumente - Produktdokumentation
title: Prioritätsüberschreibungen für Trigger-Kampagnen
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Prioritätsüberschreibungen für Trigger-Kampagnen {#priority-override-for-trigger-campaigns}

Administratoren können die von Marketo Engage festgelegte Priorität für Trigger-Kampagnen außer Kraft setzen, um Prioritäten zu setzen, die besser auf Geschäftsziele abgestimmt sind.

>[!NOTE]
>
>Diese Funktion ist nur für Trigger-Kampagnen und für Benutzende verfügbar, denen die [ &quot;Trigger-Kampagnenpriorität bearbeiten“ gewährt ](#grant-priority-override-access).

>[!CAUTION]
>
>Es wird dringend empfohlen, diese Funktion in einer begrenzten Anzahl geschäftskritischer Kampagnen zu verwenden (maximal 25 wird empfohlen). Die lockere Verwendung der Funktion auf einer großen Menge kann sich negativ auf die gesamte Kampagnenausführung auswirken.

## Zugriff auf Prioritätsüberschreibungen gewähren {#grant-priority-override-access}

>[!NOTE]
>
>Nur Admins oder Benutzende mit Admin-Zuständigkeiten sollten Zugriff auf die Kampagnenprioritätsüberschreibungen haben.

1. Klicken Sie im [!UICONTROL Admin]-Bereich auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Klicken Sie auf die **[!UICONTROL Rollen]**, wählen Sie den Benutzer aus, dem Sie Zugriff gewähren möchten, und klicken Sie dann auf **[!UICONTROL Rolle bearbeiten]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Wählen [!UICONTROL &#x200B; unter „Marketing-Aktivitäten &#x200B;]&quot; die Option **[!UICONTROL Trigger-Kampagnenpriorität bearbeiten]** aus. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Priorität aufheben {#override-priority}

1. Suchen Sie Ihren Trigger Campaign. Klicken Sie mit der rechten Maustaste darauf und wählen Sie **[!UICONTROL Kampagnenpriorität überschreiben]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Klicken Sie auf den **[!UICONTROL Kampagnenpriorität überschreiben]**, um ihn zu aktivieren. Wählen Sie eine neue Prioritätsstufe aus und klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Die neue Prioritätsstufe wird auf der Registerkarte Zeitplan angezeigt.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Sie können die Standardpriorität Ihrer Kampagne in der [!UICONTROL Kampagnenwarteschlange“ unter &#x200B;]Marketing[!UICONTROL Aktivitäten) &#x200B;]. Um die Ausführungsrate zu erhöhen, empfehlen wir, die Kampagnenpriorität eine Ebene höher als die Standardpriorität festzulegen.
>* Die Priorität für Benutzereinstellungen gilt nur für neue Personen, die sich für die Kampagne qualifizieren. Personen, die sich bereits in der Warteschlange befinden, sind davon nicht betroffen.
>* Prioritätsüberschreibungen werden im [Audit-Protokoll](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"} erfasst.
