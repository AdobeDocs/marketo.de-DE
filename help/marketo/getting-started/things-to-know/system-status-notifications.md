---
description: Abonnieren von Systemstatusbenachrichtigungen - Marketo Engage-Dokumente - Produktdokumentation
title: Abonnieren von Systemstatusbenachrichtigungen
feature: Getting Started
hide: true
hidefromtoc: true
source-git-commit: cf60167b9e9ee2ea2a2861a3cd3c661781dbf0b0
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Abonnieren von Systemstatusbenachrichtigungen {#subscribe-to-system-status-notifications}

EINFÜHRUNGSTEXT

>[!PREREQUISITES]
>
>Bevor Sie ein Abonnement erstellen können, müssen Sie zunächst ermitteln, in welchem Rechenzentrum und welchem Pod/Server sich Ihr Abonnement befindet.

## Identifizieren des Rechenzentrums {#identify}

+++Identifizieren von Rechenzentrum und Pod/Server

1. Klicken Sie im **Admin** von Marketo Engage auf **Mein Konto**.

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. Scrollen Sie nach unten zu _Support-Informationen_.

   ![](assets/subscribe-to-system-status-notifications-2.png)

Im Feld _Rechenzentrum_ sind die Buchstaben das Rechenzentrum und die Zahlen der Pod. Im obigen Beispiel befindet sich der Benutzer in unserem Ashburn-Rechenzentrum auf Pod 49.

In Schritt 7 von [Abonnement erstellen](#create-a-subscription) wählt dieser Benutzer den regionalen Speicherort **Marketo Ashburn** und Pod **ab49**.

<table style="width:225px;">
  <tr>
    <th colspan="2">Abkürzungen für Rechenzentren</th>
  </tr>
  <tr>
    <td style="width:25%;">AB</td>
    <td>aschbrennen</td>
  </tr>
  <tr>
    <td style="width:25%;">SJ</td>
    <td>San Jose</td>
  </tr>
  <tr>
    <td style="width:25%;">Sn</td>
    <td>Sydney</td>
  </tr>
  <tr>
    <td style="width:25%;">Lon</td>
    <td>London</td>
  </tr>
  <tr>
    <td style="width:25%;">NLD</td>
    <td>Amsterdam</td>
  </tr>
</table>

>[!TIP]
>
>Mit dieser Methode kann auch ermittelt werden, in welchem Real-Time Personalization (RTP)-Pod/Server sich Ihr Abonnement befindet.

+++

## Abonnement erstellen {#create-a-subscription}

Nachdem Sie [Ihr Rechenzentrum und Ihren Pod/Server identifiziert](#identify), führen Sie die folgenden Schritte aus, um ein Abonnement zu erstellen.

1. Klicken Sie auf [status.adobe.com](https://status.adobe.com/de) auf **Abonnements verwalten**.

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. Melden Sie sich mit Ihren Adobe-Anmeldeinformationen an (falls noch nicht geschehen) oder klicken Sie auf **Konto erstellen** falls noch kein Konto vorhanden ist.

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. Klicken Sie auf der Registerkarte _Produktbeschreibungen_ auf **Abonnements erstellen**.

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. Klicken Sie auf das ![Pluszeichen](assets/icon-plus-sign.png)-Symbol neben _Experience Cloud_, um das Menü zu erweitern. Tun Sie dasselbe für _Adobe Marketo Engage_.

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800" zoomable="yes"}

1. Wählen Sie die gewünschten Produktangebote/Services aus, zu denen Sie Benachrichtigungen erhalten möchten, und klicken Sie auf **Weiter**.

   >[!TIP]
   >
   >Aktivieren Sie _Adobe Marketo Engage_, um alle auszuwählen.

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800" zoomable="yes"}

1. Auswählen der gewünschten Ereignistypen.

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:600px;">
   <tr>
   <td style="width:30%;"><b>Hauptdienstproblem</b></td>
   <td>Nicht verfügbare Services oder erhebliche Leistungseinbußen für mehrere Benutzer von Produktionssystemen.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Geringfügiger Service-Fehler</b></td>
   <td>Partielle Dienstausfälle oder mäßige Leistungseinbußen für mehrere Benutzer auf Produktionssystemen.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Wartungsdienst</b></td>
   <td>Text</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Ankündigungen</b></td>
   <td>Ankündigungen zu…</td>
   </tr>
   </table>

1. Wählen Sie die gewünschte regionale Position und Umgebung aus. Klicken Sie auf **Fortfahren**.

   ![](assets/subscribe-to-system-status-notifications-9.png){width="800" zoomable="yes"}

1. Wählen Sie Ihre Abonnementvoreinstellung (E **Mail** oder **Slack** und klicken Sie auf **Weiter**.

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. Überprüfen Sie Ihre Auswahl und klicken Sie auf **Voreinstellungen bestätigen**.

   ![](assets/subscribe-to-system-status-notifications-11.png)
