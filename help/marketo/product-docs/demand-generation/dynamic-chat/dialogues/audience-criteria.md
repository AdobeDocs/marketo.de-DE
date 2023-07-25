---
description: Zielgruppenkriterien - Marketo-Dokumente - Produktdokumentation
title: Zielgruppenkriterien
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 2%

---

# Zielgruppenkriterien {#audience-criteria}

Ähnlich wie bei Smart-Lists in Marketo ermöglichen Ihnen Zielgruppenkriterien-Attribute die Definition Ihrer Zielgruppe. Sie können bekannte oder unbekannte Personen mithilfe von Inferred, Person oder Unternehmensattributen (oder einer Kombination daraus) ansprechen.

## Priorität {#priority}

Die Priorität bestimmt, welches Dialogfeld ein Lead erhält, falls er für mehr als ein Feld qualifiziert ist. Sie wird zum ersten Mal festgelegt [Dialogfeld erstellen](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}. Sie können die Priorität eines vorhandenen Dialogfelds ändern, indem Sie es öffnen und **Dialogfelddetails** auf der Registerkarte Zielgruppenkriterien .

![](assets/audience-criteria-1.png)

## Ereignisse {#events}

![](assets/audience-criteria-2.png)

Mit Ereignissen können Sie Besucher auf Basis des Bildlaufs oder der Dauer des Bildlaufs auf Ihrer Seite/Site als Ziel auswählen. Im folgenden Beispiel werden Besucher angesprochen, die sich seit mehr als 20 Sekunden auf einer bestimmten Seite befinden.

1. Grab die **Besuchszeit pro Seite** -Ereignis ein und ziehen Sie es nach rechts.

   ![](assets/audience-criteria-3.png)

1. Legen Sie die Zeit &quot;Größer als&quot;auf 20 Sekunden fest.

   ![](assets/audience-criteria-4.png)

1. Fügen Sie die URL der gewünschten Seite im [Target](#target) Abschnitt.

   ![](assets/audience-criteria-5.png)

## Attribute {#attributes}

![](assets/audience-criteria-6.png)

**Bekannte Personen**

Es gibt _many_ Attributkombinationen zur Auswahl. Im folgenden Beispiel werden alle **bekannte Personen** in Kalifornien, die in einem Unternehmen mit mehr als 50 Beschäftigten arbeiten.

1. Grab die **Bundesland** -Attribut fest und ziehen Sie es nach rechts.

   ![](assets/audience-criteria-7.png)

1. _Is_ ist standardmäßig festgelegt. Geben Sie im Feld Werte auswählen eine Zertifizierungsstelle ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/audience-criteria-8.png)

1. Grab die **Firmengröße** Attribut hinzufügen und an die gewünschte Position ziehen _Attribut hier ziehen und ablegen_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >Sie können auch ein Attribut auswählen, indem Sie auf dessen **+** Symbol.

1. Klicken Sie auf die Dropdown-Liste Operator und wählen Sie **Größer als**.

   ![](assets/audience-criteria-10.png)

1. Geben Sie 50 ein und klicken Sie auf eine andere Stelle auf dem Bildschirm, um zu speichern.

   ![](assets/audience-criteria-11.png)

Und das ist es!

**Anonyme Personen**

Es gibt eine einfache Möglichkeit, Personen gezielt anzusprechen, die noch nicht in Ihrer Datenbank sind. In diesem Beispiel zielen wir auf alle **Anonyme Personen** befindet sich im Gebiet von New York.

1. Grab die **Personen-E-Mail** -Attribut fest und ziehen Sie es nach rechts.

   ![](assets/audience-criteria-12.png)

1. Klicken Sie auf die Dropdown-Liste Operator und wählen Sie **Ist leer**.

   ![](assets/audience-criteria-13.png)

1. Grab die **Inferated State** Attribut hinzufügen und an die gewünschte Position ziehen _Attribut hier ziehen und ablegen_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Wenn jemand Ihre Website besucht, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) Cookies und setzt sie in das System. Wir suchen ihre IP-Adresse in einer speziellen Datenbank und schließen alle möglichen guten Informationen.

1. _Is_ ist standardmäßig festgelegt. Geben Sie im Feld Werte auswählen NY ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/audience-criteria-15.png)

## Gruppen hinzufügen {#add-groups}

Sie haben auch die Möglichkeit, Attribute zu gruppieren, falls Sie alle Attribute zusammen mit &quot;all&quot;oder &quot;any&quot;eines anderen Attributs haben möchten. Sie können mehrere Gruppen hinzufügen.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Zielgruppe {#target}

Hier geben Sie die URL(s) ein, für die ein bestimmtes Dialogfeld angezeigt werden soll. Sie haben auch die Möglichkeit, Ausschlüsse hinzuzufügen.

Zulässige Formate:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>Die Verwendung eines Sternchens dient als Platzhalter. Also `https://*.website.com` würde das Dialogfeld auf jeder Seite der Site platzieren, einschließlich Subdomains (z. B.: `support.website.com`). und `https://website.com/folder/*` würde das Dialogfeld auf jeder HTML-Seite im folgenden Ordner platzieren (z. B.: Nehmen wir in diesem Fall an, der Ordner ist &quot;Sport&quot;, also: website.com/sports/baseball.html, website.com/sports/football.html usw.).

**Ausschlüsse**

Verwenden Sie Ausschlüsse, um sicherzustellen, dass Ihr Dialogfeld **not** auf einer bestimmten Seite/in einem bestimmten Bereich Ihrer Site angezeigt werden. Ausschlüsse haben dasselbe Format wie Einschlüsse.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Erstellen eines Dialogfelds](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [Entwerferin bzw. Entwerfer des Streams](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target="_blank"}
>* [Berichte](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
