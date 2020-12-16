---
unique-page-id: 2359644
description: Benutzerdefiniertes HTML-Formular für bekannte Personen anzeigen - Marketing Docs - Produktdokumentation
title: Benutzerdefiniertes HTML-Formular für bekannte Personen anzeigen
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Benutzerdefiniertes HTML-Formular für bekannte Personen anzeigen {#show-custom-html-form-for-known-people}

Wenn ein Besucher in Cookies gespeichert ist (eine bekannte Person, die in der Vergangenheit eine E-Mail-Adresse angegeben hat), warum sollte sich das Formular dann mit dem Formular beschäftigen? Geben Sie ihnen einfach die Download-Schaltfläche. So geht es.

1. Gehen Sie zu **Marketing** - **Aktivitäten**.

   ![](assets/login-marketing-activities-5.png)

1. Wählen Sie unter **Marketing** - **Aktivitäten** Ihr Formular aus und klicken Sie auf **Bearbeiten** des **Formulars**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Klicken Sie unter **Formulareinstellungen** auf **Einstellungen****Einstellungen**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Bei **bekanntem** **Besucher einstellen: Anzeigen**: auf **Benutzerdefiniertes** **HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Klicken Sie auf ![—](assets/image2014-9-25-14-3a1-3a26.png) , um den **benutzerspezifischen** **HTML** -Code zu bearbeiten, der Bekannten angezeigt wird.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Es gibt einige Standardinhalte, aber Sie können sie gerne ändern.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Verfügbare Token:

   | Token | Beschreibung |
   |---|---|
   | `{{lead.FirstName}}` | Dadurch wird der Vorname der Person angezeigt. |
   | `{{lead.LastName}}` | Dadurch wird der Nachname der Person angezeigt. |
   | `{{form.Button:default=Download}}` | Dadurch wird die Formularschaltfläche angezeigt. Ersetzen Sie den Bereich nach der Schaltfläche, `=` um den Schaltflächentext zu ändern. |
   | `{{form.NotYou:default=Not you?}}` | Dies zeigt einen Link an, falls die Person eine andere Person ist. Ersetzen Sie den Bereich nach dem `=` zum Ändern des Linktextes. |

   >[!CAUTION]
   >
   >Es können nur die vier oben genannten Token verwendet werden. Ein anderes Token funktioniert hier nicht.

1. Klicken Sie auf **Fertig stellen**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Klicken Sie auf **Genehmigen und Schließen**.

   >[!NOTE]
   >
   >Das Formular muss für die Verwendung auf Landingpages genehmigt werden.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Denken Sie daran, den mit den Formularänderungen erstellten Entwurf [der Landingpage zu](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) genehmigen.

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Sie können den Klick auf die Schaltfläche zum Asset lenken, indem Sie die Formular-Folgeseite auf die URL der Datei einstellen.

Kuchen! Überprüfen Sie, was eine Person sehen würde, wenn sie dasselbe Formular erneut aufruft: