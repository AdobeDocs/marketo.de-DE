---
unique-page-id: 11378814
description: Smart-Listen für Konten - Marketo-Dokumente - Produktdokumentation
title: Smart-Listen für Konten
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Smart-Listen für Konten {#account-smart-lists}

So können Sie schnell und präzise Ihre hochwertigen Konten identifizieren.

>[!NOTE]
>
>Diese Funktion steht nur jenen zur Verfügung, die sowohl über das Add-on „Target Account Management“ als auch über eine TAM-Lizenz verfügen.

## Erstellen einer Smart-Liste für Konten {#create-an-account-smart-list}

1. Navigieren Sie in Marketo zu **Marketing-Aktivitäten**.

   ![](assets/account-smart-lists-1.png)

1. Suchen und wählen Sie Ihr gewünschtes Programm aus.

   ![](assets/account-smart-lists-2.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neues lokales Asset**.

   ![](assets/account-smart-lists-3.png)

1. Klicken Sie **Smart-Liste Konto**.

   ![](assets/account-smart-lists-4.png)

1. Geben Sie einen Namen ein und klicken Sie auf **Erstellen** (Beschreibung und Beschriftungen sind optional).

   ![](assets/account-smart-lists-5.png)

Die Smart List Ihres Kontos wurde erstellt! Anweisungen zum Definieren der Regeln finden Sie unten.

## Konto-Smart-List-Regeln {#account-smart-list-rules}

Account-Smart-Listen funktionieren ähnlich wie Standard-Smart-Listen, mit einer bemerkenswerten Ausnahme: Container.

1. Um Ihre Smart-Liste für Konten zu definieren, klicken Sie auf die Registerkarte **Regeln für Smart-Listen für**.

   ![](assets/account-smart-lists-6.png)

1. Wählen Sie Ihre gewünschten Kontofilter aus. In diesem Beispiel wählen wir &quot;_ist Healthcare_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >Die ICP-Indikatordaten, die in Ihrem [Account-Profiling, Ranking und Tuning](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) verwendet wurden, werden als benutzerdefinierte Kontoattribute zur Verwendung in Ihrer Account-Smart-Liste angezeigt. Diese benutzerdefinierten Attributdaten basieren auf dem Zeitpunkt, zu dem das Kontoprofilmodell erstellt/aktualisiert wurde.

1. Wählen Sie Ihre passenden Personenfilter aus. In diesem Beispiel wählen wir &quot;_ist Kalifornien_.

   ![](assets/account-smart-lists-9.png)

**OPTIONALER SCHRITT**: Hier kommen Container ins Spiel. Wenn Sie einen zusätzlichen Filter für übereinstimmende Personen auswählen, können Sie ihn unter dem ersten Filter ablegen oder _in_ einen Container erstellen. In diesem Beispiel erstellen wir einen Container, indem wir _Auftragstitel ist CFO_ hinzufügen.

![](assets/account-smart-lists-10.png)

So wird der Container aussehen.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Beim Erstellen eines Containers mit Filtern wird eine „Und“-Regel erstellt, d. h. es werden nur alle Ergebnisse kombiniert zurückgegeben. In diesem Beispiel Konten bei einer Branche des Gesundheitswesens zusammen mit einem Standort in Kalifornien _und_ mit einer Person, die als CFO aufgeführt ist. Wenn Sie keine Container verwenden möchten, legen Sie den Filter einfach unter/über dem vorhandenen ab.

Und das war&#39;s! Im folgenden Abschnitt erfahren Sie, wie Sie Ihre Smart List für Konten nutzen können.

>[!TIP]
>
>Genau wie bei standardmäßigen Smart Lists können Sie erweiterte Logik verwenden, um Ihre Ergebnisse weiter zu verfeinern. Dazu benötigen Sie mindestens drei Filter. Bei Smart Lists für Konten entspricht ein Container (unabhängig davon, wie viele Filter er enthält) einem Filter.

## Konto-Smart-List-Aktionen {#account-smart-list-actions}

Auf der Registerkarte Übersicht Ihrer Smart List für das Konto werden Sie einige Aktionsoptionen feststellen.

**Exportieren**: Dadurch werden die Ergebnisse Ihrer Smart-Liste „Konto“ als CSV-Datei exportiert.

**Klonen**: Erstellt eine Kopie der Smart-Liste Ihres Kontos.

**An Werbenetzwerk senden**: Sendet die Liste als neue übereinstimmende Zielgruppe an LinkedIn.

Sie können auch in einer standardmäßigen Smart-Kampagne/Liste auf Ihre Smart-Liste für Konten verweisen, indem Sie den Filter _Personen Mitglied der Smart-Liste_ Kontos“ verwenden.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Die Ergebnisse der Smart-Liste Personen Mitglied des Kontos zeigen jede Person in den identifizierten Konten an, nicht nur Personen, die über Filter für übereinstimmende Personen in der Smart-Liste des Kontos gefunden werden.

>[!NOTE]
>
>**Definition**
>
>**Personen-Mitglied der Konto-Smart-**: In diesem Fall bezieht sich das Wort „Mitglied“ auf das Konto selbst, sodass „Personen-Mitglied“ die tatsächlichen Personen (Marketo-Einträge) in diesen Konten bedeutet.
