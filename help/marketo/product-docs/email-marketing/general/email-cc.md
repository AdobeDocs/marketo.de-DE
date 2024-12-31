---
unique-page-id: 17727995
description: E-Mail-CC - Marketo-Dokumente - Produktdokumentation
title: E-Mail CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# E-Mail CC {#email-cc}

E-Mail-CC : Ermöglicht den Versand bestimmter E-Mails über Marketo, um CC-Empfänger einzuschließen.

Diese Funktion ist für alle Marketo-E-Mail-Assets verfügbar, unabhängig davon, wie die E-Mail gesendet wird (Batch- oder Trigger-Kampagne). Der CC-Empfänger erhält eine exakte Kopie der E-Mail, die an die ausgewählte Marketo-Person gesendet wurde. Jede Interaktionsaktivität (Öffnungen, Klicks usw.) wird daher im Aktivitätsprotokoll der Marketo-Person in der Zeile „An“ der E-Mail protokolliert. Eine Versandaktivität (gesendet, zugestellt, Hardbounce usw.) _anders als „Softbounce_ wird jedoch **nicht** registriert, da Marketo Versandereignisse für die Marketo-Person nicht von denen der CC-Empfänger unterscheiden kann. Marketo wird nur CC bis zu 100k Personen auf einmal. Wenn Ihre Smart-Liste 100.000 überschreitet und es zwingend erforderlich ist, dass jede Person auf ihr CC erhält, empfehlen wir, Ihre Liste aufzuschlüsseln.

>[!NOTE]
>
>E-Mail-CC wurde nicht für die Verwendung mit A/B-Tests entwickelt. Sie können es trotzdem verwenden, wenn Sie möchten. Da es jedoch technisch nicht unterstützt wird, kann der Marketo-Support Ihnen bei der Fehlerbehebung nicht helfen.

## Einrichten von E-Mail-CC {#set-up-email-cc}

1. Klicken Sie in My Marketo auf **Admin**.

   ![](assets/one.png)

1. Wählen Sie in der Struktur **E-Mail** aus.

   ![](assets/two.png)

1. Klicken Sie **E-Mail-CC-Einstellungen bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie bis zu 25 Marketo-Lead- oder Firmenfelder (vom Typ „E-Mail„) aus, um sie als CC-Adressen in E-Mails verfügbar zu machen. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/four.png)

## Verwenden von E-Mail-CC {#using-email-cc}

1. Wählen Sie Ihre E-Mail aus und klicken Sie **Entwurf bearbeiten**.

   ![](assets/five.png)

1. Klicken Sie auf **E-Mail-Einstellungen**.

   ![](assets/six.png)

1. Wählen Sie bis zu fünf Felder aus, in denen CC-Benutzer verwendet werden sollen. In diesem Beispiel möchten wir nur die Lead Owner-CC. Klicken Sie **Speichern** wenn Sie fertig sind.

   ![](assets/seven.png)

   So einfach ist das! Wenn Sie im obigen Beispiel die E-Mail senden, wird der Lead-Inhaber der ausgewählten Empfänger CC sein.

   >[!NOTE]
   >
   >Wenn sich in einem CC-Feld eine ungültige E-Mail-Adresse befindet, wird sie übersprungen.

   Zur schnellen Identifizierung zeigt die Ansicht E-Mail-Zusammenfassung an, ob/welche E-Mail-CC-Felder ausgewählt wurden.

   ![](assets/eight.png)

   Wenn die E-Mail genehmigt wurde, der Marketo-Administrator jedoch eines oder mehrere der CC-Felder deaktiviert hat, bevor die E-Mail gesendet **, erhalten diese Personen keine E-Mail**. In diesem Szenario werden in der Ansicht E-Mail-Zusammenfassung alle Felder ausgegraut, die nach der Genehmigung deaktiviert, aber vorab gesendet wurden:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Der obige Fehler wird auch im Abschnitt E-Mail-Einstellungen des E-Mail-Entwurfs angezeigt.

## Nach dem Senden {#after-the-send}

* Wenn ein CC-Empfänger auf einen verfolgten Link in der E-Mail klickt, wird die Klick-Aktivität (wie alle anderen Interaktionsaktivitäten) mit dem Hauptempfänger der E-Mail verknüpft. Darüber hinaus können sie sich durch Klicken auf eine Seite mit dem Webtrackingcode von Marketo (munchkin.js) öffnen, wodurch sie als Hauptempfänger codiert werden.

>[!TIP]
>
>Sie haben die Möglichkeit, [einige oder alle Tracking-Links zu deaktivieren](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) in einer E-Mail.

* Nachdem eine E-Mail-Kampagne ausgeführt wurde, enthält die Aktivität E-Mail senden eine Liste aller CC-Adressen, die für jeden Empfänger der E-Mail enthalten waren. Wenn CC-Adressen aufgrund einer Abmeldung übersprungen wurden, wird dies auch in der Aktivität vermerkt.
* Abmelde-Links und -Seiten funktionieren normalerweise in CC-E-Mails. Auf diese Weise können sich CC-Empfänger bei Bedarf erfolgreich abmelden (gemäß den Anti-Spam-Bestimmungen). Ein Datensatz dieser Aktion wird in der Marketo-Datenbank gespeichert.
* Personen, die in Ihrer Marketo-Datenbank als abgemeldet aufgeführt sind, erhalten **nicht** E-Mails über CC.
