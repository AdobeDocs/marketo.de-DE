---
unique-page-id: 1147027
description: Person mit dem SFDC synchronisieren - Marketing Docs - Produktdokumentation
title: Person mit dem SFDC synchronisieren
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Person mit dem SFDC synchronisieren {#sync-person-to-sfdc}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Nur verfügbar, wenn in Salesforce integriert.

## Übersicht {#overview}

Mit diesem Flussschritt fügen Sie von Marketo erstellte Personen als Interessenten in Ihre Salesforce CRM ein.

![](assets/sync-person-to-sfdc.png)

## Nutzung {#usage}

1. Standardmäßig weist dieser Flussschritt Interessenteninhabern basierend auf den Salesforce-Regeln für die automatische Zuweisung zu.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Für Salesforce müssen die Felder &quot;Firma&quot;und &quot;Nachname&quot;ausgefüllt sein. Andernfalls wird der Interessentendatensatz abgelehnt.

1. Sie können einen bestimmten Salesforce-Benutzer oder eine Interessentenwarteschlange als Interessentenbesitzer festlegen.

   ![](assets/sync-person-to-sfdc-2.png)

   Bei Verwendung dieses Flussschritts wird die Person sofort als Salesforce-Lead synchronisiert und muss nicht auf die regelmäßige Synchronisierung warten.

   >[!CAUTION]
   >
   >Salesforce lässt die Zuweisung von &quot;Kontakten&quot;zu Interessentenwarteschlangen nicht zu. In diesem Fall wird Marketo ein Duplikat &quot;Lead&quot; in Salesforce erstellen.

