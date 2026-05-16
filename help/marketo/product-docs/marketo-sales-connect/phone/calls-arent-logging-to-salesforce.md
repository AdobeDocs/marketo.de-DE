---
unique-page-id: 14352435
description: Hier erhalten Sie Hilfe, wenn sich Sales Connect-Aufrufe nicht bei Salesforce anmelden. Fehlerbehebung bei Verbindungs- und Aktivitätsprotokollierungseinstellungen.
title: Anrufe werden bei Salesforce nicht protokolliert
exl-id: 99528c1a-7398-442b-81d1-9b5908e35e2f
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/jjTIRKtODlgrMPAoM45wJD2vqFJwfPB56grKn8lRpHY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 133
ht-degree: 3%

---

# -Aufrufe werden nicht bei [!DNL Salesforce] protokolliert {#calls-arent-logging-to-salesforce}

Wenn Sie möchten, dass Ihre Anrufe von Sales Phone automatisch bei [!DNL Salesforce] protokolliert werden, stellen Sie sicher, dass Folgendes vorhanden ist.

Ihr [!DNL Sales Connect] muss über die API-Verbindung mit Ihrem [[!DNL Salesforce] Konto](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md) verbunden sein.

Wenn Sie über die [Web-Anwendung](https://toutapp.com/login) aufrufen, benötigen Sie eine [!DNL Salesforce] ID, die für diesen Kontakt gespeichert ist. [Klicken Sie hier](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/import-a-salesforce-id-into-sales-connect.md) um zu sehen, wie Sie sicherstellen können, dass allen Ihren [!DNL Sales Connect] Kontakten eine [!DNL Salesforce] ID zugeordnet ist.

>[!NOTE]
>
>Stellen Sie sicher, dass Sie in Ihrer Auswahlliste für den Aufgabentyp „Anruf“ haben, um ein genaues und einfaches Reporting in [!DNL Salesforce] zu ermöglichen.

Sobald dies eingerichtet ist, wird eine Aufgabe im Abschnitt Aktivitätsverlauf von [!DNL Salesforce] erstellt.
