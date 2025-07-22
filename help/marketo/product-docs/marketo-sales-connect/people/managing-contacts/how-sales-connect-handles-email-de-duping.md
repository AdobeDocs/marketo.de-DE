---
unique-page-id: 14352514
description: Wie Sales Connect mit der E-Mail-Deduplizierung umgeht - Marketo-Dokumente - Produktdokumentation
title: Handhabung der E-Mail-Deduplizierung durch Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 0%

---

# Wie [!DNL Sales Connect] mit der E-Mail-Deduplizierung umgeht {#how-sales-connect-handles-email-de-duping}

Wenn Sie eine CSV[-Datei in ](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) hochladen[!DNL Sales Connect] führen wir alle ähnlichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Wir tun dies basierend auf wie E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der sich bereits in Ihrer Datenbank befindet, können Sie ihn nicht hinzufügen.
