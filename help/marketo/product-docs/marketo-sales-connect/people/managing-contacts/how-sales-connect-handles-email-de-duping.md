---
unique-page-id: 14352514
description: Erfahren Sie, wie Sales Connect mit E-Mail-Deduplizierung umgeht. Erfahren Sie, wie doppelte Kontakte beim Synchronisieren zusammengeführt oder verarbeitet werden.
title: Handhaben von E-Mail-Deduplizierung durch Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '103'
ht-degree: 5%

---

# Wie [!DNL Sales Connect] mit der E-Mail-Deduplizierung umgeht {#how-sales-connect-handles-email-de-duping}

Wenn Sie eine CSV[-Datei in &#x200B;](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) hochladen[!DNL Sales Connect] führen wir alle ähnlichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Wir tun dies basierend auf wie E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der sich bereits in Ihrer Datenbank befindet, können Sie ihn nicht hinzufügen.
