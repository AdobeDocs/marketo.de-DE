---
unique-page-id: 17727995
description: E-Mail CC - Marketing-Dokumente - Produktdokumentation
title: Email CC
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---


# Email CC {#email-cc}

E-Mail CC ermöglicht den Versand spezifizierter E-Mails über Marketo mit CC-Empfängern.

Diese Funktion ist für alle Marketing-E-Mail-Assets verfügbar, unabhängig davon, wie die E-Mail gesendet wird (Batch- oder Trigger-Kampagne). Der CC-Empfänger erhält eine genaue Kopie der E-Mail, die an den ausgewählten Marker gesendet wird. Als solche werden alle Interaktionsaktionen (Aktivitäten werden geöffnet, Klicks usw.) wird in der Zeile &quot;An&quot;der E-Mail beim Aktivitäten-Protokoll des &quot;Marketo-Benutzers&quot;protokolliert. Versand-Aktivität (gesendet, ausgeliefert, Absprung usw.) *andere als &quot;Soft Bounce&quot;* werden  **** nicht registriert, da Marketo nicht in der Lage ist, die Ereignis des Versands für den Marketo-Benutzer von den CC-Empfängern zu unterscheiden. Marketo wird nur CC bis zu 100.000 Personen auf einmal. Wenn Ihre intelligente Liste 100k übersteigt und es für jeden erforderlich ist, CC&#39;d zu erhalten, empfehlen wir, Ihre Liste aufzubrechen.

>[!NOTE]
>
>Email CC wurde nicht für die Verwendung mit A/B-Tests entwickelt. Sie können es trotzdem verwenden, wenn Sie möchten, aber da es technisch nicht unterstützt wird, könnte der Support von Marketo bei der Fehlerbehebung nicht helfen.

## Einrichten von E-Mail CC {#set-up-email-cc}

1. Klicken Sie in &quot;My Marketo&quot;auf **Admin**.

   ![](assets/one.png)

1. Wählen Sie in der Struktur **E-Mail**.

   ![](assets/two.png)

1. Klicken Sie auf **E-Mail-CC-Einstellungen bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie bis zu 25 Marketing Lead- oder Firma-Felder (vom Typ &quot;E-Mail&quot;) aus, um sie als CC-Adressen in E-Mails zur Verfügung zu stellen. Klicken Sie abschließend auf **Speichern**.

   ![](assets/four.png)

## Verwenden von Email CC {#using-email-cc}

1. Wählen Sie Ihre E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/five.png)

1. Klicken Sie auf **E-Mail-Einstellungen**.

   ![](assets/six.png)

1. Wählen Sie bis zu fünf Felder aus, die Sie für CC-Benutzer verwenden möchten. In diesem Beispiel wollen wir nur den Interessentenbesitzer CC&#39;d. Klicken Sie abschließend auf **Speichern**.

   ![](assets/seven.png)

   So einfach ist es! Im obigen Beispiel ist der Lead-Inhaber der ausgewählten Empfänger beim Senden der E-Mail CC&#39;d.

   >[!NOTE]
   >
   >
   >Wenn sich eine ungültige E-Mail-Adresse in einem CC-Feld befindet, wird sie übersprungen.

   Zur schnellen Identifizierung zeigt die Ansicht &quot;E-Mail-Zusammenfassung&quot;an, ob/welche E-Mail-CC-Felder ausgewählt wurden.  ![](assets/eight.png)

   Wenn die E-Mail genehmigt wurde, der Marketing-Administrator jedoch eines oder mehrere CC-Felder deaktiviert, bevor die E-Mail gesendet wird, **erhalten diese Personen keine E-Mail**. In diesem Fall werden in der Ansicht &quot;E-Mail-Zusammenfassung&quot;alle Felder ausgegraut, die nach der Genehmigung deaktiviert, aber vorab gesendet wurden:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Sie sehen den obigen Fehler auch im Abschnitt &quot;E-Mail-Einstellungen&quot;des E-Mail-Entwurfs.

## Nach dem Senden {#after-the-send}

* Wenn ein CC-Empfänger auf einen verfolgten Link in der E-Mail klickt, wird die Aktivität (wie alle anderen Interaktions-Aktivitäten) mit dem Haupt-Empfänger der E-Mail verknüpft. Darüber hinaus können sie durch einen Klick auf eine Seite mit Marketo&#39;s Web-Trackingcode (munchkin.js) gelangen, wodurch sie als Haupt-Empfänger gekocht werden.

>[!TIP]
>
>Sie haben die Möglichkeit, [einige oder alle Verfolgungslinks](http://docs.marketo.com/x/IwAd) in einer E-Mail zu deaktivieren.

* Nachdem eine E-Mail-Kampagne ausgeführt wurde, enthält die Aktivität &quot;E-Mail senden&quot;eine Liste aller CC-Adressen, die für jeden Empfänger des Mailings enthalten waren. Wenn CC-Adressen aufgrund des Abmeldung übersprungen wurden, wird dies auch in der Aktivität vermerkt.
* Abmelden von Links und Seiten funktionieren normalerweise in CC-E-Mails. Dies ermöglicht es CC-Empfängern, sich erfolgreich abzumelden, wenn sie es wünschen (Einhaltung der Anti-Spam-Vorschriften), und ein Datensatz dieser Aktion wird in der Marketo-Datenbank gespeichert.
* Personen, die in Ihrer Marketo-Datenbank als nicht abonniert aufgeführt sind, erhalten E-Mails über CC.****

