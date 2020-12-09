---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Feldsynchronisierung
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Feldsynchronisierung {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Marketo to to Dynamics sync ist super leistungsfähig. Hier sind die Details.

## Wie werden die Felddetails zwischen den beiden Systemen synchronisiert? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional für Interessenten- und Kontaktstellen. Wenn Sie Änderungen an einem Lead oder Kontakt in Dynamics oder einer Person in Marketo vornehmen, werden Ihre Updates in beiden Systemen übernommen.

Für Konto-, Benutzer-, Gelegenheit-, Team- und benutzerdefinierte Entitäten erfolgt die Synchronisierung nur in einer Richtung: Dynamik zu Marketo. Wenn Sie Änderungen an diesen Entitäten in Dynamics vornehmen, werden Ihre Updates in Marketo übernommen.

## Was ist, wenn in beiden Systemen gleichzeitig Änderungen am gleichen Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo gewinnen für Menschen (Interessenten) und Dynamics für Kontakte gewinnen. Das liegt daran, dass wir die Marketingabteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Verkaufsabteilung (CRM) besteht. Bei einseitigen Synchronisierungsentitäten gewinnt Dynamics immer.

## Kann ich mit Marketo ein Feld in Dynamics erstellen? {#can-i-create-a-field-in-dynamics-using-marketo}

Nein, dies wird derzeit nicht unterstützt.

## Ich schuf ein Feld in Dynamics. Kann ich es mit Marketo synchronisieren? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, Sie können das Feld [](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) synchronisieren, solange Ihr Synchronisierungsbenutzer Zugriff darauf in Dynamics hat.

Welche Felder werden mit Marketo synchronisiert?

Sie können Felder [auswählen, die während der Einrichtung synchronisiert](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) werden sollen.

## Was ist, wenn ich nach der Synchronisierung von Marketo und Dynamics ein benutzerdefiniertes Feld hinzufügen muss? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Sie können jederzeit Felder hinzufügen und erwarten, dass die Daten von Dynamics zu Marketo aktualisiert werden. Weitere Informationen finden Sie unter Schnellsynchronisierung mit Microsoft Dynamics [verwenden für ein neues benutzerdefiniertes Feld](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) .

>[!MORELIKETHIS]
>
>* [Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld verwenden](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



