---
description: Erfahren Sie, wie die Veeva-CRM-Synchronisation zwischen Marketo Engage und Veeva funktioniert. Führen Sie eine Synchronisierung aus und sehen Sie, was synchronisiert wird, einschließlich Personenkonten und benutzerdefinierter Objekte.
title: Grundlegendes zur [!DNL Veeva] CRM-Synchronisierung
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
TQID: 'https://experienceleague.adobe.com/zgS75Y696DouBdRH4S7sguvmQEzObc5WEdooJXfSh1w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
subfeature_v2:
  - id: f141b8e0-5812-4581-b47d-7322a93e7f28
    internal-label: Veeva CRM
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 9%
---
# Grundlegendes zur [!DNL Veeva] CRM-Synchronisierung {#understanding-the-veeva-crm-sync}

Das Ausführen einer Synchronisierung zwischen Adobe Marketo Engage und dem [!DNL Veeva] CRM dauert nur wenige Schritte.

## Funktionsweise der Synchronisierung {#how-the-sync-works}

Marketo Engage synchronisiert mit [!DNL Veeva] CRM den ganzen Tag, jeden Tag. Jede Synchronisierung dauert einige Zeit, wird 5 Minuten angehalten und dann erneut gestartet.

>[!NOTE]
>
>Die erste Synchronisierung kann Stunden oder sogar Tage dauern, da Marketo Engage die gesamte Datenbank aus [!DNL Veeva] kopiert. Danach dauert jede Synchronisierung in der Regel Minuten (manchmal Sekunden) und synchronisiert nur Daten, die geändert wurden.

![](assets/understanding-the-veeva-sync-1.png)

Die Synchronisierung zwischen [!DNL Veeva] und Marketo Engage erfolgt nur für Kontaktfelder im Benutzerkontoobjekt bidirektional. In diesen Fällen werden Ihre Aktualisierungen bei jeder Änderung, die Sie an [!DNL Veeva] oder Marketo Engage vornehmen, auf beiden Systemen angezeigt. Alle anderen Synchronisierungen werden nur von [!DNL Veeva] nach Marketo Engage durchgeführt. Klicken Sie auf die unten stehenden Links, um Details anzuzeigen.

## Was zwischen Marketo Engage und [!DNL Veeva] synchronisiert wird {#what-is-synced-between-marketo-engage-and-veeva}

* [Personenkonten](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Benutzer
* [Aufrufen und Aufrufen von Schlüsselobjekten](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Was Sie wissen sollten {#things-to-know}

* Die [Anmeldeinformationen, die Sie in Marketo Engage für eingeben [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden verwendet, um Daten zu synchronisieren. Es werden nur Daten einbezogen, auf die diese Anmeldedaten Zugriff haben.

* [!DNL Veeva] CRM basiert auf force.com und das umfangreiche Erlebnis, das Marketo Engage mit der Plattform hat, wird von dieser Synchronisierung übernommen.

* Das Veeva CRM zeigt: Lead, Kontakt, Konten, Geschäftskonten, Opportunity, Kampagne und Aktivität. Sie werden jedoch bei der Synchronisierung mit Marketo Engage nicht unterstützt.
