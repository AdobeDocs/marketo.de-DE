---
unique-page-id: 11378814
description: Intelligente Kontolisten - Marketo-Dokumente - Produktdokumentation
title: Intelligente Kontolisten
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
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

1. Wechseln Sie in Marketo zu **Marketingaktivitäten**.

   ![](assets/account-smart-lists-1.png)

1. Wählen Sie das gewünschte Programm aus.

   ![](assets/account-smart-lists-2.png)

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neues lokales Asset** aus.

   ![](assets/account-smart-lists-3.png)

1. Klicken Sie auf **Intelligente Kontoliste**.

   ![](assets/account-smart-lists-4.png)

1. Geben Sie einen Namen ein und klicken Sie auf **Erstellen** (Beschreibung und Beschriftungen sind optional).

   ![](assets/account-smart-lists-5.png)

Ihre Konto-Smart-Liste wurde erstellt! Anweisungen zum Definieren der Regeln finden Sie unten.

## Konto-Smart-List-Regeln {#account-smart-list-rules}

Smart-Listen für Konten funktionieren ähnlich wie standardmäßige Smart-Listen, mit einer wichtigen Ausnahme: Container.

1. Um Ihre intelligente Kontoliste zu definieren, klicken Sie auf die Registerkarte **Regeln für intelligente Kontoliste** .

   ![](assets/account-smart-lists-6.png)

1. Wählen Sie die gewünschten Kontofilter aus. In diesem Beispiel wählen wir _Branche ist Gesundheitsfürsorge_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >ICP-Indikatordaten, die in Ihrer [Konto-Profiling-Ranking und -Optimierung](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) verwendet wurden, werden als benutzerdefinierte Kontoattribute zur Verwendung in Ihrer Konto-Smart-Liste angezeigt. Diese benutzerdefinierten Attributdaten basieren auf dem Zeitpunkt, zu dem das Kontoprofilmodell erstellt/aktualisiert wurde.

1. Wählen Sie die Filter für übereinstimmende Personen aus. In diesem Beispiel wählen wir &quot;_Bundesstaat ist Kalifornien_&quot;.

   ![](assets/account-smart-lists-9.png)

**OPTIONALER SCHRITT**: Hier kommen Container herein. Wenn Sie einen zusätzlichen Filter für übereinstimmende Personen auswählen, können Sie ihn unter den ersten oder unter _in_ ablegen und so einen Container erstellen. In diesem Beispiel erstellen wir einen Container, indem wir _Auftragstitel ist CFO_ hinzufügen.

![](assets/account-smart-lists-10.png)

So sieht der Container aus.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Beim Erstellen eines Containers mit Filtern wird eine &quot;und&quot;-Regel erstellt, d. h., es werden nur alle kombinierten Ergebnisse zurückgegeben. In diesem Beispiel wird eine Branche der Gesundheitsversorgung mit Standorten in Kalifornien _und_ und einer als CFO gelisteten Person erfasst. Wenn Sie keine Container verwenden möchten, legen Sie einfach den Filter unter/über dem vorhandenen ab.

Und das ist es! Im folgenden Abschnitt erfahren Sie, wie Sie Ihre intelligente Kontoliste nutzen können.

>[!TIP]
>
>Wie bei standardmäßigen Smart-Listen können Sie auch erweiterte Logik verwenden, um Ihre Ergebnisse weiter zu verfeinern. Dazu benötigen Sie mindestens drei Filter. In den Konto-Smart-Listen entspricht ein Container (unabhängig von der Anzahl der darin enthaltenen Filter) einem Filter.

## Konto-Smart-List-Aktionen {#account-smart-list-actions}

Auf der Registerkarte Übersicht Ihrer Smart-Liste Konto werden Ihnen einige Aktionsoptionen angezeigt.

**Exportieren**: Dadurch werden die Ergebnisse Ihrer Konto-Smart-Liste als CSV exportiert.

**Klonen**: Kopiert Ihre intelligente Kontoliste.

**An Anzeigennetzwerk senden**: Sendet die Liste als neue übereinstimmende Zielgruppe an LinkedIn.

Sie können Ihre intelligente Kontoliste auch in einer standardmäßigen Smart-Kampagne/Liste referenzieren, indem Sie den Filter _Personen, die Mitglied der intelligenten Kontoliste sind_ sind, verwenden.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Die Ergebnisse der Smart-Liste &quot;Personen mit Konto&quot;zeigen jede Person in den identifizierten Konten an, nicht nur Personen, die über die Filter für übereinstimmende Personen in der Konto-Smart-Liste gefunden wurden.

>[!NOTE]
>
>**Definition**
>
>**Personen, die der intelligenten Kontoliste angehören**: In diesem Fall bezieht sich das Wort &quot;Mitglied&quot;auf das Konto selbst, sodass &quot;Mitglied des Kontos&quot;die tatsächlichen Personen (Marketo-Datensätze) in diesen Konten bezeichnet.
