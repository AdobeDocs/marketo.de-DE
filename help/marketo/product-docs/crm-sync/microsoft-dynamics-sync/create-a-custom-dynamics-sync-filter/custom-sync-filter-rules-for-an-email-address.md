---
unique-page-id: 10095307
description: Benutzerdefinierte Synchronisierungsfilterregeln für eine E-Mail-Adresse - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Regeln zum Synchronisieren von Filtern für E-Mail-Adressen
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Benutzerdefinierte Regeln zum Synchronisieren von Filtern für E-Mail-Adressen {#custom-sync-filter-rules-for-an-email-address}

Um das Synchronisieren von Datensätzen ohne E-Mail-Adresse zu verhindern, befolgen Sie die folgenden Regeln.

* Wenn ein Lead erstellt ODER das Feld „E-Mail-Adresse“ des Leads aktualisiert wird, überprüfen Sie, ob der Lead eine E-Mail-Adresse hat. Falls ja, ändern Sie „Synchronisieren mit Mkto“ in **[!UICONTROL True]**. Andernfalls ändern Sie in **[!UICONTROL False]**

* Wenn ein Kontakt erstellt ODER das Feld für die E-Mail-Adresse des Kontakts aktualisiert wurde, überprüfen Sie, ob der Kontakt eine E-Mail-Adresse hat. Falls ja, ändern Sie im Kontodatensatz die Einstellung Synchronisieren auf Mkto auf **[!UICONTROL True]** und die Einstellung Synchronisieren auf **[!UICONTROL True]**. Ändern Sie andernfalls in **[!UICONTROL False]**

* Wenn das Feld „Firmenname (parentCustomerID)“ des Kontakts aktualisiert wird, überprüfen Sie, ob das Feld „Mit MKTO synchronisieren“ für den Kontakt wahr ist. Ist dies der Fall, ändern Sie auch auf dem Konto die Einstellung Synchronisieren mit Mkto **[!UICONTROL True]**.
* Wenn das Feld Potenzielle Kunden-ID (customerID) oder Kontakt (parentContactID) der Opportunity aktualisiert wird, überprüfen Sie, ob das Feld Mit MKTO synchronisieren des Kontos wahr ist oder ob das Feld Mit MKTO synchronisieren des Kontakts wahr ist. Ist dies der Fall, ändern Sie bei der Möglichkeit, ebenfalls auf &quot;**[!UICONTROL &quot; zu]**, die Option Synchronisieren auf Mkto.
