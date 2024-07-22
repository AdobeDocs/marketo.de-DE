---
description: SMS-Glossar - Marketo-Dokumente - Produktdokumentation
title: SMS-Glossar
feature: Mobile Marketing
exl-id: 0c23ca9f-f994-42ae-bd72-7d37289b7a94
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 1%

---

# SMS-Glossar {#sms-glossary}

Im Folgenden finden Sie einige häufig verwendete Begriffe, auf die Sie bei der Verwendung von Vibes SMS-Nachrichten mit Marketo Engage stoßen.

<table>
<thead>
  <tr>
    <th>Begriff</th>
    <th>Definition</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Akquisekampagne</td>
    <td>Eine Kampagne zum Erwerb neuer Abonnenten auf Ihren Abonnementlisten. Ein Abonnent kann über ein Marketo-Webformular oder durch SMS zu einer Akquisekampagne hinzugefügt werden.</td>
  </tr>
  <tr>
    <td>Kampagnen-Manager</td>
    <td>In Campaign Manager auf der Plattform "Vibes"können Sie eine Abonnementliste und eine Akquisekampagne einrichten. Benutzer mit einer vollständigen Vibes-Plattformlizenz haben Zugriff auf zusätzliche Kampagnentypen.</td>
  </tr>
  <tr>
    <td>Unternehmensschlüssel</td>
    <td>Der company_key ist eine eindeutige alphanumerische Kennung für Ihr Plattformkonto. Wenn Sie über mehrere Unternehmenskonten in der Vibes-Plattform verfügen (z. B. untergeordnete Konten), können Sie über mehrere company_keys verfügen. Jede Instanz von Marketo Engage kann nur einem Vibes company_key zugeordnet werden.</td>
  </tr>
  <tr>
    <td>CTA (Aktionsaufruf)</td>
    <td>Digitale oder physische Beschilderung oder verbale Skripte zum Erwerb von Abonnenten in einem wiederkehrenden Textnachrichtenprogramm oder einer Abonnementliste. Können online, in sozialen Medien, in E-Mails, in Druckform usw. platziert werden.</td>
  </tr>
  <tr>
    <td>Benutzerdefinierte kurze Domäne</td>
    <td>Wenn Sie den Link-Shortener "Vibes"verwenden, wird die gekürzte URL standardmäßig unter der kurzen URL "Vibes"angezeigt: https://vbs.cm/xxxxxx. Eine benutzerdefinierte kurze Domäne ist eine Domäne, die für Ihre Marke eindeutig ist. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">Erfahren Sie mehr über benutzerdefinierte kurze Domänen</a>.<p>
    Dies gilt nur für Nachrichten, die von der Vibes-Plattform gesendet werden, insbesondere Akquise-Kampagnennachrichten und Standardnachrichten mit Kurzwahlnummern.<p>
    Es wird empfohlen, den Marketo-URL-Shortener zu verwenden, um Klickdaten in Ihrem Marketo-Programm zu haben.</td>
  </tr>
  <tr>
    <td>Standardmeldungen</td>
    <td>Obligatorische Meldungen für die Kurzwahlnummer zur Beantwortung von HELP-, STOP- und nicht erkannten Nachrichtenanfragen.</td>
  </tr>
  <tr>
    <td>Verbindung trennen</td>
    <td>Trennzeichen sind eine Form des Opt-outs, da die Mobiltelefonnummer aus einem Mobilfunknetz entfernt wird. Gründe für eine Abschaltung sind unter anderem die vollständige Schließung eines Kontos, das Auslaufen eines Guthabenkontos oder die Streichung der Nummer aus dem Betreibernetz aus anderen unbekannten Gründen. Mobiltelefonnummern, die getrennt und nicht auf einen anderen Mobilnetzbetreiber portiert werden, werden von allen Abonnementlisten auf der Vibes-Plattform abgemeldet.</td>
  </tr>
  <tr>
    <td>Double Opt-in</td>
    <td>Eine Akquisemethode, bei der ein potenzieller Abonnent seine Zustimmung zum Hinzufügen zu einer Abonnementliste mit einem Antwortbefehl wie "Y"oder seiner Postleitzahl bestätigen muss. Die Verwendung einer doppelten Anmeldeaufforderung kann Ihnen bei der Einhaltung der Richtlinien für den staatlichen und föderalen Textnachrichtenversand helfen.</td>
  </tr>
  <tr>
    <td>Veranstaltung</td>
    <td>Ein Ereignis ist ein definiertes Ereignis, das an die Vibes-Plattform gesendet und zum Trigger API-gesteuerter Aktionen verwendet werden kann, einschließlich Nachrichtensendungen. Jedes Ereignis enthält ereignisspezifische Daten, einschließlich event_type, mit denen bestimmt wird, welcher API-ausgelösten Nachrichtenkampagne es entspricht. Die Ereignis-API kann über Webhook in Marketo Engage ausgelöst werden. Weitere Informationen finden Sie in der <a href="https://developer-platform.vibes.com/reference/event-api">Ereignis-API-Referenz</a>.</td>
  </tr>
  <tr>
    <td>Keyword</td>
    <td>Ein kurzes Wort oder eine alphanumerische Zeichenfolge, die vom Verbraucher an die Kurzwahlnummer gesendet wird, um ein mobiles Erlebnis zu initiieren.</td>
  </tr>
  <tr>
    <td>Long Code (10DLC)</td>
    <td>Eine Absender-ID, mit der zwischen Marke und Verbraucher Nachrichten in beide Richtungen gesendet werden. US-lange Codes sind 10 numerische Ziffern.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Mobiltelefonnummer oder Telefonnummer einer Person. MDN- und Mobiltelefonnummern sind in Marketo keine eindeutigen Kennungen.</td>
  </tr>
  <tr>
    <td>Mobile Datenbank</td>
    <td>Die mobile Datenbank ist die Datenbank, in der Vibes Abonnentendaten speichert. Jeder Abonnent verfügt über einen eindeutigen "Personendatensatz", in dem die Mobiltelefonnummer und alle zugehörigen benutzerdefinierten Felder ausgefüllt sind.</td>
  </tr>
  <tr>
    <td>Teilnehmer</td>
    <td>Eine Person, die über eine oder mehrere mobile Interaktionen (z. B. das Senden einer Textnachricht) mit Ihrem Mobilprogramm verfügt, sich jedoch nicht für eine Abonnementliste angemeldet hat.</td>
  </tr>
  <tr>
    <td>Personenaufzeichnung</td>
    <td>Ein Personendatensatz ist eine Sammlung von Daten für eine bestimmte Mobiltelefonnummer. Jedem Personendatensatz wird auch ein eindeutiger person_key zur Identifizierung zugewiesen. Marketo-IDs werden über das Feld external_person_id mit Vibes verknüpft. Weitere Informationen zu Personendatensätzen finden Sie in der Dokumentation zur Personen-API </a> von <a href="https://developer-platform.vibes.com/reference/person-api">Vibes Person.</td>
  </tr>
  <tr>
    <td>Kurzwahlnummer</td>
    <td>Eine Absender-ID, mit der zwischen Marke und Verbraucher Nachrichten in beide Richtungen gesendet werden. US-Kurzwahlnummern sind 5 bis 6 numerische Ziffern. Kanadische Kurzwahlnummern sind 4 bis 6 numerische Ziffern. Die Marketo LaunchPoint-Integration in Vibes unterstützt eine Kurzwahlnummer pro Instanz.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Kurznachrichtendienst. Dies ist eine Nachricht, die nur Text enthält.</td>
  </tr>
  <tr>
    <td>Abonnementlisten</td>
    <td>Eine Liste der Mobiltelefonnummern (und der zugehörigen Personendatensätze), die die Zustimmung zum Erhalt wiederkehrender Nachrichten von Ihrem Programm gegeben haben.</td>
  </tr>
  <tr>
    <td>Abonnent</td>
    <td>Eine Mobiltelefonnummer, die für eine oder mehrere Abonnementlisten angemeldet ist.</td>
  </tr>
  <tr>
    <td>Vibes Platform</td>
    <td>Die Website, bei der Sie sich zur Verwaltung Ihrer Kampagnen anmelden. Rufen Sie <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> auf, um auf die Plattform "Vibes"zuzugreifen.</td>
  </tr>
</tbody>
</table>
