---
description: Grundlegendes zur  [!DNL Veeva] -CRM-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur  [!DNL Veeva] -CRM-Synchronisierung
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Grundlegendes zur [!DNL Veeva] CRM-Synchronisierung {#understanding-the-veeva-crm-sync}

In wenigen einfachen Schritten ist es einfach, eine Synchronisierung zwischen Adobe Marketo Engage und dem [!DNL Veeva] CRM durchzuführen.

## Funktionsweise der Synchronisierung {#how-the-sync-works}

Marketo Engage synchronisiert mit [!DNL Veeva] CRM den ganzen Tag, jeden Tag. Jede Synchronisierung dauert einige Zeit, wird 5 Minuten angehalten und dann erneut gestartet.

>[!NOTE]
>
>Die erste Synchronisierung kann Stunden oder sogar Tage dauern, da Marketo Engage die gesamte Datenbank aus [!DNL Veeva] kopiert. Danach dauert jede Synchronisierung in der Regel Minuten (manchmal Sekunden) und synchronisiert nur Daten, die geändert wurden.

![](assets/understanding-the-veeva-sync-1.png)

Die Synchronisierung zwischen [!DNL Veeva] und Marketo Engage erfolgt nur für Kontaktfelder im Benutzerkontoobjekt bidirektional. In diesen Fällen werden Ihre Aktualisierungen bei jeder Änderung, die Sie an [!DNL Veeva] oder Marketo Engage vornehmen, auf beiden Systemen angezeigt. Alle anderen Synchronisierungen werden nur von [!DNL Veeva] nach Marketo Engage durchgeführt. Klicken Sie auf die unten stehenden Links, um Details zu jedem anzuzeigen.

## Was zwischen Marketo Engage und [!DNL Veeva] synchronisiert wird {#what-is-synced-between-marketo-engage-and-veeva}

* [Personenkonten](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Benutzer
* [Aufruf- und Aufrufschlüsselobjekte](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Was man wissen muss {#things-to-know}

* Die [Anmeldeinformationen, die Sie in Marketo Engage für eingeben [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden verwendet, um Daten zu synchronisieren. Nur Daten, auf die diese Anmeldeinformationen Zugriff haben, werden einbezogen.

* [!DNL Veeva] CRM basiert auf force.com und das umfangreiche Erlebnis, das Marketo Engage mit der Plattform hat, wird von dieser Synchronisierung übernommen.

* Das Veeva CRM zeigt: Lead, Kontakt, Konten, Geschäftskonten, Opportunity, Kampagne und Aktivität. Sie werden jedoch bei der Synchronisierung mit Marketo Engage nicht unterstützt.
