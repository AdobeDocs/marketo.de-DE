---
description: Wie werden mit Sales Insight-Aktionen E-Mail-Deduplizierung behandelt - Marketo Docs - Produktdokumentation
title: Wie behandelt Sales Insight-Aktionen das Deduplizieren von E-Mails?
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Wie werden E-Mail-Deduplizierungen in Sales Insight-Aktionen behandelt? {#how-does-sales-insight-actions-handle-email-de-duping}

Wann du bist [Hochladen einer CSV-Datei](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) in Sales Insight-Aktionen zusammenführen, führen wir alle ähnlichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Dies geschieht anhand einer ähnlichen E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der bereits in Ihrer Datenbank gespeichert ist, wird Ihnen dies nicht möglich sein.
