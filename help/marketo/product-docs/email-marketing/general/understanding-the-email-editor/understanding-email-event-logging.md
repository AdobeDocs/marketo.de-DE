---
unique-page-id: 1147356
description: Grundlagen zur Protokollierung von E-Mail-Ereignissen - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zur E-Mail-Ereignisprotokollierung
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 3%

---

# Grundlagen zur E-Mail-Ereignisprotokollierung {#understanding-email-event-logging}

Beim Versand von E-Mails protokolliert Marketo verschiedene Datenpunkte in den Aktivitätsprotokollen der Person. Hier sind die grundlegendsten.

| Veranstaltung | Beschreibung |
|---|---|
| Gesendet | Wird jedes Mal protokolliert, wenn eine E-Mail von den Marketo-Servern gesendet wird, unabhängig davon, ob sie tatsächlich zugestellt wird. Bounce Messages werden weiterhin als „Gesendet“ protokolliert. |
| Zugestellt | Wird jedes Mal protokolliert, wenn eine E-Mail vom Empfänger-Mail-Server akzeptiert wird. Dies bedeutet nicht, dass Spam-Filter vermieden wurden. Es kann nur einen Versand pro gesendeter E-Mail geben. |
| Hard Bounce-Ereignis aufgetreten | Einige Hardbounces sind das Ergebnis von Spam-Sperren, sodass wir in keiner Kampagne versuchen werden, dieser Person 24 Stunden lang eine E-Mail zu senden. Andere Hardbounces wie nicht vorhandene Posteingänge sind dauerhaft und wir werden der Person nie wieder eine E-Mail von einer Kampagne senden. |
| Soft Bounce-Ereignis aufgetreten | Wird protokolliert, wenn eine Server-Antwort unklar, Postfach voll oder allgemeine Server-Probleme ist. Wir setzen diese Personen für 24-36 Stunden durch eine Logik für weitere Zustellversuche. Dies schließt die Person nicht von anderen Mailings aus. |
| Geöffnet | Wird protokolliert, wenn ein Empfänger eine E-Mail mit NICHT blockierten Bildern anzeigt. Pro Smart-Kampagne wird nur ein offenes Ereignis pro E-Mail, pro Person protokolliert. Wenn dieselbe E-Mail zweimal in ihrem Posteingang geöffnet wird, wird sie nur einmal protokolliert. |
| Angeklickt | Wird jedes Mal protokolliert, wenn eine dekorierte URL aus der E-Mail in den Browser geladen wird (das Ergebnis des Klicks auf den Link). Normalerweise ist dies der Empfänger, der klickt, aber es kann auch ein Ausschneiden/Einfügen sein. |
| Abbestellt | Wird protokolliert, wenn eine Person auf den Abmelde-Link einer E-Mail klickt und das Abmeldeformular sendet. |

>[!CAUTION]
>
>Wenn dieselbe E-Mail zweimal von derselben Kampagne an dieselbe Person gesendet wird **wird das** Geöffnet“ maximal 1 Mal protokolliert.
