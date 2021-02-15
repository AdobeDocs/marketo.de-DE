---
unique-page-id: 14352514
description: Vorgehensweise von Sales Connect bei der E-Mail-Deduplizierung - Marketing Docs - Produktdokumentation
title: Vorgehensweise von Sales Connect bei der Deduplizierung per E-Mail
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Vorgehensweise von Sales Connect bei der E-Mail-Deduplizierung {#how-sales-connect-handles-email-de-duping}

Wenn Sie [eine CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)-Datei in Sales Connect hochladen, führen wir alle ähnlichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Wir machen dies auf der Grundlage einer ähnlichen E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, werden diese zu einem einzigen Kontakt zusammengeführt.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, wird er nicht zusammengeführt.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der bereits in Ihrer Datenbank vorhanden ist, verhindern wir, dass Sie ihn hinzufügen.
