---
description: Einrichten von reCAPTCHA v3 - Marketo Docs - Produktdokumentation
title: Einrichten von reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Einrichten von reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3 ist ein reibungsloses Erlebnis, bei dem Formularübermittlungen basierend darauf bewertet werden, wie misstrauisch sie sind, ohne Text-, Bild- oder Schaltflächen-Herausforderungen zu verwenden. [Weitere Infos](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Abrufen Ihres Rechenzentrums und Ihrer Munchkin-ID {#retrieve-your-data-center-and-munchkin-id}

Für Schritt 6 im unten stehenden Abschnitt zur Einrichtung von reCAPTCHA v3 benötigen Sie das Data Center und die Munchkin-ID Ihres Marketo Engage-Abonnements. Hier ist, wie man sie findet.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Klicken Sie auf **Mein Konto**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Scrollen Sie nach unten zu Support-Informationen.

   ![](assets/setting-up-recaptcha-v3-3.png)

## Erstmaliges reCAPTCHA v3-Setup {#initial-recaptcha-v3-setup}

Die folgenden Schritte werden außerhalb von Marketo ausgeführt.

1. Wechseln Sie zu [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} und klicken Sie auf die Admin Console v3.

1. Melden Sie sich mit einem Google-Konto an/melden Sie sich an.

1. Klicken Sie auf die Schaltfläche Erstellen (+-Zeichen), um einen neuen Schlüssel zu erstellen.

1. Erstellen Sie einen Titel, der angibt, welcher Schlüssel für das Marketo Engage verwendet werden soll.

1. Wählen Sie den Typ **reCAPTCHA v3** aus. Marketo Engage unterstützt reCAPTCHA v2 derzeit nicht.

1. Fügen Sie jede Domäne hinzu, die das Marketo Engage-Abonnement verwendet. Domänen, die hier nicht festgelegt sind, geben Fehler in Formularen zurück, bei denen reCAPTCHA aktiviert ist. Denken Sie daran, die Wörter &quot;datacenter&quot;und &quot;munchkinID&quot;durch die [Daten in Ihrem Abonnement](#retrieve-your-data-center-and-munchkin-id) zu ersetzen.

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * jede Landingpage-Domäne und jeden im Abonnement konfigurierten Alias

   >[!NOTE]
   >
   >Wenn das Rechenzentrum Ihres Kontos beispielsweise &quot;sjst&quot;lautet, lautet die von Ihnen auf die Zulassungsliste gesetzt Domäne `app-sjst.marketo.com`. Wenn Ihre Munchkin-ID 123-ABC-789 lautet, lautet die Domäne, für die Sie Zulassungsliste haben, `123-ABC-789.mktoweb.com`.

1. Legen Sie einen Eigentümer und eine zusätzliche E-Mail-Adresse fest, die Warnhinweise zu diesem Dienst erhalten sollen.

1. Akzeptieren Sie die reCAPTCHA-Nutzungsbedingungen.

1. Klicken Sie auf **Senden**.

   >[!NOTE]
   >
   >Halten Sie den Site-Schlüssel und den geheimen Schlüssel für die Marketo Engage-Konfiguration bereit.

## CAPTCHA in Marketo Engage einrichten {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>Nachdem Sie diese Schritte ausgeführt haben und [CAPTCHA in Ihrem ersten Marketo-Formular aktivieren](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}, sollten Sie das Formular sofort testen, da jede Art von Fehlkonfiguration in der reCAPTCHA-Einrichtung das Formular beschädigen kann.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Wählen Sie **CAPTCHA** im Baum aus.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Klicken Sie in den CAPTCHA-Einstellungen auf **Bearbeiten** .

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Klicken Sie auf die Dropdown-Liste CAPTCHA und wählen Sie reCAPTCHA v3 aus.

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Geben Sie den geheimen Schlüssel und den Site-Schlüssel ein. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[CAPTCHA in Marketo Forms aktivieren](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
