---
unique-page-id: 10095307
description: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse {#custom-sync-filter-rules-for-an-email-address}

Um die Synchronisierung von Datensätzen ohne E-Mail-Adresse zu verhindern, befolgen Sie diese Regeln.

* Wenn ein Lead erstellt wird ODER wenn das E-Mail-Adressfeld des Leads aktualisiert wird, überprüfen Sie, ob der Lead über eine E-Mail-Adresse verfügt, und ändern Sie in Mkto synchronisieren zu . **True**. Andernfalls ändern Sie zu **False**

* Wenn ein Kontakt erstellt wird ODER wenn das E-Mail-Adressfeld des Kontakts aktualisiert wird, überprüfen Sie, ob der Kontakt über eine E-Mail-Adresse verfügt, und ändern Sie die Option In Mkto synchronisieren in **True** und ändern Sie &quot;Synchronisieren mit &quot;Mkto&quot; in **True** im Kontodatensatz. Andernfalls ändern Sie zu **False**

* Wenn das Feld Firmenname (parentCustomerID) des Kontakts aktualisiert wird, überprüfen Sie, ob das Feld Mit Mkto synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie im Konto die Option Auf Mkto synchronisieren in **True** auch
* Wenn das Feld Potenzieller Kunde (customerid) oder Kontakt (parentContactID) der Gelegenheit aktualisiert wird, überprüfen Sie, ob das Feld Mit Mkto synchronisieren des Kontos wahr ist oder ob das Feld Mit Mkto synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie die Option In Mkto synchronisieren , um **True** auch
