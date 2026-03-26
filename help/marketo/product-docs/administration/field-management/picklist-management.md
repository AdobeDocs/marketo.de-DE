---
description: Die Beschreibung ist hier zu finden.
title: Auswahllisten-Verwaltung
hide: true
hidefromtoc: true
feature: Field Management
source-git-commit: 3c9facaed46a72c12a8a604aa9d22b47e28183cb
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Auswahllisten-Verwaltung {#picklist-management}

Mit der Auswahllistenverwaltung können Sie einen festen Satz von Werten für ein Feld definieren, um die Daten- und Workflow-Verwaltung in Marketo Engage zu vereinfachen. Nur Nicht-Text-Felder, die keinem CRM-Feld mit einer definierten Auswahlliste zugeordnet sind, können in Marketo verwaltet werden. Wenn ein Feld einem CRM-Feld zugeordnet ist, das über eine definierte Auswahlliste verfügt, müssen die Werte für dieses Feld im CRM definiert werden.

Sie können den Status einer Auswahlliste auf der Seite „Feldverwaltung“ einsehen. Ein Feld kann einen der folgenden Auswahllistenstatus aufweisen:

* **Verwaltet**: Ein Benutzer hat den Satz von Werten definiert, die für dieses Feld automatisch vorgeschlagen werden können. Nur in der Feldverwaltung definierte Werte werden automatisch vorgeschlagen. Wenn eine verwaltete Auswahlliste gelöscht wird, wird der Auswahllistenstatus auf den ursprünglichen Wert für das Feld zurückgesetzt, entweder „Nicht verwaltet“ oder „Vordefiniert“.

* **Nicht verwaltet**: Die möglichen Werte für dieses Feld sind nicht definiert. Werte werden automatisch vorgeschlagen, basierend auf den Werten, die in den Feldern in der Datenbank vorhanden sind.

* **Seed**: Das Feld verfügt über eine systemdefinierte Liste von Werten, die den Benutzenden vorgeschlagen werden.

* **CRM**: Das Feld hat einen Wert, der vom CRM-System, Salesforce.com oder Microsoft Dynamics definiert wird, das mit der Instanz synchronisiert wird.

  ![](assets/picklist-management-1.png)

## Auswahlliste verwalten {#manage-picklist}

Um die Werte für ein Feld zu ändern, gehen Sie zu **Admin** > **Feldverwaltung** und wählen Sie das gewünschte Feld aus.

Klicken Sie auf die _Feldaktionen_ und wählen Sie **Auswahlliste verwalten** aus.

![](assets/picklist-management-2.png)

Im Dialogfeld _Auswahlliste verwalten_ können Sie Werte hinzufügen, bearbeiten oder löschen. Sie können die verwaltete Auswahlliste auch löschen, um den ursprünglichen Auswahllistenstatus des Felds wiederherzustellen, entweder _Nicht verwaltet_ oder _Seeding_.

![](assets/picklist-management-3.png)

Jeder Eintrag in der Auswahlliste hat einen Anzeigewert und einen gesendeten Wert. Der Anzeigewert wird dem Benutzer beim Erstellen von Smart Lists, Smart Kampagnen oder Formularen empfohlen, während der gesendete Wert derjenige ist, der gespeichert wird. Beispielsweise kann Ihr Anwendungsfall Gebiets-Code den vollständigen Namen eines Gebiets (z. B. Alberta) vorschlagen, während der aus zwei Buchstaben bestehende Code (AB) gespeichert wird.

## AutoSuggest {#autosuggest}

### Wechseln zwischen verwalteten und nicht verwalteten Auswahllisten {#switching}

Die meisten Marketo Engage-Abonnements enthalten Daten aus der Zeit vor der Einführung von verwalteten Auswahllisten. Um Werte in Smart-Listen oder Flussschritten aus dieser nicht verwalteten Versionsauswahlliste zu verwenden (z. B. aus dem vollständigen Satz von Werten, die in Datensätzen in Ihrer Datenbank vorhanden sind), schalten Sie die Einstellung Verwaltete Auswahlliste in Ihrer Smart-Listen- oder Kampagnenansicht um. Wenn diese Option aktiviert ist, werden nur die verwalteten Auswahllistenwerte angezeigt. Wenn diese Option deaktiviert ist, wird die nicht verwaltete Auswahlliste verwendet und Werte werden basierend auf vorhandenen Werten in der Datenbank automatisch vorgeschlagen.

### Formular-Auswahllisten (Felder vom Typ auswählen) {#form-picklists}

Wie bei Seed- und CRM-verwalteten Auswahllisten werden die Werte für verwaltete Auswahllisten bei Verwendung des Feldtyps Auswählen nach Forms übertragen. Wählen Sie für ein Feld mit einer verwalteten Auswahlliste dieses Feld aus und setzen Sie den Feldtyp auf _Auswählen_.

![](assets/picklist-management-4.png)

Zeigt den Satz von Werten der verwalteten Auswahlliste an, die für dieses Feld definiert sind.

![](assets/picklist-management-5.png)
