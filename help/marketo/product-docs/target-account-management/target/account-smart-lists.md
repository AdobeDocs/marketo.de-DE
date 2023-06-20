---
unique-page-id: 11378814
description: Intelligente Kontolisten - Marketo-Dokumente - Produktdokumentation
title: Intelligente Kontolisten
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Intelligente Kontolisten {#account-smart-lists}

So können Sie Ihre hochwertigen Konten schnell und präzise identifizieren.

>[!NOTE]
>
>Diese Funktion ist nur für Benutzer verfügbar, die sowohl über das Target Account Management-Add-on als auch über eine lizenzierte TAM verfügen.

## Erstellen einer intelligenten Kontoliste {#create-an-account-smart-list}

1. Navigieren Sie in Marketo zu **Marketingaktivitäten**.

   ![](assets/account-smart-lists-1.png)

1. Wählen Sie das gewünschte Programm aus.

   ![](assets/account-smart-lists-2.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neues lokales Asset**.

   ![](assets/account-smart-lists-3.png)

1. Klicken **Intelligente Kontoliste**.

   ![](assets/account-smart-lists-4.png)

1. Geben Sie einen Namen ein und klicken Sie auf **Erstellen** (Beschreibung und Beschriftungen sind optional).

   ![](assets/account-smart-lists-5.png)

Ihre Konto-Smart-Liste wurde erstellt! Anweisungen zum Definieren der Regeln finden Sie unten.

## Konto-Smart-List-Regeln {#account-smart-list-rules}

Smart-Listen für Konten funktionieren ähnlich wie standardmäßige Smart-Listen, mit einer wichtigen Ausnahme: Container.

1. Klicken Sie zum Definieren Ihrer Konto-Smart-Liste auf die Schaltfläche **Intelligente Listenregeln für Konten** Registerkarte.

   ![](assets/account-smart-lists-6.png)

1. Wählen Sie die gewünschten Kontofilter aus. In diesem Beispiel wählen wir _Industrie ist Gesundheitswesen_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >In Ihrer [Ranking und Optimierung von Kontoprofilen](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) wird als benutzerdefinierte Kontoattribute angezeigt, die in Ihrer intelligenten Kontoliste verwendet werden können. Diese benutzerdefinierten Attributdaten basieren auf dem Zeitpunkt, zu dem das Kontoprofilmodell erstellt/aktualisiert wurde.

1. Wählen Sie die Filter für übereinstimmende Personen aus. In diesem Beispiel wählen wir _Bundesstaat Kalifornien_.

   ![](assets/account-smart-lists-9.png)

**OPTIONALER SCHRITT**: Hier kommen Container herein. Wenn Sie einen zusätzlichen Filter für übereinstimmende Personen auswählen, können Sie ihn unter den ersten Filter legen oder _in_ Erstellen eines Containers. In diesem Beispiel erstellen wir einen Container, indem wir _Auftragstitel ist CFO_.

![](assets/account-smart-lists-10.png)

So sieht der Container aus.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Beim Erstellen eines Containers mit Filtern wird eine &quot;und&quot;-Regel erstellt, d. h., es werden nur alle kombinierten Ergebnisse zurückgegeben. In diesem Beispiel entfällt eine Branche des Gesundheitswesens auf Kalifornien. _und_ mit einer Person, die als CFO gelistet ist. Wenn Sie keine Container verwenden möchten, legen Sie einfach den Filter unter/über dem vorhandenen ab.

Und das ist es! Im folgenden Abschnitt erfahren Sie, wie Sie Ihre intelligente Kontoliste nutzen können.

>[!TIP]
>
>Wie bei standardmäßigen Smart-Listen können Sie auch erweiterte Logik verwenden, um Ihre Ergebnisse weiter zu verfeinern. Dazu benötigen Sie mindestens drei Filter. In den Konto-Smart-Listen entspricht ein Container (unabhängig von der Anzahl der darin enthaltenen Filter) einem Filter.

## Konto-Smart-List-Aktionen {#account-smart-list-actions}

Auf der Registerkarte Übersicht Ihrer Smart-Liste Konto werden Ihnen einige Aktionsoptionen angezeigt.

**Export**: Dadurch werden die Ergebnisse Ihrer Konto-Smart-Liste als CSV exportiert.

**Klonen**: Kopiert Ihre intelligente Kontoliste.

**An Werbenetzwerk senden**: Sendet die Liste als neue übereinstimmende Zielgruppe an LinkedIn.

Sie können Ihre intelligente Kontoliste auch in einer standardmäßigen Smart-Kampagne/-Liste referenzieren, indem Sie die _Personen, die Mitglied der intelligenten Kontoliste sind_ Filter.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Die Ergebnisse der Smart-Liste &quot;Personen mit Konto&quot;zeigen jede Person in den identifizierten Konten an, nicht nur Personen, die über die Filter für übereinstimmende Personen in der Konto-Smart-Liste gefunden wurden.

>[!NOTE]
>
>**Definition**
>
>**Personen, die Mitglied der intelligenten Kontoliste sind**: In diesem Fall bezieht sich das Wort &quot;Mitglied&quot;auf das Konto selbst, also bedeutet &quot;Mitglied des Benutzers&quot; die Personen (Marketo-Datensätze) in diesen Konten.
