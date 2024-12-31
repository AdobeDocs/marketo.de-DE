---
unique-page-id: 2359644
description: Benutzerdefiniertes HTML-Formular für Bekannte Personen anzeigen - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefiniertes HTML-Formular für Bekannte Personen anzeigen
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 1%

---

# Benutzerdefiniertes HTML-Formular für Bekannte Personen anzeigen {#show-custom-html-form-for-known-people}

Wenn ein Besucher Cookies erhält (bekannte Person, die in der Vergangenheit eine E-Mail-Adresse angegeben hat), warum sollte man sich dann mit dem Formular beschäftigen? Gib ihnen einfach die Download-Schaltfläche. So geht&#39;s.

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-5.png)

1. Wählen **unter „Marketing** Aktivitäten Ihr Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Klicken **unter &quot;**&quot; auf **Einstellungen**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Wenn **Bekannter Besucher, Anzeigen**: auf **Benutzerdefiniertes HTML** setzen

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Klicken Sie auf die ![-](assets/image2014-9-25-14-3a1-3a26.png), um die **Benutzerdefinierte HTML** zu bearbeiten, die bekannten Personen angezeigt wird.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Es gibt einige Standardinhalte, aber Sie können sie jederzeit ändern.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Verfügbare Token:

   | Token | Beschreibung |
   |---|---|
   | `{{lead.FirstName}}` | Dadurch wird der Vorname der Person angezeigt. |
   | `{{lead.LastName}}` | Dadurch wird der Nachname der Person angezeigt. |
   | `{{form.Button:default=Download}}` | Dadurch wird die Formularschaltfläche angezeigt. Ersetzen Sie den Bereich nach dem `=`, um den Schaltflächentext zu ändern. |
   | `{{form.NotYou:default=Not you?}}` | Dadurch wird ein Link angezeigt, falls die Person eine andere Person ist. Ersetzen Sie den Bereich nach dem `=`, um den Link-Text zu ändern. |

   >[!CAUTION]
   >
   >Nur die vier oben genannten Token können verwendet werden. Andere Token funktionieren hier nicht.

1. Klicken Sie auf **Fertigstellen**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Klicken Sie **Genehmigen und schließen**.

   >[!NOTE]
   >
   >Das Formular muss für die Verwendung auf Landingpages genehmigt sein.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Denken Sie daran[ den Landingpage-Entwurf zu genehmigen](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) der durch die Formularänderungen erstellt wurde.

   Ein Stück Kuchen! Sehen Sie nach, was eine Person sehen würde, wenn sie zum selben Formular zurückkehren würde:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Sie können den Klick auf die Schaltfläche zum Asset leiten, indem Sie die Formular-Folgeseite auf die URL der Datei festlegen.
