---
unique-page-id: 1147356
description: Verstehen der E-Mail-Ereignisprotokollierung - Marketo-Dokumente - Produktdokumentation
title: Informationen zur E-Mail-Ereignisprotokollierung
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 3%

---

# Informationen zur E-Mail-Ereignisprotokollierung {#understanding-email-event-logging}

Beim Senden von E-Mails protokolliert Marketo verschiedene Datenpunkte in den Aktivitätsprotokollen der Person. Hier sind die grundlegenden.

| Veranstaltung | Beschreibung |
|---|---|
| Gesendet | Wird jedes Mal protokolliert, wenn eine E-Mail von den Marketo-Servern gesendet wird, unabhängig davon, ob sie tatsächlich gesendet wird. Bounce Messages werden weiterhin als &quot;Gesendet&quot;protokolliert. |
| Zugestellt | Wird jedes Mal protokolliert, wenn eine E-Mail vom Empfänger-E-Mail-Server akzeptiert wird. Dies bedeutet nicht, dass Spam-Filter vermieden werden. Es kann nur 1 Versand pro gesendeter E-Mail geben. |
| Hard Bounce-Ereignis aufgetreten | Manche Hardbounces sind das Ergebnis von Spam-Blöcken. Daher werden wir in keiner Kampagne versuchen, diese Person 24 Stunden lang per E-Mail zu versenden. Andere Hardbounces wie nicht vorhandene Postfächer sind dauerhaft, und wir werden die Person nie wieder per E-Mail von einer Kampagne versenden. |
| Soft Bounce-Ereignis aufgetreten | Wird protokolliert, wenn eine Server-Antwort unklar ist, Postfach voll ist oder allgemeine Serverprobleme auftreten. Wir führen diese Personen 24 bis 36 Stunden lang durch, um eine potenzielle zukünftige Bereitstellung zu ermöglichen. Dadurch wird die Person nicht von anderen Mailings ausgeschlossen. |
| Geöffnet | Wird protokolliert, wenn ein Empfänger eine E-Mail mit NICHT blockierten Bildern anzeigt. Pro E-Mail, Person und Smart-Kampagne wird nur ein einziges Öffnungs-Ereignis protokolliert. Wenn sie dieselbe E-Mail zweimal aus ihrem Posteingang öffnen, wird sie nur einmal protokolliert. |
| Angeklickt | wird jedes Mal protokolliert, wenn eine dekorierte URL aus der E-Mail im Browser geladen wird (Ergebnis des Klicks auf den Link). Normalerweise ist dies der Empfänger, der klickt, kann aber auch ein Schnitt/Einfügen sein. |
| Abbestellt | Wird protokolliert, wenn eine Person auf den Abmelde-Link einer E-Mail klickt und das Abmeldeformular sendet. |

>[!CAUTION]
>
>Wenn dieselbe E-Mail zweimal von derselben Kampagne an dieselbe Person gesendet wird, wird das Ereignis **Geöffnet** maximal 1 Mal protokolliert.
