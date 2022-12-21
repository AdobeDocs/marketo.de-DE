---
unique-page-id: 14352514
description: So verarbeitet Sales Connect das Deduplizieren von E-Mails - Marketo-Dokumente - Produktdokumentation
title: Vorgehensweise von Sales Connect beim Deduplizieren von E-Mails
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Vorgehensweise von Sales Connect beim Deduplizieren von E-Mails {#how-sales-connect-handles-email-de-duping}

Wann du bist [Hochladen einer CSV-Datei](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) in Sales Connect, führen wir alle gleichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Dies geschieht anhand einer ähnlichen E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der bereits in Ihrer Datenbank gespeichert ist, wird Ihnen dies nicht möglich sein.
