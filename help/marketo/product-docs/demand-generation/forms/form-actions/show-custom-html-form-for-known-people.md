---
unique-page-id: 2359644
description: Benutzerdefiniertes HTML-Formular für bekannte Personen anzeigen - Marketo Docs - Produktdokumentation
title: Benutzerdefiniertes HTML-Formular für bekannte Personen anzeigen
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Benutzerdefiniertes HTML-Formular für bekannte Personen anzeigen {#show-custom-html-form-for-known-people}

Wenn ein Besucher Cookies hat (eine bekannte Person, die in der Vergangenheit eine E-Mail-Adresse bereitgestellt hat), warum sollte er sich dann mit dem Formular beschäftigen? Geben Sie ihnen einfach die Download-Schaltfläche. So geht es.

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities-5.png)

1. Wählen Sie unter **Marketingaktivitäten** Ihr Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Klicken Sie unter &quot;**Formulareinstellungen**&quot;auf &quot;**Einstellungen**&quot;.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Wenn **bekannter Besucher, Show**: auf **Benutzerspezifische HTML** gesetzt ist.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Klicken Sie auf ![—](assets/image2014-9-25-14-3a1-3a26.png) , um die **benutzerdefinierte HTML** zu bearbeiten, die bekannten Personen angezeigt wird.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Es gibt einige Standardinhalte, aber Sie können sie gerne ändern.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Verfügbare Token:

   | Token | Beschreibung |
   |---|---|
   | `{{lead.FirstName}}` | Dadurch wird der Vorname der Person angezeigt. |
   | `{{lead.LastName}}` | Dadurch wird der Nachname der Person angezeigt. |
   | `{{form.Button:default=Download}}` | Dadurch wird die Formularschaltfläche angezeigt. Ersetzen Sie den Bereich nach dem `=` , um den Schaltflächentext zu ändern. |
   | `{{form.NotYou:default=Not you?}}` | Dadurch wird ein Link angezeigt, falls die Person jemand anderes ist. Ersetzen Sie den Bereich nach dem `=` , um den Link-Text zu ändern. |

   >[!CAUTION]
   >
   >Es können nur die vier oben genannten Token verwendet werden. Hier funktioniert kein anderes Token.

1. Klicken Sie auf **Beenden**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Klicken Sie auf **Genehmigen und schließen**.

   >[!NOTE]
   >
   >Das Formular muss validiert sein, damit es auf Landingpages verwendet werden kann.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Denken Sie daran, den durch die Formularänderungen erstellten Landingpage-Entwurf ](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) zu genehmigen.[

   Kuchen! Überprüfen Sie, was eine Person sehen würde, wenn sie zum selben Formular zurückkehrt:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Sie können den Klick auf die Schaltfläche zum Asset leiten, indem Sie die Formular-Folgenachricht auf die URL der Datei setzen.
