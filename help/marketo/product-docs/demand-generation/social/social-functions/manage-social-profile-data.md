---
unique-page-id: 2950578
description: Social-Profil-Daten verwalten - Marketing-Dokumente - Produktdokumentation
title: Social-Profil-Daten verwalten
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# Social-Profil-Daten verwalten {#manage-social-profile-data}

Wenn jemand mit einer Marketing- [Social-App](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)interagiert oder ihr soziales Netzwerk autorisiert, ein Marketo-Formular mit [Social-Formularen auszufüllen](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), erfasst Marketo alle Daten, die in ihrem Social-Profil verfügbar sind. Sie können diese Informationen auf der Seite [&quot;](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)Personendetails&quot;oder als Spalte in eine [benutzerdefinierte Ansicht einer intelligenten Liste](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)einfügen.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

In Social-Formularen und Social-Apps werden leicht unterschiedliche Feldsätze erfasst. siehe den Abschnitt für die einzelnen unten.

>[!NOTE]
>
>**Verfügbarkeit**
>
>Nicht alle Kunden haben diese Funktion erworben. Weitere Informationen erhalten Sie von Ihrem Vertriebsmitarbeiter.

## Über Social-App erfasst {#captured-via-social-app}

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

### Über Social-Formularausfüllung erfasst {#captured-via-social-form-fill}

Je nach den Datenschutzeinstellungen des Netzwerks und des Benutzers werden eines oder mehrere der folgenden Felder abgerufen:

>[!CAUTION]
>
>Durch das Ausfüllen sozialer Formulare erfasste Daten überschreiben übereinstimmende Felder, es sei denn, Sie [blockieren Updates auf Formularebene](../../../../product-docs/administration/field-management/block-updates-to-a-field.md).

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
>Das Ausfüllen von Social-Formularen erfasst die E-Mail-Adresse *nur* , wenn die Person sie in das Formular eingibt. Wenn Sie die E-Mail-Adresse benötigen, [sollten Sie sie in Ihr Formular](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)aufnehmen.

>[!MORELIKETHIS]
>
>Um diese Informationen aus Formularen zu erfassen, aktivieren Sie das Ausfüllen [sozialer Formulare](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).

>[!NOTE]
>
>**Tieftauchen**
>
>Erfahren Sie mehr über das Arbeiten mit Formularen im [Forms](http://docs.marketo.com/display/docs/forms) Deep Dive.

