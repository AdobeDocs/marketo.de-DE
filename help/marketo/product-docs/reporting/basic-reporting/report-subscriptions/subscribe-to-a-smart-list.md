---
unique-page-id: 7505310
description: Abonnieren einer Smart-Liste - Marketo-Dokumente - Produktdokumentation
title: Abonnieren einer Smart-Liste
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---

# Abonnieren einer Smart-Liste {#subscribe-to-a-smart-list}

Das Abonnieren von Smart Lists ist eine hervorragende Möglichkeit, den Überblick über Personen zu behalten, wobei Berichte direkt an Ihren Posteingang gesendet werden.

Sie können ein Smart-Listen-Abonnement an zwei separaten Stellen erstellen:

* Marketingaktivitäten
* Datenbank

Abonnements verwenden die vollständige Liste der Personen zum Zeitpunkt der Abonnementausführung.

Abonnements sind dort verfügbar, wo Ihre Smart-Liste lebt, ob in Marketing-Aktivitäten oder in der Datenbank.

Sie können mehrere Abonnements über dieselbe Smart-Liste erstellen.

Abonnements sind bereichsspezifisch. Beispielsweise befindet sich diese Liste von Abonnements in einem anderen Arbeitsbereich als der, der im Rest dieses Artikels angezeigt wird:

![](assets/one.png)

>[!NOTE]
>
>Pro Marketo-Instanz sind auf 100 Abonnements und maximal 100.000 Personen pro Abonnement in allen Arbeitsbereichen beschränkt. Wenn die Smart-Liste mehr als 100.000 Namen enthält, führt Marketo das Abonnement für die ersten 100.000 aus.

## Erstellen eines Smart-Listen-Abonnements {#create-a-smart-list-subscription}

1. Navigieren Sie zu **Datenbank** oder **Marketing-Aktivitäten**.

   ![](assets/db.png)

1. Wählen Sie die Smart-Liste aus, für die Sie ein Abonnement erstellen möchten. Klicken Sie auf **Aktionen auflisten** und wählen Sie **Neues Smart-Listen-Abonnement** aus.

   ![](assets/three.png)

1. Geben Sie Ihrem Abonnement **Name** und wählen oder geben Sie dann die E-Mail-Adressen der **Empfänger** ein.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Klicken Sie auf **Häufigkeit** und wählen Sie eine Häufigkeit aus.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Legen Sie das **Ende des Versands** fest. Sie können **Nie** oder ein Kalenderdatum auswählen.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Klicken Sie **Format** und wählen Sie aus der Liste aus.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. Ihr neues Smart-Listen-Abonnement wird oben in der Liste auf der Registerkarte Abonnements angezeigt. Klicken Sie **Senden**, wenn Sie jetzt senden möchten, und nicht auf den geplanten E-Mail-Versand warten möchten.

   ![](assets/eight.png)

1. Es wird empfohlen, das Kontrollkästchen Aktiv zu deaktivieren, um Smart-Listen-Abonnements zu deaktivieren, die von niemandem abonniert wurden.

   ![](assets/nine.png)

   Das war einfach, nicht wahr?

## E-Mail-Nachricht {#email-message}

Die Empfänger erhalten eine E-Mail mit der Option, den Bericht herunterzuladen, sowie einen Link direkt zur Liste innerhalb der Marketo-Instanz. Der Downloadlink läuft in vier Tagen ab.

>[!NOTE]
>
>Wenn die Einstellung [Sichere Abonnementverwaltung](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) auf **Ja** festgelegt ist, können nur Personen mit Zugriff auf die Marketo-Instanz den Bericht herunterladen.

![](assets/image2015-4-17-15-3a46-3a47.png)

Wenn ein Bericht 0 Personen enthält, erhalten Empfänger weiterhin eine E-Mail. Die E-Mail besagt jedoch lediglich, dass keine Personen zum Anzeigen vorhanden sind.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Wenn Sie einen Smart-Listen-Filter ändern, auf dem Sie ein Abonnement erstellt haben, wird auch der Bericht aktualisiert.

Die E-Mail enthält auch zusätzliche Informationen zu den Filtern, die zum Erstellen der Liste verwendet wurden.

## Löschen eines Abonnements {#delete-a-subscription}

Um ein Abonnement zu löschen, wählen Sie es auf der Registerkarte Abonnements aus und klicken Sie auf Abonnement löschen .

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Bearbeiten eines Smart-Listen-Abonnements](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Sichern der Abonnement-Admin-Einstellung](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
