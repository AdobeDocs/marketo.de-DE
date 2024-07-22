---
description: Landingpage für konversalen Fluss verwenden - Marketo-Dokumente - Produktdokumentation
title: Landingpage für Konversionsfluss verwenden
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 1%

---

# Landingpage für Konversionsfluss verwenden{#use-a-conversational-flow-landing-page}

Durch das Einbetten eines Dynamic Chat-Konversationsflusses direkt in eine Marketo Engage-Landingpage können Besucher ein Treffen über Dynamic Chat planen, ohne ein Formular ausfüllen oder mit einem Chat-Bot interagieren zu müssen.

>[!PREREQUISITES]
>
>Erstellen Sie einen einfachen [Konversationsfluss](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md), der nur eine **Sitzungsbuchungskarte** enthält.

## Geführte Einstiegsseiten {#guided-landing-pages}

Betten Sie den folgenden Code in Ihre Vorlage für die geführte Einstiegsseite ein: `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Öffnen Sie die Vorlage für die geführte Einstiegsseite im Editor und wählen Sie den Platzhalter für den Konversationsfluss aus.

Klicken Sie auf die Dropdown-Liste Konversionsfluss und wählen Sie den Inhaltsordner aus, den Sie in Schritt 1 erstellt haben.

Behalten Sie den Bereitstellungstyp immer als **In-line** bei. Klicken Sie auf **Einfügen**.

Der soeben eingegebene Konversationsfluss erscheint als Element auf der rechten Seite.

SCREENSHOT

>[!NOTE]
>
>Zu diesem Zeitpunkt wird der Konversationsfluss nicht im Hauptvorschaufenster angezeigt.

## Freiform-Einstiegsseiten {#free-form-landing-pages}

Text


HINWEISE VON SCHRITTSMEETING

geführter lp, neue div id für Vorlage, Konvertierungsfluss wählen

Freeform lp, Übermittlungssymbol - Caveat: add note - Wenn Sie cf im Editor platzieren, wird Ihnen keine Vorschau angezeigt (auch kein Platzhalter) - &quot;Sie werden keine Vorschau sehen&quot;- in der Seitenleiste wird angezeigt, dass sich der cf auf der Seite befindet - &quot;Geführte Seite listet ihn als Element auf - verwenden Sie &quot;zu diesem Zeitpunkt&quot; bei der Erläuterung - Funktion wird möglicherweise in der 22. Woche live geschaltet

