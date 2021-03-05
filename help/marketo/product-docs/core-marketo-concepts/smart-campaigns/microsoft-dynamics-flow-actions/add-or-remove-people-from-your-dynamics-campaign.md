---
description: hinzufügen oder entfernen Sie Personen aus Ihrer Dynamics-Kampagne - Marketing Docs - Produktdokumentation
title: hinzufügen oder entfernen Sie Personen aus Ihrer Kampagne "Dynamics"
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# hinzufügen oder entfernen Sie Personen aus Ihrer Dynamics Kampagne {#add-or-remove-people-from-your-dynamics-campaign}

## hinzufügen auf Dynamics Kampagne {#add-to-dynamics-campaign}

Dieser Flussschritt kann in Marketo Smart-Kampagnen verwendet werden, um Personen als Interessenten oder Ansprechpartner in einer Microsoft-Kampagne hinzuzufügen. Wenn der Interessent noch nicht in Dynamics vorhanden ist, wird er automatisch synchronisiert und der Kampagne hinzugefügt.

>[!NOTE]
>
>Diese Flussaktion ist nur für Trigger-Kampagnen verfügbar.

Wählen Sie in Ihrer intelligenten Kampagne die Dynamics Kampagne aus, der Sie Ihre Mitarbeiter hinzufügen möchten.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Wenn Sie keine Dynamics-Kampagne in der Liste Kampagne sehen können:
>
>* Stellen Sie sicher, dass die Synchronisierung der Kampagne funktioniert.
>* Die Kampagne ist in Microsoft Dynamics nicht aktiv


Das System erstellt automatisch eine Kampagne-spezifische statische Marketing-Liste, jeweils für Kontakte und Kontakte, die der Person hinzugefügt werden. Es handelt sich um eine einmalige Aktion, bei der einmal für eine nachfolgende Synchronisierung mit der Kampagne dieselbe Marketing-Liste verwendet wird. Der für den Namen der statischen Marketing-Liste verwendete Benennungsstandard lautet `Mkto-leads-<uniqueID>` für Interessenten und `Mkto-contacts-<uniqueID>` für Kontakte.

Die Verknüpfung dieser marketinggenerierten Marketing-Listen mit anderen Kampagnen könnte zu Verwirrung führen. Beispiel: die einer Kampagne hinzugefügt wird, würde auch dazu führen, dass die zweite Kampagne hinzugefügt wird. Ebenso wird auch eine Trennung der von Marketo generierten Marketing-Liste von der Kampagne in Dynamics nicht empfohlen.

## Aus Dynamics-Kampagne {#remove-from-dynamics-campaign} entfernen

Dieser Flussschritt kann in Marketo Smart-Kampagnen zum Entfernen von Personen aus einer Microsoft-Kampagne verwendet werden. Dadurch werden nur die Interessenten aus einer Kampagne entfernt, die der Kampagne zuvor über die Flussaktion &quot;Zur Microsoft-Kampagne hinzugefügt&quot;hinzugefügt wurden.

>[!NOTE]
>
>Diese Flussaktion ist nur für Trigger-Kampagnen verfügbar.

Wählen Sie in Ihrer intelligenten Kampagne die Dynamics Kampagne aus, aus der Sie Ihre Mitarbeiter entfernen möchten.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Wenn Sie keine Dynamics-Kampagne in der Kampagne-Liste sehen:
>
>* Stellen Sie sicher, dass die Synchronisierung der Kampagne funktioniert.
>* Die Kampagne ist in Microsoft Dynamics nicht aktiv

