---
unique-page-id: 2359807
description: Preisausschreiben anpassen - Marketo Docs - Produktdokumentation
title: Gewinnspielstile anpassen
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Gewinnspielstile anpassen {#customize-sweepstakes-styles}

Wenn Sie [ein Gewinnspiel erstellen](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), können Sie anpassen, wie es auf Ihrer Landingpage aussieht.

>[!IMPORTANT]
>
>Am 31. Juli 2024 begannen wir mit der Einstellung dieser Funktion. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

1. Wechseln Sie zu **Marketingaktivitäten**.

![](assets/login-marketing-activities-1.png)

1. Wählen Sie die Gewinnspiele aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Wechseln Sie im Gewinnspiel-Editor zu **App-Einstellungen** > **Erscheinungsbild**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Bearbeiten Sie den Text der Anmelde-Schaltfläche und den Fortschrittslink.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Geben Sie für jedes Element, das Sie anpassen möchten, Ihre benutzerdefinierten CSS-Eigenschaften ein.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Beispiel-CSS für **Eingabeschaltfläche**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Beispielbild für **Eingabeschaltfläche**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Wenn Sie ein Bild mit Text darin verwenden, denken Sie daran, den Text aus dem Feld **Eingabetaste** unter Text oben zu entfernen.

1. Bei jeder Änderung wird das Ergebnis in der Vorschau &quot;Ansicht und Bearbeiten&quot;angezeigt.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testen Sie Ihre Schaltfläche in verschiedenen Browsern, einschließlich älterer Versionen.

   >[!MORELIKETHIS]
   >
   >Der nächste Schritt besteht darin, Ihrem Gewinnspiel ](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md) [Anmelde- und Erfüllungs-E-Mails hinzuzufügen.
