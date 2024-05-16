---
description: Benutzer- und Lizenzverwaltung - Marketo-Dokumente - Produktdokumentation
title: Benutzer- und Lizenzverwaltung
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 0ab3b8075923f58a9546acff8039d67126f22bf3
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 2%

---

# Benutzer- und Lizenzverwaltung {#user-and-license-management}

Erfahren Sie, wie Sie Benutzer hinzufügen und entfernen sowie Ihre aktuellen Lizenzen anzeigen können.

## Hinzufügen von Benutzern {#add-a-user}

1. Navigieren Sie zu **Admin** Bereich.

   ![](assets/user-and-license-management-1.png)

1. Klicks **Interaktive Webinare**.

   ![](assets/user-and-license-management-2.png)

1. Klicks **Benutzer hinzufügen/entfernen**.

   ![](assets/user-and-license-management-3.png)

1. Klicken Sie auf das Dropdown-Menü Verfügbare Benutzer , wählen Sie die Benutzer aus, die Sie hinzufügen möchten, und klicken Sie auf **OK**.

   ![](assets/user-and-license-management-4.png)

## Entfernen von Benutzern {#remove-a-user}

1. Navigieren Sie zu **Admin** Bereich.

   ![](assets/user-and-license-management-5.png)

1. Klicks **Interaktive Webinare**.

   ![](assets/user-and-license-management-6.png)

1. Klicks **Benutzer hinzufügen/entfernen**.

   ![](assets/user-and-license-management-7.png)

1. Markieren Sie die Benutzer, die Sie entfernen möchten, und drücken Sie die Entf-Taste auf Ihrer Tastatur. Klicks **OK** wann geschehen.

   ![](assets/user-and-license-management-8.png)

## Lizenznutzung {#license-usage}

Interaktive Webinare bieten spezifische Lizenzen für die Erstellung von Veranstaltungen auf Basis von Adobe Connect. Jedes Mal, wenn eine Lizenz hinzugefügt wird, wird ein neues Feld zur Lizenzverwendung angezeigt. Marketo-Administratoren können die Lizenzen anzeigen (nicht bearbeiten), indem sie die folgenden Schritte ausführen. Wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer), um zusätzliche Lizenzen zu erhalten.

1. Navigieren Sie zu **Admin** Bereich.

   ![](assets/user-and-license-management-9.png)

1. Klicks **Interaktive Webinare**.

   ![](assets/user-and-license-management-10.png)

1. Scrollen Sie nach unten zu den Karten für die Lizenznutzung .

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr>
   <td width="20%"><b>Startdatum</b></td>
   <td width="80%">Datum, an dem die Lizenz beginnt</td>
  </tr>
  <tr> 
   <td width="20%"><b>Ablaufdatum</b></td>
   <td width="80%">Datum, an dem die Lizenz abläuft.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Typ</b></td>
   <td width="80%">Die Art der erworbenen Lizenz. Es stehen drei Typen zur Verfügung: Shared Events License, Shared Rooms License, Additional Storage License.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Veranstaltungskapazität</b></td>
   <td width="80%">Die maximale Anzahl der Teilnehmer, die für eine Veranstaltung geeignet sind.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Veranstaltungen insgesamt</b></td>
   <td width="80%">Die Gesamtzahl der Ereignisse, die mit dieser Lizenz bereitgestellt wurden.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Verbrauchte Ereignisse</b></td>
   <td width="80%">Die Gesamtzahl der abgeschlossenen Ereignisse.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Speicherkapazität</b></td>
   <td width="80%">Speichermenge, die zum Speichern von Aufzeichnungen, Collaterals, hero images, Dokumentationen und anderen Assets verfügbar ist.</td>
  </tr>
  </tbody>
</table>

**Zu beachten**

* Der Typ &quot;Zusätzliche Speicherlizenz&quot;liefert nur Speicher, daher der Wert in jedem Feld _beats_ Die Speicherkapazität wird einfach als &quot;-&quot;aufgeführt.

