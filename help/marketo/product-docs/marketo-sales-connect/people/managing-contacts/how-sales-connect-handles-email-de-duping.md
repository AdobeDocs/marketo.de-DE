---
unique-page-id: 14352514
description: Vorgehensweise von Sales Connect bei der E-Mail-Deduplizierung - Marketing Docs - Produktdokumentation
title: Vorgehensweise von Sales Connect bei der Deduplizierung per E-Mail
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Vorgehensweise von Sales Connect bei der Deduplizierung per E-Mail {#how-sales-connect-handles-email-de-duping}

Wenn Sie eine CSV [-Datei in Sales Connect](http://docs.marketo.com/x/VADb) hochladen, führen wir alle Kontakte wie Kontakte in der CSV zusammen, bevor der Import stattfindet.

Wir machen dies auf der Grundlage einer ähnlichen E-Mail-Adresse. Wenn es also zwei identische E-Mail-Adressen gibt, werden diese zu einem einzigen Kontakt zusammengeführt.

Wenn Sie später versuchen, denselben Kontakt manuell hinzuzufügen/hochzuladen, wird er nicht zusammengeführt.

Wenn Sie versuchen, einen Kontakt hinzuzufügen, der bereits in Ihrer Datenbank vorhanden ist, verhindern wir, dass Sie ihn hinzufügen.

