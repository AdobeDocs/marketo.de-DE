---
unique-page-id: 1147356
description: Informationen zur Protokollierung von E-Mail-Ereignissen - Marketing-Dokumente - Produktdokumentation
title: Informationen zur Protokollierung von E-Mail-Ereignissen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


# Informationen zur Protokollierung von E-Mail-Ereignissen {#understanding-email-event-logging}

Beim Versenden von E-Mails protokolliert Marketo verschiedene Datenpunkte in den Aktivitäten der Person. Hier sind die grundlegenden.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

| Ereignis | Beschreibung |
|---|---|
| Gesendet | Wird jedes Mal protokolliert, wenn eine E-Mail von den Marketing-Servern gesendet wird, unabhängig davon, ob sie tatsächlich zugestellt wird. Abgebrochene E-Mails werden weiterhin als &quot;Gesendet&quot;protokolliert. |
| Ausgeliefert | Wird jedes Mal protokolliert, wenn eine E-Mail vom Empfänger-Mail-Server akzeptiert wird. Das bedeutet nicht, dass Spam-Filter vermieden werden. Für jede gesendete E-Mail kann es nur 1 Versand geben. |
| Harter Absprung | Einige harte Absprünge sind das Ergebnis von Spam-Blöcken, daher werden wir nicht versuchen, diese Person für 24 Stunden in irgendeiner Kampagne per E-Mail zu versenden. Andere harte Absprünge wie nicht vorhandene Postfächer sind dauerhaft, und wir werden die Person nie wieder per E-Mail von irgendeiner Kampagne versenden. |
| Weich gebohrt | Wird protokolliert, wenn eine Serverantwort unklar ist, Mailbox-vollständige oder allgemeine Serverprobleme. Wir führen diese Menschen für einen potenziellen zukünftigen Versand 24-36 Stunden durch eine Wiederholungslogik. Dadurch wird die Person nicht von anderen Mailings ausgeschlossen. |
| Geöffnet | Wird protokolliert, wenn ein Empfänger eine E-Mail mit NICHT blockierten Bildern Ansicht. Pro E-Mail, pro Person und pro Smart-Kampagne wird nur ein geöffnetes Ereignis protokolliert. Wenn sie dieselbe E-Mail zweimal aus ihrem Posteingang öffnen, wird sie nur einmal protokolliert. |
| geklickt | Wird jedes Mal protokolliert, wenn eine dekorierte URL aus der E-Mail in den Browser geladen wird (das Ergebnis des Klicks auf den Link). Normalerweise ist dies der Empfänger klickt, kann aber auch ein Schnitt/Einfügen sein. |
| Nicht abonniert | Wird protokolliert, wenn eine Person auf den Link zum Abbestellen einer E-Mail klickt und das Abbestellen-Formular sendet. |

>[!CAUTION]
>
>Wenn dieselbe E-Mail zweimal von derselben Kampagne an dieselbe Person gesendet wird, wird das **geöffnete** Ereignis maximal 1 Mal protokolliert.

