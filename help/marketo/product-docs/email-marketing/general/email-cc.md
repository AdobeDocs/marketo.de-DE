---
unique-page-id: 17727995
description: Email CC - Marketo Docs - Produktdokumentation
title: Email CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Email CC {#email-cc}

E-Mail CC ermöglicht den Versand bestimmter E-Mails über Marketo, um CC-Empfänger einzubeziehen.

Diese Funktion ist für alle Marketo-E-Mail-Assets verfügbar, unabhängig davon, wie die E-Mail gesendet wird (Batch- oder Trigger-Kampagne). Der CC-Empfänger erhält eine exakte Kopie der E-Mail, die an die ausgewählte Marketo-Person gesendet wird. Interaktionsaktivitäten (Öffnungen, Klicks usw.) wird im Aktivitätsprotokoll der Marketo-Person in der Zeile &quot;An&quot;der E-Mail protokolliert. Versandaktivität (gesendet, zugestellt, Hardbounce usw.) _anders als &quot;Softbounce&quot;_ registriert sich **nicht**, da Marketo keine Versandereignisse für die Marketo-Person von den CC-Empfängern unterscheiden kann. Marketo kann nur bis zu 100.000 Personen gleichzeitig bedienen. Wenn Ihre intelligente Liste 100.000 übersteigt und es für jede Person wichtig ist, CC&#39;d zu erhalten, empfehlen wir, Ihre Liste aufzuschlüsseln.

>[!NOTE]
>
>E-Mail CC wurde nicht für die Verwendung mit A/B-Tests entwickelt. Sie können es trotzdem verwenden, wenn Sie möchten, aber da es technisch nicht unterstützt wird, kann der Marketo-Support bei der Fehlerbehebung nicht helfen.

## E-Mail einrichten CC {#set-up-email-cc}

1. Klicken Sie in My Marketo auf **Admin**.

   ![](assets/one.png)

1. Wählen Sie im Baum **E-Mail** aus.

   ![](assets/two.png)

1. Klicken Sie auf **E-Mail-CC-Einstellungen bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie bis zu 25 Marketo Lead- oder Firmenfelder (vom Typ &quot;E-Mail&quot;) aus, um diese als CC-Adressen in E-Mails verfügbar zu machen. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/four.png)

## Verwenden von Email CC {#using-email-cc}

1. Wählen Sie Ihre E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/five.png)

1. Klicken Sie auf **E-Mail-Einstellungen**.

   ![](assets/six.png)

1. Wählen Sie bis zu fünf Felder aus, die Sie für CC-Benutzer verwenden möchten. In diesem Beispiel möchten wir nur den Lead Owner CC&#39;d. Klicken Sie abschließend auf **Speichern** .

   ![](assets/seven.png)

   So einfach ist es! Im obigen Beispiel lautet der Lead-Inhaber der ausgewählten Empfänger beim Versand der E-Mail CC&#39;d.

   >[!NOTE]
   >
   >Wenn sich eine ungültige E-Mail-Adresse in einem CC-Feld befindet, wird sie übersprungen.

   Zur schnellen Identifizierung zeigt die Ansicht E-Mail-Zusammenfassung an, ob/welche E-Mail-CC-Felder ausgewählt wurden.

   ![](assets/eight.png)

   Wenn die E-Mail genehmigt wurde, der Marketo-Administrator jedoch eines oder mehrere CC-Felder deaktiviert, bevor die E-Mail gesendet wird, erhält **dieser Benutzer keine E-Mail**. In diesem Szenario werden in der Ansicht &quot;E-Mail-Zusammenfassung&quot;alle Felder grau dargestellt, die nach der Genehmigung deaktiviert, aber vorab gesendet wurden:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Der oben genannte Fehler wird auch im Abschnitt E-Mail-Einstellungen des E-Mail-Entwurfs angezeigt.

## Nach dem Senden {#after-the-send}

* Wenn ein CC-Empfänger auf einen verfolgten Link in der E-Mail klickt, wird die Klickaktivität (wie alle anderen Interaktionsaktivitäten) mit dem Hauptempfänger der E-Mail verknüpft. Darüber hinaus klicken sie möglicherweise zu einer Seite mit dem Web-Trackingcode von Marketo (munchkin.js), wodurch sie als Hauptempfänger gekocht werden.

>[!TIP]
>
>Sie haben die Option [, einige oder alle Tracking-Links](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) in einer E-Mail zu deaktivieren.

* Nach Ausführung einer E-Mail-Kampagne enthält die Aktivität E-Mail senden eine Liste aller CC-Adressen, die für jeden Empfänger des Mailings enthalten waren. Wenn CC-Adressen aufgrund einer Abmeldung übersprungen wurden, wird dies auch in der Aktivität vermerkt.
* Abmelde-Links und -Seiten funktionieren in CC&#39;d-E-Mails normal. Auf diese Weise können CC-Empfänger sich erfolgreich abmelden, wenn sie dies wünschen (Einhaltung der Anti-Spam-Vorschriften). Ein Datensatz mit dieser Aktion wird in der Marketo-Datenbank gespeichert.
* Personen, die in Ihrer Marketo-Datenbank als abgemeldet aufgeführt sind, erhalten **keine** E-Mails über CC.
