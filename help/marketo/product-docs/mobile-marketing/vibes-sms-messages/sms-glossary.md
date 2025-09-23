---
description: SMS-Glossar - Marketo-Dokumente - Produktdokumentation
title: SMS-Glossar
feature: Mobile Marketing
exl-id: 0c23ca9f-f994-42ae-bd72-7d37289b7a94
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 2%

---

# SMS-Glossar {#sms-glossary}

Im Folgenden finden Sie einige allgemeine Begriffe, die bei der Verwendung von Vibes-SMS-Nachrichten mit Marketo Engage auftreten können.

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
    <td>Eine Kampagne zur Akquise neuer Abonnenten auf Ihren Abonnement-Listen. Ein Abonnent kann einer Akquisekampagne über ein Marketo-Web-Formular oder durch SMS an ein Keyword hinzugefügt werden.</td>
  </tr>
  <tr>
    <td>Kampagnen-Manager</td>
    <td>Campaign Manager befindet sich auf der Vibes-Plattform, wo Sie eine Abonnement-Liste und eine Akquise-Kampagne einrichten können. Benutzer mit einer vollständigen Vibes Platform-Lizenz haben Zugriff auf zusätzliche Kampagnentypen.</td>
  </tr>
  <tr>
    <td>Unternehmensschlüssel</td>
    <td>Der company_key ist eine eindeutige alphanumerische Kennung für Ihr Platform-Konto. Wenn Sie mehrere Unternehmenskonten in der Vibes-Plattform haben (z. B. untergeordnete Konten), können Sie mehrere company_keys haben. Jede Instanz von Marketo Engage kann nur einem Vibes-Unternehmensschlüssel zugeordnet werden.</td>
  </tr>
  <tr>
    <td>CTA (call to action)</td>
    <td>Digitale oder physische Beschilderung oder verbales Script zur Aufnahme von Abonnenten in ein wiederkehrendes Textnachrichtenprogramm oder Abonnementliste. Kann online, in sozialen Medien, in E-Mails, in gedruckten Medien usw. platziert werden.</td>
  </tr>
  <tr>
    <td>Benutzerdefinierte kurze Domain</td>
    <td>Wenn Sie den gekürzten Link Vibes verwenden, wird die gekürzte URL standardmäßig unter der kurzen URL Vibes angezeigt: https://vbs.cm/xxxxxx. Eine benutzerdefinierte kurze Domain ist eine Domain, die eindeutig für Ihre Marke ist. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">Weitere Informationen zu benutzerdefinierten kurzen Domains</a>.<p>
    Dies gilt nur für Nachrichten, die von der Vibes-Plattform gesendet werden, insbesondere für die Akquise-Kampagnen-Nachrichten und die Standard-Kurzwahlnummern.<p>
    Der Marketo-URL-Kürzer wird empfohlen, um Klickdaten in Ihrem Marketo-Programm zu haben.</td>
  </tr>
  <tr>
    <td>Standardnachrichten</td>
    <td>Obligatorische Nachrichten für die Kurzwahlnummer, um auf HILFE-, STOP- und nicht erkannte Nachrichtenanfragen zu antworten.</td>
  </tr>
  <tr>
    <td>Verbindung trennen</td>
    <td>Trennungen sind eine Form des Opt-outs, da die Mobilfunknummer aus einem Betreibernetz entfernt wird. Gründe für eine Unterbrechung sind: Ein Konto wurde vollständig geschlossen, einem Prepaid-Konto ging das Geld aus oder die Nummer wurde aus anderen unbekannten Gründen aus dem Betreibernetz entfernt. Mobiltelefonnummern, die nicht mit einem anderen Mobilnetzbetreiber verbunden sind, werden von allen Abonnementlisten in der Vibes-Plattform abgemeldet.</td>
  </tr>
  <tr>
    <td>Double-Opt-in</td>
    <td>Eine Akquise-Methode, bei der ein potenzieller Abonnent seine Zustimmung zum Hinzufügen zu einer Abonnement-Liste mit einem Antwortbefehl wie „Y“ oder seiner Postleitzahl bestätigen muss. Die Verwendung einer doppelten Opt-in-Eingabeaufforderung kann Ihnen bei der Einhaltung der bundesstaatlichen und bundesstaatlichen Richtlinien für Textnachrichten helfen.</td>
  </tr>
  <tr>
    <td>Ereignis</td>
    <td>Ein Ereignis ist ein definiertes Ereignis, das an die Vibes-Plattform gesendet und für Trigger-API-ausgelöste Aktionen, einschließlich Nachrichtensendungen, verwendet werden kann. Jedes Ereignis enthält ereignisspezifische Daten, einschließlich event_type , mit denen bestimmt wird, welcher API-ausgelösten Nachrichtenkampagne es entspricht. Die Ereignis-API kann über einen Webhook in Marketo Engage ausgelöst werden. Weitere Informationen finden Sie in unserer <a href="https://developer-platform.vibes.com/reference/event-api">Ereignis-API-</a>.</td>
  </tr>
  <tr>
    <td>Keyword</td>
    <td>Ein kurzes Wort oder eine alphanumerische Zeichenfolge, die vom Kunden an die Kurzwahlnummer gesendet wird, um ein mobiles Erlebnis zu initiieren.</td>
  </tr>
  <tr>
    <td>Long Code (10DLC)</td>
    <td>Eine Absender-ID, von der aus bidirektionale Nachrichten zwischen der Marke und dem Verbraucher gesendet werden. US-Langcodes sind 10 numerische Ziffern.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Mobiltelefonnummer oder die Telefonnummer einer Person. MDN- und Mobiltelefonnummern sind in Marketo keine eindeutigen Kennungen.</td>
  </tr>
  <tr>
    <td>Mobile-Datenbank</td>
    <td>Die Mobile-Datenbank ist die Datenbank, in der die Abonnentendaten von Vibes gespeichert werden. Jeder Abonnent verfügt über einen eindeutigen „Personendatensatz“, in dem die Mobilfunknummer und alle zugehörigen benutzerdefinierten Felder ausgefüllt sind.</td>
  </tr>
  <tr>
    <td>Teilnehmer/in</td>
    <td>Eine Person, die über eine oder mehrere mobile Interaktionen (z. B. das Senden einer Textnachricht) mit Ihrem mobilen Programm verfügt, sich jedoch nicht für eine Abonnement-Liste angemeldet hat.</td>
  </tr>
  <tr>
    <td>Personendatensatz</td>
    <td>Ein Personendatensatz ist eine Sammlung von Daten für eine bestimmte Mobiltelefonnummer. Jedem Personendatensatz wird außerdem ein eindeutiger Personenschlüssel zur Identifizierung zugewiesen. Marketo-IDs werden über das Feld external_person_id mit Vibes verknüpft. Weitere Informationen zu Personendatensätzen finden Sie in der <a href="https://developer-platform.vibes.com/reference/person-api">Dokumentation zur Personen-API</a>.</td>
  </tr>
  <tr>
    <td>Kurzwahlnummer</td>
    <td>Eine Absender-ID, von der aus bidirektionale Nachrichten zwischen der Marke und dem Verbraucher gesendet werden. US-Kurzwahlnummern sind 5-6 numerische Ziffern. Kanadische Kurzwahlnummern sind 4-6 numerische Ziffern. Die Marketo LaunchPoint-Integration in Vibes unterstützt eine Kurzwahlnummer pro Instanz.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Short Message Service. Dies ist eine Nachricht, die nur Text enthält.</td>
  </tr>
  <tr>
    <td>Abonnement-Listen</td>
    <td>Eine Liste der Mobilfunknummern (und der zugehörigen Personendatensätze), die dem Empfang wiederkehrender Nachrichten von Ihrem Programm zugestimmt haben.</td>
  </tr>
  <tr>
    <td>Abonnent</td>
    <td>Eine Mobiltelefonnummer, die von einer oder mehreren Abonnement-Listen abonniert wurde.</td>
  </tr>
  <tr>
    <td>Vibes-Plattform</td>
    <td>Die Website, bei der Sie sich anmelden, um Ihre Kampagnen zu verwalten. Wechseln Sie zu <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a>, um auf die Vibes-Plattform zuzugreifen.</td>
  </tr>
</tbody>
</table>
