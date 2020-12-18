---
unique-page-id: 2950578
description: Social-Profil-Daten verwalten - Marketing-Dokumente - Produktdokumentation
title: Social-Profil-Daten verwalten
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Social-Profil-Daten verwalten {#manage-social-profile-data}

Wenn jemand mit einer Marketing [Social-App](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) interagiert oder ihr soziales Netzwerk autorisiert, ein Marketing-Formular mit [Social-Formularausfüllung](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md) im Voraus auszufüllen, erfasst Marketo alle Daten, die in ihrem Social-Profil verfügbar sind. Sie können diese Informationen auf der Seite [Personendetails](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page) oder als Spalte in einer [benutzerdefinierten Ansicht einer intelligenten Liste](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List) Ansicht hinzufügen.

In Social-Formularen und Social-Apps werden leicht unterschiedliche Feldsätze erfasst. siehe den Abschnitt für die einzelnen unten.

>[!NOTE]
>
>**Verfügbarkeit**
>
>Nicht alle Kunden haben diese Funktion erworben. Weitere Informationen erhalten Sie von Ihrem Vertriebsmitarbeiter.

## Erfasst über Social App {#captured-via-social-app}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere der folgenden Felder abgerufen:

>[!NOTE]
>
>Die zusätzlichen Informationen aus sozialen Netzwerken werden auf der Seite &quot;Personendetails&quot;etwa fünf Minuten nach der Erlaubnis der Person angezeigt.

## Von Twitter: {#from-twitter}

* Vorname (analysiert aus Anzeigename)
* Nachname (analysiert aus Anzeigename)
* Profil Foto-URL
* URL der Profil-Seite
* Soziale Reichweite (Follower-Anzahl)

>[!NOTE]
>
>Social-Apps rufen die E-Mail-Adresse der Person nicht ab.

## Von Facebook: {#from-facebook}

* Vorname
* Nachname
* Profil-URL
* Profil Foto-URL
* Geschlecht
* Soziale Reichweite (Anzahl der Freunde)

### Erfasst über Social-Formularausfüllung {#captured-via-social-form-fill}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere der folgenden Felder abgerufen:

>[!CAUTION]
>
>Durch das Ausfüllen sozialer Formulare erfasste Daten überschreiben übereinstimmende Felder, es sei denn, Sie [blockieren Aktualisierungen dieser Felder auf Formularebene](../../../../product-docs/administration/field-management/block-updates-to-a-field.md).

## Von Twitter: {#from-twitter-1}

* Vorname (analysiert aus Anzeigename)
* Nachname (analysiert aus Anzeigename)
* Email

## Von Facebook: {#from-facebook-1}

* Vorname
* Nachname
* Email
* Geburtsdatum
* Auftragstitel
* Firma

>[!NOTE]
>
>Beim Ausfüllen eines sozialen Formulars wird die E-Mail-Adresse *nur dann erfasst, wenn die Person sie in das Formular eingibt.* Wenn Sie die E-Mail-Adresse benötigen, sollten Sie [sie zu einem erforderlichen Feld in Ihrem Formular](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md) machen.

>[!MORELIKETHIS]
>
>Um diese Informationen aus Formularen zu erfassen, aktivieren Sie die Option [Ausfüllen sozialer Formulare](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).

>[!NOTE]
>
>**Tieftauchen**
>
>Weitere Informationen zum Arbeiten mit Formularen finden Sie im Tieftauchgang [Forms](http://docs.marketo.com/display/docs/forms).

