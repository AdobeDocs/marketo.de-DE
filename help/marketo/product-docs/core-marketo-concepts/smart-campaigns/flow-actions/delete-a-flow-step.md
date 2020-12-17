---
unique-page-id: 1146987
description: Löschen eines Flussschritts - Marketing-Dokumente - Produktdokumentation
title: Flussschritt löschen
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Löschen eines Flussschritts {#delete-a-flow-step}

>[!CAUTION]
>
>Das Entfernen von Flussschritten, *vor allem Warteschritte* aus aktiven intelligenten Kampagnen kann zu unerwarteten Ergebnissen führen. **Lesen Sie diesen Artikel aufmerksam durch.**

Zuerst machen wir die Grundlagen. So entfernen Sie einen unerwünschten Flussschritt aus einer intelligenten Kampagne. 1. Klicken Sie im Fluss für intelligente Kampagnen auf das X-Symbol, um jeden Flussschritt zu löschen.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Klicken Sie auf **Löschen**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Einfach und einfach, nicht wahr? Nun, meistens...

   >[!CAUTION]
   >
   >Das Löschen, Hinzufügen und Verschieben von Schritten innerhalb einer **active**-Kampagne kann definitiv zu unerwarteten Ergebnissen führen. Erwägen Sie, eine neue Kampagne zu erstellen, sie zu testen und dann zu wechseln.

   An einer aktiven Kampagne können Änderungen vorgenommen werden, die jedoch unvorhergesehene Folgen haben können. Im Folgenden finden Sie die Details:

   **Stapelverarbeitung intelligenter Kampagnen**

   Wenn Ihre Kampagne:

   1. **Es ist nie gerannt.** Nehmen Sie alle gewünschten Änderungen vor. Das betrifft niemanden, solange du die Kampagne nicht durchführt.
   1. **Ist eine wiederkehrende intelligente Kampagne.** Die Änderungen betreffen die Benutzer in den zukünftigen Versionen, nicht in vorherigen Versionen.
   1. **Bereits ausgeführt, OHNE Schritte zu warten.** Es werden keine Menschen betroffen sein, weil die Kampagne nach dem Laufen ruhmt.
   1. **Läuft gerade.** Änderungen können je nach Zeitpunkt und Details des Löschvorgangs zu unerwartetem Verhalten führen. Es wird dringend empfohlen, KEINE Batch-Kampagne zu bearbeiten, die aktiv ausgeführt wird. Erfahren Sie, wie Sie eine laufende intelligente Kampagne [abbrechen können.](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)

   1. **Mit Warteschritten bereits ausgeführt.** Einige Details dazu.\
      Wenn eine Person einen Warteschritt aufruft, teilt die Person die Dauer mit und zu welcher NUMBER-SCHRIFT sie zurückkehren soll. Siehe Beispiel unten.

   **Auslösen intelligenter Kampagnen**

   1. **Keine Warteschritte.** Wenn Sie einen normalen Schritt löschen, werden nur Personen betroffen sein, die zukünftig die Kampagne durchlaufen.
   1. **Bei Warteschritten.** Siehe Beispiel unten für Batch-Kampagnen. Dieselbe Logik gilt.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >    
   >    
   >1. Eine intelligente Kampagne besteht aus drei Schritten.
   >
   >   * SCHRITT 1. Email Nr. 1 senden
   >   * SCHRITT 2. Warten Sie 1 Woche
   >   * SCHRITT 3. Email Nr. 2 senden
   >
   >1. Personen, die auf **Schritt 2** klicken, warten eine Woche, bevor sie zu **Schritt 3** fortfahren.
   >1. Sie löschen **Schritt 2** während der Woche.
   >1. Die Leute werden weiterhin die Woche warten. (Sie tauchen nicht automatisch in den Fluss zurück.)
   >1. Wenn sie schließlich zurückkehren, versuchen sie, zu **Schritt 3** zu wechseln. Sie werden es nicht finden.
   >1. **WICHTIG:** Da es jetzt nur 2 Schritte gibt, erhalten die  *Personen keine E-Mail Nr. 2.*


Vornehmen von Änderungen an einer aktiven Kampagne

Verstehen Sie diese Funktion und Sie werden intelligente Kampagnen Übergeordnet. Oh!
