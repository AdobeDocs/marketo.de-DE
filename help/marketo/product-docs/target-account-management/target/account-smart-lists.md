---
unique-page-id: 11378814
description: Kontointelligente Listen - Marketo Docs - Produktdokumentation
title: Intelligente Listen
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
translation-type: tm+mt
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 1%

---

# Konto-Smart-Listen {#account-smart-lists}

Hier sehen Sie, wie Sie Ihre hochwertigen Konten schnell und präzise identifizieren können.

>[!NOTE]
>
>Diese Funktion wird für alle qualifizierenden Marketo-Instanzen am Abend des 11. Mai aktiviert.

>[!NOTE]
>
>Diese Funktion ist nur für Benutzer verfügbar, für die sowohl TAM als auch das Adobe Marketo Engage Next-Gen-Benutzererlebnis aktiviert sind.

## Erstellen einer Konto-Smart-Liste {#create-an-account-smart-list}

1. Gehen Sie in Marketo zu **Marketing-Aktivitäten**.

   ![](assets/account-smart-lists-1.png)

1. Wählen Sie das gewünschte Programm aus.

   ![](assets/account-smart-lists-2.png)

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neues lokales Element**.

   ![](assets/account-smart-lists-3.png)

1. Klicken Sie auf **Intelligente Konto-Liste**.

   ![](assets/account-smart-lists-4.png)

1. Geben Sie einen Namen ein und klicken Sie auf **Erstellen** (Beschreibung und Bezeichnungen sind optional).

   ![](assets/account-smart-lists-5.png)

Ihre Account Smart Liste wurde erstellt! Die Schritte zum Definieren der Regeln finden Sie unten.

## Konto-Smart-List-Regeln {#account-smart-list-rules}

Intelligente Kontoausnahmen funktionieren ähnlich wie normale Smart-Listen, mit einer bemerkenswerten Ausnahme: Container.

1. Klicken Sie zum Definieren der Smart-Liste Ihres Kontos auf die Registerkarte **Regeln für die intelligente Liste des Kontos**.

   ![](assets/account-smart-lists-6.png)

1. Wählen Sie die gewünschten Kontofilter aus. In diesem Beispiel wählen wir _Industrie ist Gesundheitswesen_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. Wählen Sie Ihre Filter für übereinstimmende Personen aus. In diesem Beispiel wählen wir _Bundesland ist Kalifornien_.

   ![](assets/account-smart-lists-9.png)

**Optionaler Schritt**: Hier kommen Container herein. Wenn Sie einen weiteren Filter für übereinstimmende Personen auswählen, können Sie ihn unter dem ersten oder unter _unter_ ablegen und einen Container erstellen. In diesem Beispiel erstellen wir einen Container, indem wir _Auftragstitel CFO_ hinzufügen.

![](assets/account-smart-lists-10.png)

So sieht der Container aus.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Beim Erstellen eines Containers von Filtern wird eine &quot;Und&quot;-Regel erstellt, d. h., es werden nur alle kombinierten Ergebnisse zurückgegeben. In diesem Beispiel werden Konten mit einer Branche der Gesundheitsversorgung zusammen mit dem Standort in Kalifornien _und_ mit einer Person als CFO aufgeführt. Wenn Sie keine Container verwenden möchten, legen Sie den Filter einfach unter/über dem vorhandenen Filter ab.

Und das ist es! Sehen Sie sich den unten stehenden Abschnitt an, um zu sehen, wie Sie Ihre Konto-Smart-Liste nutzen können.

>[!TIP]
>
>Genau wie bei standardmäßigen Smart-Listen können Sie mit fortschrittlicher Logik Ihre Ergebnisse weiter verfeinern. Dazu benötigen Sie mindestens drei Filter, und bei den Account-Smart-Listen ist ein Container (unabhängig von der Anzahl der darin enthaltenen Filter) gleich einem Filter.

## Konto-Smart-List-Aktionen {#account-smart-list-actions}

Auf der Registerkarte Übersicht Ihrer Konto-Smart-Liste werden Sie einige Aktionsoptionen sehen.

**Exportieren**: Dadurch werden die Ergebnisse Ihrer Account Smart-Liste als CSV exportiert.

**Klonen**: Erstellt eine Kopie der Smart-Liste Ihres Kontos.

**An Werbenetzwerk** senden: Sendet die Liste als neue übereinstimmende Audience an LinkedIn.

Sie können Ihre Konto-Smart-Liste auch in einer standardmäßigen Smart-Kampagne/Liste referenzieren, indem Sie den Filter _People Member of Account Smart Liste_ verwenden.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Die Ergebnisse der People Member of Account Smart-Liste zeigen jede Person in dem/den angegebenen Konto(en) an, nicht nur Personen, die über die Filter von &quot;Matched Person&quot;in der Liste &quot;Account Smart&quot;gefunden werden.

>[!NOTE]
>
>**Definition**
>
>**Personen, die Mitglied der Smart-Liste** des Kontos sind: In diesem Fall bezieht sich das Wort &quot;Mitglied&quot; auf das Konto selbst, sodass &quot;Mitglied der Person&quot; die tatsächlichen Personen (Marketo-Aufzeichnungen) in diesen Konten.
