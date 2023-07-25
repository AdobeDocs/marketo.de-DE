---
unique-page-id: 2950578
description: Social-Profildaten verwalten - Marketo-Dokumente - Produktdokumentation
title: Social-Profildaten verwalten
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 8%

---

# Social-Profildaten verwalten {#manage-social-profile-data}

Interaktion mit einer Marketo [Social App](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md), oder autorisiert ihr soziales Netzwerk, ein Marketo-Formular vorab auszufüllen mit [Soziales Formular ausfüllen](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), erfasst Marketo alle Daten, die über ihr Social-Profil verfügbar sind. Diese Informationen finden Sie im [Seite &quot;Personendetails&quot;](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)oder fügen Sie sie als Spalte in einer [benutzerdefinierte Ansicht einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

Social-Formulare und Social-Apps erfassen leicht unterschiedliche Feldsätze. sehen Sie den Abschnitt für jeden unten.

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Detaillierte Informationen erhalten Sie vom zuständigen Vertriebsmitarbeiter.

## Erfasst über Social App {#captured-via-social-app}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere dieser Felder abgerufen:

>[!NOTE]
>
>Die zusätzlichen Informationen aus sozialen Netzwerken werden auf der Seite &quot;Personendetails&quot;ca. fünf Minuten nach der Erlaubnis der Person angezeigt.

## In Twitter: {#from-twitter}

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
>Durch das Ausfüllen von sozialen Formularen erfasste Daten überschreiben übereinstimmende Felder, es sei denn, Sie [Blockaktualisierungen dieser Felder auf Formularebene](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## In Twitter: {#from-twitter-1}

* Vorname (basierend auf Anzeigename geparst)
* Nachname (basierend auf Anzeigename geparst)
* E-Mail

## Von Facebook: {#from-facebook-1}

* Vorname
* Nachname
* E-Mail
* Geburtsdatum
* Job-Titel
* Unternehmen

>[!NOTE]
>
>Durch das Ausfüllen eines Social-Formulars wird die E-Mail-Adresse erfasst _only_ wenn die Person sie in das Formular eingibt. Wenn Sie die E-Mail-Adresse benötigen, sollten Sie [Machen Sie es zu einem erforderlichen Feld in Ihrem Formular](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Um diese Informationen aus Formularen zu erfassen, aktivieren Sie [Soziales Formular ausfüllen](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
