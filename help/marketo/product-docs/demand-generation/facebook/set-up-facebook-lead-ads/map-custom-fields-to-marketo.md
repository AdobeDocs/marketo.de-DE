---
unique-page-id: 12983101
description: Benutzerdefinierte Felder Marketo zuordnen - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Felder Marketo zuordnen
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Benutzerdefinierte Felder Marketo zuordnen {#map-custom-fields-to-marketo}

Möglicherweise möchten Sie mehr als die standardmäßigen Informationen erfassen, die Facebook speichert, z. B. wie oft jemand Ihren Online-Versanddienst verwendet. Sie können dies erreichen, indem Sie [benutzerdefinierte Fragen erstellen](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) in Ihren Facebook-Lead-Anzeigen.

**Marketo beginnt jedoch nicht automatisch mit der Datenerfassung**. Damit Marketo mit der Erfassung benutzerdefinierter Feldwerte beginnt, müssen Sie diese benutzerdefinierten Felder **** einem Feld in Marketo zuordnen.

Hier erfahren Sie, wie Sie dies im Admin-Bereich von LaunchPoint einrichten.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Wechseln Sie zum Admin-Bereich und klicken Sie auf **LaunchPoint**. Suchen und bearbeiten Sie unter &quot;Installierte Dienste&quot;die Option **Facebook Lead Ads**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Belassen Sie das autorisierte Konto wie besehen - nehmen Sie **nicht** Änderungen vor. Klicken Sie auf **Weiter**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Lassen Sie wie zuvor die ausgewählten Seiten unverändert - nehmen Sie **keine** Änderungen vor. Klicken Sie auf **Weiter**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Hier ordnen Sie das benutzerdefinierte Facebook-Feld Ihrem Marketo-Feld zu. Klicken Sie auf **Hinzufügen.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Geben Sie in der neuen Zeile den Namen Ihres benutzerdefinierten Facebook-Felds ein.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Hier werden nur die in Facebook-Formularvorlagen gespeicherten Felder als Optionen angezeigt.

1. Klicken Sie in die Spalte **Marketo-Feld** . Geben Sie ein, um nach dem Feld zu suchen, dem Sie zuordnen möchten. Nachdem Sie ein Feld ausgewählt haben, klicken Sie auf **Speichern**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Wenn Sie noch kein Feld in Marketo haben, dem das Facebook-Feld zugeordnet werden soll, erfahren Sie, wie Sie [benutzerdefinierte Felder erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Sie **müssen** diesen Vorgang für jedes neue Facebook-Feld durchlaufen, damit Marketo die Daten erfassen kann.
