---
unique-page-id: 1146987
description: Flussschritt löschen - Marketo-Dokumente - Produktdokumentation
title: Flussschritt löschen
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Flussschritt löschen {#delete-a-flow-step}

>[!CAUTION]
>
>Entfernen von Flussschritten, _insbesondere Warteschritte_ von aktiven Smart-Kampagnen können zu unerwarteten Ergebnissen führen. **Lesen Sie diesen Artikel aufmerksam durch.**

Machen wir zunächst die Grundlagen. So können Sie einen unerwünschten Flussschritt aus einer intelligenten Kampagne entfernen. 1. Klicken Sie im Fluss der intelligenten Kampagne auf das X-Symbol, um jeden Flussschritt zu löschen.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Klicken **Löschen**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Einfach und einfach, nicht wahr? Die meiste Zeit...

   >[!CAUTION]
   >
   >Löschen, Hinzufügen und Verschieben von Schritten innerhalb eines **active** Kampagne kann auf jeden Fall unerwartete Ergebnisse haben. Ziehen Sie die Erstellung einer neuen Kampagne in Erwägung, testen Sie sie und wechseln Sie dann.

   Änderungen können an einer aktiven Kampagne vorgenommen werden, können aber unvorhergesehene Folgen haben. Im Folgenden finden Sie die Details:

   **Smart-Kampagnen stapeln**

   Wenn Ihre Kampagne:

   1. **Nie rannte.** Nehmen Sie alle gewünschten Änderungen vor. Bis zum Ausführen dieser Kampagne wirkt sich dies auf niemanden aus.
   1. **ist eine wiederkehrende Smart-Kampagne.** Die Änderungen wirken sich auf die Benutzer in zukünftigen Ausführungen aus, nicht auf vorherige Ausführungen.
   1. **Bereits ausgeführt, OHNE die Schritte abzuwarten.** Es sind keine Personen betroffen, da die Kampagne nach dem Ausführen ruhend ist.
   1. **Läuft gerade.** Änderungen können abhängig vom Zeitpunkt und den Details des Löschvorgangs zu unerwartetem Verhalten führen. Es wird dringend empfohlen, KEINE Batch-Kampagne zu bearbeiten, die aktiv ausgeführt wird. Erfahren Sie, wie Sie bei Notfällen [Abbrechen einer laufenden Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Bereits MIT Warteschritten ausgeführt.** Einige Details dazu.\
      Wenn eine Person in einen Warteschritt eintritt, teilt die Person die Dauer mit und zu welchem NUMBER-SCHRITT sie zurückkehren soll. Siehe Beispiel unten.

   **Smart-Kampagnen für Trigger**

   1. **Keine Warteschritte.** Wenn Sie einen normalen Schritt löschen, sind nur Personen betroffen, die die Kampagne in der Zukunft durchlaufen.
   1. **Mit Warteschritten.** Siehe Beispiel unten für Batch-Kampagnen. Dieselbe Logik gilt.

   >[!NOTE]
   >
   >**Beispiel**
   >
   >1. Eine intelligente Kampagne besteht aus drei Schritten.
   >    * SCHRITT 1. E-Mail Nr. 1 senden
   >    * SCHRITT 2. Warten 1 Woche
   >    * SCHRITT 3. E-Mail Nr. 2 senden
   >
   >1. Personen, die **Schritt 2** wird 1 Woche warten, bevor Sie fortfahren **Schritt 3**.
   >1. Sie löschen **Schritt 2** in der Woche.
   >1. Die Leute werden weiterhin die 1 Woche warten. (Sie springen nicht automatisch in den Fluss zurück.)
   >1. Wenn sie schließlich zurückkehren, werden sie versuchen, **Schritt 3**. Sie werden es nicht finden.
   >1. **WICHTIG:** Da es jetzt nur 2 Schritte gibt, wird die *Personen erhalten keine E-Mail Nr. 2.*

Durchführen von Änderungen an einer aktiven Kampagne

Machen Sie sich mit dieser Funktion vertraut, und Sie werden Smart-Kampagnen Übergeordnet.
