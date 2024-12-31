---
description: Veeva CRM-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Verstehen der Veeva CRM-Synchronisierung
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Verstehen der Veeva CRM-Synchronisierung {#understanding-the-veeva-crm-sync}

Mit nur wenigen Handgriffen ist es einfach, eine Synchronisation zwischen Adobe Marketo Engage und dem Veeva CRM durchzuführen.

## Funktionsweise der Synchronisierung {#how-the-sync-works}

Marketo Engage synchronisiert mit Veeva CRM den ganzen Tag, jeden Tag. Jede Synchronisierung dauert einige Zeit, wird 5 Minuten angehalten und dann erneut gestartet.

>[!NOTE]
>
>Die erste Synchronisation kann Stunden oder sogar Tage dauern, da Marketo Engage die gesamte Datenbank von Veeva kopiert. Danach dauert jede Synchronisierung in der Regel Minuten (manchmal Sekunden) und synchronisiert nur Daten, die geändert wurden.

![](assets/understanding-the-veeva-sync-1.png)

Die Synchronisation zwischen Veeva und Marketo Engage erfolgt nur bidirektional für Kontaktfelder im Benutzerkontoobjekt. In diesen Fällen werden Ihre Aktualisierungen in beiden Systemen angezeigt, wenn Sie Änderungen in Veeva oder Marketo Engage vornehmen. Alle anderen Synchronisationen werden nur von Veeva nach Marketo Engage durchgeführt. Klicken Sie auf die unten stehenden Links, um Details zu jedem anzuzeigen.

## Was zwischen Marketo Engage und Veeva synchronisiert wird {#what-is-synced-between-marketo-engage-and-veeva}

* [Personenkonten](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Benutzer
* [Aufruf- und Aufrufschlüsselobjekte](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Was man wissen muss {#things-to-know}

* Die [Anmeldeinformationen, die Sie auf Marketo Engage für Veeva eingeben](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden verwendet, um Daten zu synchronisieren. Nur Daten, auf die diese Anmeldeinformationen Zugriff haben, werden einbezogen.

* Veeva CRM basiert auf force.com und das Rich-Experience-Marketo Engage mit der Plattform wird von dieser Synchronisation übernommen.

* Das Veeva CRM zeigt: Lead, Kontakt, Konten, Geschäftskonten, Opportunity, Kampagne und Aktivität. Sie werden jedoch bei der Synchronisierung mit Marketo Engage nicht unterstützt.
