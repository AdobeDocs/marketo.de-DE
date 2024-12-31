---
unique-page-id: 2359807
description: Anpassen von Gewinner-Stilen - Marketo-Dokumente - Produktdokumentation
title: Anpassen von Verlosungsstilen
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Anpassen von Verlosungsstilen {#customize-sweepstakes-styles}

Wenn Sie [ein Gewinnspiel erstellen](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md) können Sie anpassen, wie es auf Ihrer Landingpage aussieht.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

1. Navigieren Sie **Marketing-Aktivitäten**.

![](assets/login-marketing-activities-1.png)

1. Wählen Sie das Gewinnspiel aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Navigieren Sie im Sweepstakes-Editor zu **App-Einstellungen** > **Erscheinungsbild**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Bearbeiten Sie den Text Ihrer Anmelde-Schaltfläche und den Fortschritts-Link.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Geben Sie für jedes Element, das Sie anpassen möchten, Ihre benutzerdefinierten CSS-Eigenschaften ein.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Beispiel-CSS für **Eingabetaste**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Beispielbild für **Eingabetaste**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Wenn Sie ein Bild mit Text verwenden, denken Sie daran, den Text aus dem Feld **Eingabetaste** unter Text oben zu entfernen.

1. Bei jeder Änderung wird das Ergebnis in der Vorschau anzeigen und bearbeiten angezeigt.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testen Sie die Schaltfläche in verschiedenen Browsern, einschließlich älterer Versionen.

   >[!MORELIKETHIS]
   >
   >Der nächste Schritt besteht darin, [Anmelde- und Erfüllungs-E-Mails zu Ihren Gewinnspielen hinzuzufügen](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