* Der Typ &quot;Shared Room License&quot; hat unbegrenzte Ereignisse und &quot;Additional Storage License&quot; stellt nur Speicher bereit, daher wird das Feld Total Events für diese Lizenzen einfach als &quot;-&quot;aufgeführt.

* Jedes Mal, wenn ein Ereignis erstellt wird, zählt es von seiner jeweiligen Lizenz aus als &quot;konsumiert&quot;(es sei denn, es handelt sich um eine Shared Room-Lizenz). Die &quot;Lizenz für freigegebene Ereignisse&quot;erhält Vorrang, wenn sowohl &quot;Lizenz für freigegebene Ereignisse&quot;als auch &quot;Lizenz für freigegebene Ereignisse&quot;mit derselben Kapazität vorhanden sind. Wenn das Ereignis nicht bereitgestellt wurde und das Ereignisprogramm vor der geplanten Zeit gelöscht wird, wird die Ereignisanzahl erneut aufgefüllt, indem ein Ereignis von &quot;Entnommen&quot;abgezogen wird.

* Sobald eine Lizenz erschöpft ist, bleibt ihre Kachel auf dem Bildschirm der interaktiven Webinare im Admin-Bereich mit dem Wert &quot;Gesamtereignisse&quot;und &quot;Entsuchte Ereignisse&quot;erhalten. Erst wenn die Lizenz abläuft, wird sie vom Bildschirm entfernt.

## Benutzerzugang {#user-access}

Interaktive Webinare bieten die Möglichkeit, die Nutzung zu regulieren, indem sie Marketo Engage-Benutzern Berechtigungen zum Erstellen und Bereitstellen interaktiver Webinare erteilen. Ein Benutzer mit interaktiven Webinaren (oder Benutzer ohne diese Funktion) kann jedoch weiterhin Lese-/Bearbeitungsrechte für von anderen Benutzern erstellte interaktive Webinare-Ereignisprogramme haben.

Marketo-Benutzer, denen interaktive Webinare zugewiesen wurden und die Inhaber eines bestimmten Interaktiven Webinar-Veranstaltungsprogramms sind, können alle mit diesem Programm verbundenen interaktiven Webinar-Funktionen ausführen. Dazu gehören das Erstellen, Zugreifen auf, Ändern, Klonen, Verschieben und Löschen dieses Programms. Sobald dieser Benutzer jedoch kein interaktiver Webinar-Benutzer mehr ist, kann der Programmeigentümer auf das Programm zugreifen und es verschieben, jedoch keine anderen Funktionen ausführen.

Marketo-Benutzer, denen interaktive Webinare Berechtigungen erteilt wurden und die _not_ Inhaber eines bestimmten Interaktiven Webinars Event Program können begrenzte Funktionen für diese Programme ausführen. Nicht-Admin-Benutzer von Marketo können auf das Programm zugreifen und es klonen, können jedoch keine anderen Funktionen ausführen, wenn sie über Berechtigungen für interaktive Webinare verfügen. Marketo Admin-Benutzer _will_ Sie können alle Funktionen ausführen, z. B. auf das Programm zugreifen, es ändern, klonen, verschieben und löschen (sofern sie über Berechtigungen für interaktive Webinare verfügen). Wenn diese Berechtigung für Marketo-Administratoren und Benutzer ohne Administratorrechte widerrufen wird, können sie nur auf das interaktive Webinar-Veranstaltungsprogramm zugreifen und keine anderen Funktionen ausführen.

Die Einschränkung von umsetzbaren Funktionen wird durch eine ausgegraute Aktionsschaltfläche und eine Hover-Meldung angezeigt. Einige Beispiele für die ausgegrauten Aktionsschaltflächen sind &quot;Webinar entwerfen&quot;oder &quot;Webinar eingeben&quot;. Bei nicht ausführbaren Funktionen wird eine Meldung mit den Einschränkungen angezeigt. Siehe Beispiel unten:

![](assets/user-and-license-management-12.png)
