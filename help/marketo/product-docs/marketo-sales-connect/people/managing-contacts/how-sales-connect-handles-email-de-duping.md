---
unique-page-id: 14352514
description: Wie Sales Connect mit der E-Mail-Deduplizierung umgeht - Marketo-Dokumente - Produktdokumentation
title: Handhabung der E-Mail-Deduplizierung durch Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Handhabung der E-Mail-Deduplizierung durch Sales Connect {#how-sales-connect-handles-email-de-duping}

Wenn Sie eine CSV[-Datei in Sales Connect hochladen](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) führen wir alle ähnlichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Wir tun dies basierend auf wie E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der sich bereits in Ihrer Datenbank befindet, können Sie ihn nicht hinzufügen.
