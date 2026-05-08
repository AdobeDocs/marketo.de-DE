---
description: Erfahren Sie, wie die Veeva-CRM-Synchronisation zwischen Marketo Engage und Veeva funktioniert. Führen Sie eine Synchronisierung aus und sehen Sie, was synchronisiert wird, einschließlich Personenkonten und benutzerdefinierter Objekte.
title: Grundlegendes zur  [!DNL Veeva] -CRM-Synchronisierung
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '251'
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

* Die [Anmeldeinformationen, die Sie in Marketo Engage für eingeben [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden verwendet, um Daten zu synchronisieren. Es werden nur Daten einbezogen, auf die mit diesen Anmeldedaten zugegriffen werden kann.

* [!DNL Veeva] CRM basiert auf force.com und das umfangreiche Erlebnis, das Marketo Engage mit der Plattform hat, wird von dieser Synchronisierung übernommen.

* Das Veeva CRM zeigt: Lead, Kontakt, Konten, Geschäftskonten, Opportunity, Kampagne und Aktivität. Sie werden jedoch bei der Synchronisierung mit Marketo Engage nicht unterstützt.
