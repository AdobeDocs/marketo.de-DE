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

* Wenn ein Lead erstellt wird ODER wenn das E-Mail-Adressfeld des Leads aktualisiert wird, überprüfen Sie, ob der Lead über eine E-Mail-Adresse verfügt, und ändern Sie die Option &quot;Synchronisieren mit Mkto&quot;zu **[!UICONTROL True]**. Ändern Sie andernfalls &quot;**[!UICONTROL False]**&quot;.

* Wenn ein Kontakt erstellt wird ODER wenn das E-Mail-Adressfeld des Kontakts aktualisiert wird, überprüfen Sie, ob der Kontakt über eine E-Mail-Adresse verfügt. Wenn dies der Fall ist, ändern Sie &quot;Synchronisieren auf MKTO&quot; in &quot;**[!UICONTROL True]**&quot; und ändern Sie im Kontodatensatz die Option &quot;Mit MKTO synchronisieren&quot;in &quot;**[!UICONTROL True]**&quot;. Ändern Sie andernfalls &quot;**[!UICONTROL False]**&quot;.

* Wenn das Feld Firmenname (parentCustomerID) des Kontakts aktualisiert wird, überprüfen Sie, ob das Feld Mit Mkto synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie im Konto die Option Auf Mkto synchronisieren ebenfalls in **[!UICONTROL True]** .

* Wenn das Feld Potenzieller Kunde (customerid) oder Kontakt (parentContactID) der Gelegenheit aktualisiert wird, überprüfen Sie, ob das Feld Mit MKTO synchronisieren des Kontos wahr ist oder ob das Feld Mit MKTO synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie die Option &quot;Auf Mkto synchronisieren&quot;bei der Möglichkeit ebenfalls zu **[!UICONTROL True]** .
