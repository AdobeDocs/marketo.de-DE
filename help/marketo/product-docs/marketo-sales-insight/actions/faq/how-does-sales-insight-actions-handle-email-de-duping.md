---
description: Wie werden mit Sales Insight-Aktionen E-Mail-Deduplizierung behandelt - Marketo Docs - Produktdokumentation
title: Wie behandelt Sales Insight-Aktionen das Deduplizieren von E-Mails?
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Wie werden E-Mail-Deduplizierungen in Sales Insight-Aktionen behandelt? {#how-does-sales-insight-actions-handle-email-de-duping}

Wenn Sie eine CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md)-Datei [ in Sales Insight-Aktionen hochladen, führen wir alle wie Kontakte in der CSV zusammen, bevor der Import erfolgt.

Dies geschieht anhand einer ähnlichen E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der bereits in Ihrer Datenbank gespeichert ist, wird Ihnen dies nicht möglich sein.
