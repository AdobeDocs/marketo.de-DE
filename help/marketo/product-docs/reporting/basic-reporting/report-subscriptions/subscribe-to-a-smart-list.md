---
unique-page-id: 7505310
description: Smart List abonnieren - Marketo Docs - Produktdokumentation
title: Smart-Liste abonnieren
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# Smart-Liste abonnieren {#subscribe-to-a-smart-list}

Das Abonnieren von Smart-Listen ist eine hervorragende Möglichkeit, Personen zu verfolgen, wobei Berichte direkt an Ihren Posteingang gesendet werden.

Sie können ein Abonnement mit der intelligenten Liste an zwei verschiedenen Stellen erstellen:

* Marketingaktivitäten
* Datenbank

Abonnements verwenden die vollständige Liste der Personen zum Zeitpunkt der Abonnementausführung.

Abonnements wohnen an der Stelle, an der sich Ihre Smart-Liste befindet, in Marketingaktivitäten oder in der Datenbank.

Sie können mehrere Abonnements aus derselben Smart-Liste erstellen.

Abonnements sind Workspace-spezifisch. Beispielsweise befindet sich diese Abonnementliste in einem anderen Arbeitsbereich als im Rest dieses Artikels:

![](assets/one.png)

>[!NOTE]
>
>Sie sind auf 100 Abonnements und maximal 100.000 Personen pro Abonnement in allen Arbeitsbereichen und pro Marketo-Instanz beschränkt. Wenn die Smart-Liste mehr als 100.000 Namen enthält, führt Marketo das Abonnement für die ersten 100.000 aus.

## Abonnement mit intelligenter Liste erstellen {#create-a-smart-list-subscription}

1. Navigieren Sie zu **Datenbank** oder **Marketingaktivitäten**.

   ![](assets/db.png)

1. Wählen Sie die Smart-Liste aus, für die Sie ein Abonnement erstellen möchten. Klicken **Aktionen auflisten** und wählen Sie **Neues Abonnement der Smart-Liste**.

   ![](assets/three.png)

1. Geben Sie Ihrem Abonnement eine **Name** und wählen Sie dann die E-Mail-Adressen der **Empfänger**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Klicken Sie auf **Häufigkeit** und wählen Sie eine Häufigkeit aus.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Legen Sie die **Endversand** Datum. Sie können **Nie** oder ein Kalenderdatum.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Klicken **Format** und wählen Sie aus der Liste aus.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. Ihr neues Smart-List-Abonnement wird oben in der Liste auf der Registerkarte Abonnements angezeigt. Klicken **Senden** , wenn Sie jetzt senden möchten, und nicht bis zum geplanten E-Mail-Versand warten.

   ![](assets/eight.png)

1. Es wird empfohlen, das Kontrollkästchen Aktiv zu deaktivieren, um ein Abonnement mit der intelligenten Liste zu deaktivieren, wenn niemand ein Abonnement mit der intelligenten Liste hat.

   ![](assets/nine.png)

   Das war einfach, oder?

## E-Mail-Nachricht {#email-message}

Die Empfänger erhalten eine E-Mail mit einer Option zum Herunterladen des Berichts sowie einen Link direkt zur Liste innerhalb der Marketo-Instanz. Der Download-Link läuft in vier Tagen ab.

>[!NOTE]
>
>Wenn die Variable [Sicherer Abonnementadministrator](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) festgelegt ist auf **Ja**, können nur Benutzer mit Zugriff auf die Marketo-Instanz den Bericht herunterladen.

![](assets/image2015-4-17-15-3a46-3a47.png)

Wenn ein Bericht 0 Personen enthält, erhalten die Empfänger weiterhin eine E-Mail. In der E-Mail wird jedoch lediglich darauf hingewiesen, dass es keine Personen gibt, die gemeldet werden müssen.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Wenn Sie einen Smart-List-Filter ändern, auf dem ein Abonnement basiert, wird auch der Bericht aktualisiert.

Die E-Mail enthält außerdem zusätzliche Informationen zu den Filtern, die zum Erstellen der Liste verwendet werden.

## Abonnement löschen {#delete-a-subscription}

Um ein Abonnement zu löschen, wählen Sie es im Tab Abonnements aus und klicken Sie auf Abonnement löschen .

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Abonnement einer Smart-Liste bearbeiten](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Sichern der Abonnement-Admin-Einstellung](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
