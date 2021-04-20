---
title: understand-my-tokens
description: My Tokens
exl-id: d56748e2-d742-45dd-96a8-dd80e30d9d8b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 5%

---

# My Tokens

<br> 

Meine Tokens sind benutzerspezifische Variablen, die Sie in Ihren Programmen oder Kampagnen-Ordnern erstellen und verwenden können. Sie sehen wie folgt aus: `{{_my.Name of Token_}}`

## Beispiele

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Um My Tokens aufzurufen und zu erstellen, wählen Sie den Ordner &quot;Programm&quot;oder &quot;Kampagne&quot;aus und gehen Sie zur Registerkarte [!UICONTROL My Tokens]. Ziehen Sie ein beliebiges Token auf Ihre Arbeitsfläche [!UICONTROL Lokale Token].

![Bild eins](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Die Namen meiner Tokens können nach dem Speichern nicht mehr geändert werden. Wählen Sie daher sorgfältig aus.

>[!NOTE]
>
>Meine Tokens werden nicht aufgelöst, wenn eine E-Mail von Sales Insight auf Microsoft Dynamics oder Salesforce gesendet wird. Es werden nur Standard-Token ausgefüllt (Interessent, Firma usw.). Die Standardwerte für Token funktionieren jedoch.

>[!NOTE]
>
>Link-Token funktionieren nicht in Nur-Text-E-Mails.

## Verschachteln von Tokens

Wenn Sie ein neues Token erstellen, kann es von anderen Objekten in der Struktur referenziert werden. Sie können globale Variablen auf niedrigeren Ebenen in der Struktur überschreiben. Es gibt eine Benennungsstruktur, bei der das Token zur einfachen Verwaltung erstellt wurde.

* **Lokales Token:** Das Token wurde direkt in diesem Programm oder Ordner erstellt.
* **[Überschriebenes Token:](/help/sky/override-an-inherited-my-token.md)** Das Token wurde geerbt, in diesem Programm oder Ordner wurde jedoch eine Ausnahme gemacht.
* **Erbtes Token:** Das Token wurde in einem übergeordneten Programm oder Ordner in der Struktur erstellt.

Sie finden diese drei Typen auf der Registerkarte **[!UICONTROL Meine Token]** im Ordner &quot;Programm&quot;oder &quot;Kampagne&quot;.

![Bild zwei](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Das Verschieben von Programmen und Ordnern wirkt sich auch auf Token aus. Vergewissern Sie sich stets, dass Verweise während des Verschiebevorgangs nicht beschädigt werden.

>[!NOTE]
>
>Wenn es sich bei der von einem Interaktions-Programm gesendeten E-Mail um eine untergeordnete E-Mail eines Standard-Programms handelt (d. h. nicht lokal in Ihrem Interaktions-Programm), werden alle in der E-Mail verwendeten &quot;Meine Token&quot;aus dem Programm gelöst, in dem sich die untergeordnete E-Mail befindet.

## Token-Verwendung

Wählen Sie ein beliebiges Token aus und klicken Sie dann oben rechts auf das Nutzungssymbol, um eine Liste der Assets anzuzeigen, die dieses Token enthalten.

![Bild drei](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Bild vier](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Vertiefung**

Weitere Informationen zu jedem der My Tokens:

* [CRM-Kampagne](/help/sky/my-token-crm-campaign.md)
* [Datum](/help/sky/my-token-date.md)
* [Kalenderdatei](/help/sky/my-token-calendar-file.md)
* [Bild](/help/sky/my-token-image.md)
* [Link](/help/sky/my-token-link.md)
* [Zahl](/help/sky/my-token-number.md)
* [RTF](/help/sky/my-token-rich-text.md)
* [Bewerten](/help/sky/my-token-score.md)
* [E-Mail-Script](/help/sky/my-token-email-script.md)
* [Text](/help/sky/my-token-text.md)
