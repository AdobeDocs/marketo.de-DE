---
description: Zielgruppenkriterien - Marketo-Dokumente - Produktdokumentation
title: Zielgruppenkriterien
feature: Dynamic Chat
exl-id: 95c4558e-0c0c-4623-bb7d-b6ac2f455c01
source-git-commit: f5f93a993d5b13c1fda0b31172393eff0bc65fd4
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Zielgruppenkriterien {#audience-criteria}

Ähnlich wie bei der Marketo Engage von Smart-Listen ermöglichen Ihnen Zielgruppenkriterien-Attribute die Definition Ihrer Zielgruppe. Sie können bekannte oder unbekannte Personen mithilfe von Inferred, Person oder Unternehmensattributen (oder einer Kombination daraus) ansprechen.

## Priorität {#priority}

Die Priorität bestimmt, welches Dialogfeld ein Lead erhält, falls er für mehr als ein Feld qualifiziert ist. Sie wird zum ersten Mal festgelegt [Erstellen eines Dialogfelds](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}. Sie können die Priorität eines vorhandenen Dialogfelds ändern, indem Sie es öffnen und **[!UICONTROL Dialogfelddetails]** auf der Registerkarte Zielgruppenkriterien .

![](assets/audience-criteria-1.png)

## Ereignisse {#events}

Mit Ereignissen können Sie Besucher auf Basis des Bildlaufs oder der Dauer des Bildlaufs auf Ihrer Seite/Site als Ziel auswählen. Im folgenden Beispiel werden Besucher angesprochen, die sich seit mehr als 20 Sekunden auf einer bestimmten Seite befinden.

1. Grab die **[!UICONTROL Besuchszeit pro Seite]** -Ereignis ein und ziehen Sie es nach rechts.

   ![](assets/audience-criteria-3.png)

1. Legen Sie die Zeit &quot;Größer als&quot;auf 20 Sekunden fest.

   ![](assets/audience-criteria-4.png)

1. Fügen Sie im [Target](#target) Abschnitt.

   ![](assets/audience-criteria-5.png)

## Attribute {#attributes}

**Bekannte Personen**

Es gibt _many_ Attributkombinationen zur Auswahl. Im folgenden Beispiel richten wir uns an alle bekannten Personen in Kalifornien, die in einem Unternehmen mit mehr als 50 Mitarbeitern arbeiten.

1. Grab die **[!UICONTROL Bundesland]** -Attribut fest und ziehen Sie es nach rechts.

   ![](assets/audience-criteria-7.png)

1. _Is_ ist standardmäßig festgelegt. Geben Sie im Feld Werte auswählen eine Zertifizierungsstelle ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/audience-criteria-8.png)

1. Grab die **[!UICONTROL Firmengröße]** Attribut hinzufügen und an die gewünschte Position ziehen _Attribut hier ziehen und ablegen_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >Sie können auch ein Attribut auswählen, indem Sie auf dessen **+** Symbol.

1. Klicken Sie auf die Dropdown-Liste Operator und wählen Sie **[!UICONTROL Größer als]**.

   ![](assets/audience-criteria-10.png)

1. Geben Sie 50 ein und klicken Sie auf eine andere Stelle auf dem Bildschirm, um zu speichern.

   ![](assets/audience-criteria-11.png)

Und das ist es!

**Anonyme Personen**

Es gibt eine einfache Möglichkeit, Personen gezielt anzusprechen, die noch nicht in Ihrer Datenbank sind. In diesem Beispiel richten wir uns an alle anonymen Personen im Raum New York.

1. Grab die **[!UICONTROL Personen-Email]** -Attribut fest und ziehen Sie es nach rechts.

   ![](assets/audience-criteria-12.png)

1. Klicken Sie auf die Dropdown-Liste Operator und wählen Sie **[!UICONTROL Ist leer]**.

   ![](assets/audience-criteria-13.png)

1. Grab die **[!UICONTROL Abgegrenzter Status]** Attribut hinzufügen und an die gewünschte Position ziehen _Attribut hier ziehen und ablegen_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Wenn jemand Ihre Website besucht, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} Cookies und setzt sie in das System. Wir suchen ihre IP-Adresse in einer speziellen Datenbank und schließen alle möglichen guten Informationen.

1. _Is_ ist standardmäßig festgelegt. Geben Sie im Feld Werte auswählen NY ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/audience-criteria-15.png)

## Mitgliedschaft {#membership}

Verwenden Sie Marketo Engage Smart Lists für die Ziel-Audience Ihres Dialogfelds.

>[!AVAILABILITY]
>
>Mitglied der Smart List oder Mitglied der List-Kriterien erfordert Dynamic Chat Prime. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

1. Nehmen Sie unter Mitgliedschaft **[!UICONTROL Mitglied der Smart List]** und legen Sie es auf die Arbeitsfläche.

   ![](assets/audience-criteria-15a.png)

1. Wählen Sie die gewünschte Smart-Liste aus.

   ![](assets/audience-criteria-15b.png)

## Gruppen hinzufügen {#add-groups}

Sie haben auch die Möglichkeit, Attribute zu gruppieren, falls Sie alle Attribute zusammen mit &quot;all&quot;oder &quot;any&quot;eines anderen Attributs haben möchten. Sie können mehrere Gruppen hinzufügen.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Target {#target}

Hier geben Sie die URL(s) ein, für die ein bestimmtes Dialogfeld angezeigt werden soll. Sie haben auch die Möglichkeit, Ausschlüsse hinzuzufügen.

Zulässige Formate:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>Die Verwendung eines Sternchens dient als Platzhalter. Also `https://*.website.com` würde das Dialogfeld auf jeder Seite der Site platzieren, einschließlich Subdomains (z. B.: `support.website.com`). und `https://website.com/folder/*` würde das Dialogfeld auf jeder HTML-Seite im folgenden Ordner platzieren (z. B.: in diesem Fall ist der Ordner &quot;Sport&quot;, also: website.com/sports/baseball.html, website.com/sports/football.html usw.).

**Ausnahmen**

Verwenden Sie Ausschlüsse, um sicherzustellen, dass Ihr Dialogfeld _not_ auf einer bestimmten Seite/in einem bestimmten Bereich Ihrer Site angezeigt werden. Ausschlüsse haben dasselbe Format wie Einschlüsse.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Erstellen eines Dialogfelds](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Stream-Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}
