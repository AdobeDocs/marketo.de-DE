---
description: Einrichten von reCAPTCHA v3 - Marketo Docs - Produktdokumentation
title: Einrichten von reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: ccc62b22f260293ac193ce03a31e4f03aba34768
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Einrichten von reCAPTCHA v3 {#setting-up-recaptcha-v3}

Intro Text

## Erstmaliges reCAPTCHA v3-Setup {#initial-recaptcha-v3-setup}

Text: Beschreiben Sie v3 : Die folgenden Schritte werden außerhalb von Marketo Engage ausgeführt.

1. Navigieren Sie zu [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} und klicken Sie auf die Admin Console v3.

1. Melden Sie sich mit einem Google-Konto an/melden Sie sich an.

1. Klicken Sie auf die Schaltfläche Erstellen (+-Zeichen) , um einen neuen Schlüssel zu erstellen.

1. Erstellen Sie einen Titel, der angibt, welcher Schlüssel zum Marketo Engage verwendet werden soll.

1. Typ auswählen **reCAPTCHA v3**. Marketo Engage unterstützt reCAPTCHA v2 derzeit nicht.

1. Fügen Sie alle Domänen hinzu, die das Marketo Engage-Abonnement verwendet. Domänen, die hier nicht festgelegt sind, geben Fehler in Formularen zurück, bei denen reCAPTCHA aktiviert ist.

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * jede Landingpage-Domäne und jeden im Abonnement konfigurierten Alias

1. Legen Sie einen Eigentümer und eine zusätzliche E-Mail-Adresse fest, die Warnhinweise zu diesem Dienst erhalten sollen.

1. Akzeptieren Sie die reCAPTCHA-Nutzungsbedingungen.

1. Klicken **Einsenden**.

>[!NOTE]
>
>Halten Sie den Site-Schlüssel und den geheimen Schlüssel für die Konfiguration von Marketo Engage bereit.

## CAPTCHA in Marketo Engage einrichten {#setting-up-captcha-in-marketo-engage}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Auswählen **CAPTCHA** im Baum.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Klicken **Bearbeiten** in den CAPTCHA-Einstellungen.

   ![](assets/setting-up-recaptcha-v3-3.png)

1. Klicken Sie auf die Dropdown-Liste CAPTCHA und wählen Sie reCAPTCHA v3 aus.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Geben Sie den geheimen Schlüssel und den Site-Schlüssel ein. Klicken **Speichern** wann geschehen.

   ![](assets/setting-up-recaptcha-v3-5.png)
