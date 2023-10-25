---
unique-page-id: 10095307
description: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse {#custom-sync-filter-rules-for-an-email-address}

Um die Synchronisierung von Datensätzen ohne E-Mail-Adresse zu verhindern, befolgen Sie diese Regeln.

* Wenn ein Lead erstellt wird ODER wenn das E-Mail-Adressfeld des Leads aktualisiert wird, überprüfen Sie, ob der Lead über eine E-Mail-Adresse verfügt, und ändern Sie die Option In Mkto synchronisieren in **[!UICONTROL True]**. Andernfalls ändern Sie zu **[!UICONTROL False]**.

* Wenn ein Kontakt erstellt wird ODER wenn das E-Mail-Adressfeld des Kontakts aktualisiert wird, überprüfen Sie, ob der Kontakt über eine E-Mail-Adresse verfügt, und ändern Sie die Option In Mkto synchronisieren in **[!UICONTROL True]** und ändern Sie &quot;Synchronisieren mit &quot;Mkto&quot; in **[!UICONTROL True]** im Kontodatensatz. Andernfalls ändern Sie zu **[!UICONTROL False]**.

* Wenn das Feld Firmenname (parentCustomerID) des Kontakts aktualisiert wird, überprüfen Sie, ob das Feld Mit Mkto synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie im Konto die Option Auf Mkto synchronisieren in **[!UICONTROL True]** auch.

* Wenn das Feld Potenzieller Kunde (customerid) oder Kontakt (parentContactID) der Gelegenheit aktualisiert wird, überprüfen Sie, ob das Feld Mit MKTO synchronisieren des Kontos wahr ist oder ob das Feld Mit MKTO synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie die Option In Mkto synchronisieren , um **[!UICONTROL True]** auch.
