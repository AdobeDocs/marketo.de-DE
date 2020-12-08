---
unique-page-id: 10095307
description: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse - Marketing-Dokumente - Produktdokumentation
title: Benutzerdefinierte Sync-Filterregeln für eine E-Mail-Adresse
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Benutzerdefinierte Sync-Filterregeln für eine E-Mail-Adresse {#custom-sync-filter-rules-for-an-email-address}

Um die Synchronisierung von Datensätzen ohne E-Mail-Adresse zu verhindern, befolgen Sie diese Regeln.

* Wenn ein Interessent erstellt wird ODER wenn das E-Mail-Adressfeld des Interessenten aktualisiert wird, prüfen Sie, ob der Interessent eine E-Mail-Adresse hat, und ändern Sie, falls dies der Fall ist, die Option Synchronisierung zu Mkto zu **True**. Andernfalls **False**

* Wenn ein Kontakt erstellt wird ODER wenn das Feld der E-Mail-Adresse des Kontakts aktualisiert wird, prüfen Sie, ob der Kontakt eine E-Mail-Adresse hat. Ändern Sie in diesem Fall die Option Synchronisierung zu Mkto zu **True** und die Option Synchronisierung zu Mkto zu **True** im Kontodatensatz. Andernfalls **False**

* Wenn das Feld &quot;Firma des Kontakts&quot;(parentcustomerid) aktualisiert wird, prüfen Sie, ob das Feld &quot;Mit Mkto synchronisieren&quot;des Kontakts wahr ist. Ist dies der Fall, ändern Sie die Option &quot;Synchronisieren mit Mkto&quot;im Konto ebenfalls in &quot; **True** &quot;.
* Wenn das Feld Potenzieller Kunde (benutzerdefiniert) oder Kontakt (übergeordnet) aktualisiert wird, überprüfen Sie, ob das Feld Synchronisierung mit Mkto des Kontos wahr ist oder ob das Feld Synchronisierung mit Mkto des Kontakts wahr ist. Wenn dies der Fall ist, ändern Sie die Synchronisierung auf Mkto, um die Möglichkeit zu **True** ebenfalls

