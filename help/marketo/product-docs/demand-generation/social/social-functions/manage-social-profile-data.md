---
unique-page-id: 2950578
description: Social-Profildaten verwalten - Marketo-Dokumente - Produktdokumentation
title: Social-Profildaten verwalten
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 5%

---

# Social-Profildaten verwalten {#manage-social-profile-data}

Wenn ein Benutzer mit einer Marketo [Social-App](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) interagiert oder sein soziales Netzwerk autorisiert, ein Marketo-Formular mit [Ausfüllen eines Social-Formulars](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md) im Voraus auszufüllen, erfasst Marketo alle Daten, die über sein Social-Profil verfügbar sind. Sie können diese Informationen auf der Seite [Personendetails](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) anzeigen oder sie als Spalte in einer [benutzerdefinierten Ansicht einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md) hinzufügen.

>[!IMPORTANT]
>
>Am 31. Juli 2024 begannen wir mit der Einstellung dieser Funktion. Sie können keine neuen Assets erstellen. Vorhandene Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Das Ausfüllen von Social-Formularen und Social-Apps erfassen geringfügig unterschiedliche Feldsätze. Weitere Informationen finden Sie im folgenden Abschnitt.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

## Erfasst über Social App {#captured-via-social-app}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere dieser Felder abgerufen:

>[!NOTE]
>
>Die zusätzlichen Informationen aus sozialen Netzwerken werden auf der Seite &quot;Personendetails&quot;ca. fünf Minuten nach der Erlaubnis der Person angezeigt.

## Von Twitter: {#from-twitter}

* Vorname (basierend auf Anzeigename geparst)
* Nachname (basierend auf Anzeigename geparst)
* Profilfoto-URL
* Profilseiten-URL
* Soziale Reichweite (Anzahl der Follower)

>[!NOTE]
>
>Social-Apps rufen die E-Mail-Adresse der Person nicht ab.

## In Facebook: {#from-facebook}

* Vorname
* Nachname
* Profil-URL
* Profilfoto-URL
* Geschlecht
* Soziale Reichweite (Anzahl Freunde)

### Erfasst über Social-Formular {#captured-via-social-form-fill}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere dieser Felder abgerufen:

>[!CAUTION]
>
>Durch das Ausfüllen von sozialen Formularen erfasste Daten überschreiben übereinstimmende Felder, es sei denn, Sie [blockieren Aktualisierungen dieser Felder auf Formularebene](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Von Twitter: {#from-twitter-1}

* Vorname (basierend auf Anzeigename geparst)
* Nachname (basierend auf Anzeigename geparst)
* E-Mail

## In Facebook: {#from-facebook-1}

* Vorname
* Nachname
* E-Mail
* Geburtsdatum
* Jobtitel
* Unternehmen

>[!NOTE]
>
>Durch das Ausfüllen eines Social-Formulars wird die E-Mail-Adresse _nur_ erfasst, wenn die Person sie in das Formular eingibt. Wenn Sie die E-Mail-Adresse benötigen, sollten Sie sie [in Ihrem Formular als erforderliches Feld festlegen](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Um diese Informationen aus Formularen zu erfassen, aktivieren Sie [Ausfüllen von Social-Formularen](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
