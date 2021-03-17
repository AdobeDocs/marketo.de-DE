---
unique-page-id: 37356194
description: Senden Sie eine Liste an Adobe Experience Cloud - Marketing Docs - Produktdokumentation
title: Liste an Adobe Experience Cloud senden
translation-type: tm+mt
source-git-commit: 96d6cc030ecd9d1da844fe27e1c6f62bbd181d62
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 0%

---


# Liste an Adobe Experience Cloud senden {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Eine HIPAA-bereite Bereitstellung einer Marketing-Instanz kann diese Funktion nicht verwenden.

>[!PREREQUISITES]
>
>[Einrichten der Freigabe von Adobe Experience Cloud-Audiencen](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Unterstützte Zielanwendungen {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (**nur**, wenn Sie eine Adobe Audience Manager-Lizenz besitzen)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Echtzeit-Kundendatenplattform
* Adobe Target

## Senden einer statischen Liste {#how-to-send-a-static-list}

Eine statische Liste ist genau das, statisch. Die Liste in Adobe Experience Cloud wird nur dann geändert, wenn Sie sie manuell vornehmen.

1. Suchen Sie in Marketo die Liste, die Sie exportieren möchten, und wählen Sie sie aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Klicken Sie auf die Dropdown-Liste **Liste Aktionen** und wählen Sie **An Experience Cloud senden**.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Klicken Sie auf die Dropdownliste **Audience Manager-Ordner** und wählen Sie den gewünschten Zielordner im Experience Cloud aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Wählen Sie, ob Sie eine neue Audience erstellen oder eine vorhandene überschreiben möchten (in diesem Beispiel erstellen wir eine neue). Geben Sie den Namen der neuen Audience ein und klicken Sie auf **Senden**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

1. Klicken Sie auf **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

   >[!NOTE]
   >
   >Es kann bis zu 6-8 Stunden dauern, bis die Audience in der Adobe voll gefüllt ist.

## So senden Sie eine synchronisierte Liste {#how-to-send-a-synced-list}

Das Synchronisieren einer Liste bedeutet, dass eine Liste in Marketo jedes Mal, wenn Sie sie aktualisieren, automatisch mit ihrer Audience in Adobe Experience Cloud synchronisiert wird.

1. Suchen Sie in Marketo die Liste, die Sie synchronisieren möchten, und wählen Sie sie aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Klicken Sie auf die Dropdown-Liste **Liste Aktionen** und wählen Sie **An Experience Cloud senden**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Klicken Sie auf die Dropdownliste **Audience-Bibliotheksordner** und wählen Sie den gewünschten Zielordner im Experience Cloud aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

1. Wählen Sie, ob Sie eine neue Audience erstellen oder eine vorhandene überschreiben möchten (in diesem Beispiel erstellen wir eine neue). Geben Sie den Namen der neuen Audience ein, aktivieren Sie das Kontrollkästchen **Mitgliedschaft in Audience beibehalten in Sync** und klicken Sie auf **Senden**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Klicken Sie auf **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

## Anhalten einer Liste-Synchronisierung {#how-to-stop-a-list-sync}

Sie können die Synchronisierung Ihrer Liste jederzeit unterbrechen.

1. Suchen Sie in Marketo die Liste, die Sie beenden möchten, und wählen Sie sie aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

1. Klicken Sie auf die Dropdown-Liste **Liste Aktionen** und wählen Sie **Liste-Synchronisierung beenden**.

   ![](assets/send-a-list-to-adobe-experience-cloud-12.png)

1. Wählen Sie die Audiencen aus, die nicht mehr synchronisiert werden sollen, und klicken Sie auf **Stopp**.

   ![](assets/send-a-list-to-adobe-experience-cloud-13.png)

1. Klicken Sie zur Bestätigung auf **Stopp**.

   ![](assets/send-a-list-to-adobe-experience-cloud-14.png)

## Dinge zu beachten {#things-to-note}

**Freigeben für Adobe Analytics**

Für Kunden, die sowohl Adobe Audience Manager als auch Adobe Analytics besitzen, ermöglicht diese Integration die Freigabe von Audiencen von Marketo an Ihre Adobe Analytics Report Suites, es gibt jedoch einige zusätzliche Konfigurationsschritte, die in Adobe Audience Manager durchgeführt werden müssen, um dies zu ermöglichen. Weitere Informationen zum Einrichten dieser Funktion finden Sie in der Adobe Audience Manager-Dokumentation: [https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Eigenschaftsverwendung für Adobe Audience Manager-Kunden**

Wenn Sie einen Export von Listen in Marketo starten, werden die folgenden Änderungen in Ihrer Adobe Audience Manager-Instanz angezeigt:

* Für alle Interessenten in der exportierten Liste schreibt Marketo eine Eigenschaft mit den Hash-E-Mails der Interessenten als geräteübergreifende ID. Der Name der Eigenschaft stimmt mit dem Namen der Ziel-Audience überein, den Sie während des Exports angegeben haben.
* Für alle ECIDs, die Marketo mit den Interessenten in der exportierten Liste abgleichen konnte, schreibt Marketo eine Eigenschaft mit der ECID-Gerätekennung. Der Name der Eigenschaft stimmt mit dem Namen der Ziel-Audience überein, den Sie während des Exports angegeben haben.
* Marketo erstellt auch ein Segment in Ihrer Audience Manager-Instanz mit dem ECID-Merkmal als einziges Segmentierungskriterium. Der Segmentname entspricht dem Segmentnamen, den Sie während des Exports angegeben haben.

## FAQ {#faq}

**Warum unterscheidet sich die Liste in Marketo von der in der Adobe?**

Unter der Haube funktioniert die Audience-Integration, indem Marketo Munchkin-Cookies mit dem entsprechenden ECID-Cookie der Adobe synchronisiert werden. Marketo kann nur Mitgliedsdaten für Interessenten freigeben, für die Marketo eine ECID synchronisiert hat. Um optimale Ergebnisse zu erzielen, wird empfohlen, das Verfolgungsskript &quot;munchkin.js&quot;von Marketo parallel zum Trackingcode &quot;Besucher.js&quot;der Adobe auf allen Seiten zu laden, die Sie zu Marketingzwecken verfolgen möchten.

**Wie funktioniert die Cookie-Synchronisierung?**

Wenn die Cookie-Synchronisierung für Ihr Marketo-Abonnement aktiviert ist, versucht die Datei &quot;munchkin.js&quot;von Marketo, ECIDs der Adobe für die Adobe IMS Org zu erfassen und zu speichern, die Sie während der Integrationseinstellung angegeben haben, und diese ECIDs mit der entsprechenden Marketo-Cookie-ID abzustimmen. Dadurch können die anonymen Profil von Marketo mit Adobe-ECIDs bereichert werden.

Ein weiterer Schritt ist erforderlich, um das anonyme Benutzerkonto mit einem Lead-Profil zu verknüpfen, das mit einer E-Mail-Adresse ohne Text identifiziert wird. Genau wie das funktioniert, wird hier [beschrieben.](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)

**Welche Informationen werden freigegeben?**

Diese Integration gibt nur Informationen zur Liste von Marketo an die Adobe weiter (z.B. das Wissen, dass Lead X Mitglied der Liste Y ist). Über diese Integration werden keine weiteren Interessentenattribute für die Adobe freigegeben.
