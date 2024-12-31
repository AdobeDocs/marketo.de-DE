---
unique-page-id: 2950578
description: Verwalten von Profildaten aus sozialen Netzwerken - Marketo-Dokumente - Produktdokumentation
title: Verwalten von Profildaten aus sozialen Netzwerken
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Verwalten von Profildaten aus sozialen Netzwerken {#manage-social-profile-data}

Wenn jemand mit einer Marketo [Social-App](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) interagiert oder sein soziales Netzwerk autorisiert, ein Marketo-Formular mit [Social-Formular ausfüllen](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md) vorauszufüllen, erfasst Marketo alle verfügbaren Daten aus seinem sozialen Profil. Sie können diese Informationen auf der Seite [Personendetails](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) anzeigen oder als Spalte in einer [benutzerdefinierten Ansicht einer Smart-Liste“ ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Ausfüllen von Social-Media-Formularen und Social-Media-Apps erfassen geringfügig unterschiedliche Mengen von Feldern; siehe den Abschnitt für jede dieser Apps unten.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

## Über die Social App erfasst {#captured-via-social-app}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere dieser Felder abgerufen:

>[!NOTE]
>
>Die zusätzlichen Informationen aus den sozialen Netzwerken werden auf der Seite „Personendetails“ etwa fünf Minuten nach der Autorisierung durch die Person angezeigt.

## Von Twitter: {#from-twitter}

* Vorname (aus Anzeigename ausgewertet)
* Nachname (aus Anzeigename ausgewertet)
* URL des Profilbilds
* URL der Profilseite
* Soziale Reichweite (Anzahl der Follower)

>[!NOTE]
>
>Soziale Apps rufen die E-Mail-Adresse der Person nicht ab.

## Aus Facebook: {#from-facebook}

* Vorname
* Nachname
* Profil-URL
* URL des Profilbilds
* Geschlecht
* Soziale Reichweite (Anzahl Freunde)

### Über das Ausfüllen eines Social-Media-Formulars erfasst {#captured-via-social-form-fill}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere dieser Felder abgerufen:

>[!CAUTION]
>
>Daten, die von Social Media-Formularausfüllungen erfasst werden, überschreiben übereinstimmende Felder, es sei denn, [ blockieren Aktualisierungen dieser Felder auf Formularebene](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Von Twitter: {#from-twitter-1}

* Vorname (aus Anzeigename ausgewertet)
* Nachname (aus Anzeigename ausgewertet)
* E-Mail

## Aus Facebook: {#from-facebook-1}

* Vorname
* Nachname
* E-Mail
* Geburtsdatum
* Jobtitel
* Unternehmen

>[!NOTE]
>
>Ausfüllen eines Social-Media-Formulars erfasst die E _Mail-Adresse (nur_ wenn die Person sie im Formular eingibt. Wenn Sie die E-Mail-Adresse benötigen[ sollten Sie sie zu einem Pflichtfeld in Ihrem Formular ](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Um diese Informationen aus Formularen zu erfassen, aktivieren Sie [Social-Formular ausfüllen](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
