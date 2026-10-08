---
unique-page-id: 14352514
description: Erfahren Sie, wie Sales Connect mit E-Mail-Deduplizierung umgeht. Erfahren Sie, wie doppelte Kontakte beim Synchronisieren zusammengeführt oder verarbeitet werden.
title: So verarbeitet Sales Connect die Deduplizierung von E-Mail-Adressen
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
TQID: 'https://experienceleague.adobe.com/gO6I2rCotAEDOGQNdRleeJbqMIix1wQizZe84JZSLPs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: ab9cc269-26ac-5c58-b645-e0736aefe9f3
    internal-label: Marketo Sales Connect
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 6%
---
# Wie [!DNL Sales Connect] mit der E-Mail-Deduplizierung umgeht {#how-sales-connect-handles-email-de-duping}

Wenn Sie [eine CSV)-Datei in [!DNL Sales Connect] hochladen](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) führen wir alle ähnlichen Kontakte in der CSV zusammen, bevor der Import stattfindet.

Wir tun dies basierend auf wie E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, führen wir sie zu einem Kontakt zusammen.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, werden wir ihn nicht zusammenführen.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der sich bereits in Ihrer Datenbank befindet, können Sie ihn nicht hinzufügen.
