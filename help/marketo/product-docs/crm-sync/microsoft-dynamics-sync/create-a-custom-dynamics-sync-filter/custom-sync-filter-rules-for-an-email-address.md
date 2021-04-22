---
unique-page-id: 10095307
description: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse - Marketo Dokumente - Produktdokumentation
title: Benutzerdefinierte Sync-Filterregeln für eine E-Mail-Adresse
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse {#custom-sync-filter-rules-for-an-email-address}

Um die Synchronisierung von Datensätzen ohne E-Mail-Adresse zu verhindern, befolgen Sie diese Regeln.

* Wenn ein Interessent erstellt wird ODER wenn das Feld für die E-Mail-Adresse des Interessenten aktualisiert wird, prüfen Sie, ob der Interessent eine E-Mail-Adresse hat. Ändern Sie andernfalls &quot;Synchronisieren&quot;zu &quot;Mkto&quot;in **True**. Andernfalls ändern Sie zu **False**

* Wenn ein Kontakt erstellt wird ODER wenn das Feld für die E-Mail-Adresse des Kontakts aktualisiert wird, prüfen Sie, ob der Kontakt eine E-Mail-Adresse hat. Wenn dies der Fall ist, ändern Sie &quot;Synchronisieren&quot;zu &quot;Mkto&quot;in **True** und ändern Sie im Kontodatensatz die Option &quot;Synchronisieren zu Mkto&quot;in **True**. Andernfalls wechseln Sie zu **False**

* Wenn das Feld &quot;Firma des Kontakts&quot;(parentcustomerid) aktualisiert wird, prüfen Sie, ob das Feld &quot;Mit Mkto synchronisieren&quot;des Kontakts wahr ist. Ist dies der Fall, ändern Sie für das Konto die Option Auf Mkto synchronisieren in **True** ebenfalls
* Wenn das Feld Potenzieller Kunde (benutzerdefiniert) oder Kontakt (übergeordnet) aktualisiert wird, überprüfen Sie, ob das Feld Synchronisierung mit Mkto des Kontos wahr ist oder ob das Feld Synchronisierung mit Mkto des Kontakts wahr ist. Ist dies der Fall, ändern Sie &quot;Synchronisieren&quot;zu &quot;Mkto&quot;, um **True** ebenfalls aufzurufen.
