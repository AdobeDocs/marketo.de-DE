---
description: Benutzer- und Lizenzverwaltung - Marketo-Dokumente - Produktdokumentation
title: Benutzer- und Lizenzverwaltung
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: fe167b4a70a23f129d56ed20ac6c1ed1130049ef
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 2%

---

# Benutzer- und Lizenzverwaltung {#user-and-license-management}

Erfahren Sie, wie Sie Benutzer hinzufügen und entfernen und Ihre aktuellen Lizenzen anzeigen können.

## Benutzer hinzufügen {#add-a-user}

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/user-and-license-management-1.png)

1. Klicken Sie **Interaktive Webinare**.

   ![](assets/user-and-license-management-2.png)

1. Klicken Sie **Benutzer hinzufügen/**.

   ![](assets/user-and-license-management-3.png)

1. Klicken Sie auf die Dropdown-Liste Verfügbare Benutzer , wählen Sie die Benutzer aus, die Sie hinzufügen möchten, und klicken Sie auf **OK**.

   ![](assets/user-and-license-management-4.png)

## Benutzer entfernen {#remove-a-user}

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/user-and-license-management-5.png)

1. Klicken Sie **Interaktive Webinare**.

   ![](assets/user-and-license-management-6.png)

1. Klicken Sie **Benutzer hinzufügen/**.

   ![](assets/user-and-license-management-7.png)

1. Markieren Sie die zu entfernenden Benutzer und drücken Sie die Entf-Taste auf der Tastatur. Klicken **abschließend** OK“.

   ![](assets/user-and-license-management-8.png)

## Lizenznutzung {#license-usage}

Interaktive Webinare bieten spezielle Lizenzen zum Erstellen von Ereignissen, die von Adobe Connect unterstützt werden. Jedes Mal, wenn eine Lizenz hinzugefügt wird, wird ein neues Lizenznutzungsfeld angezeigt. Marketo-Administratoren bzw. -Administratorinnen können die Lizenzen anzeigen (nicht bearbeiten), indem sie die folgenden Schritte ausführen. Wenden Sie sich an das Adobe Account Team (Ihren Account Manager), um zusätzliche Lizenzen zu erhalten.

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/user-and-license-management-9.png)

1. Klicken Sie **Interaktive Webinare**.

   ![](assets/user-and-license-management-10.png)

1. Scrollen Sie nach unten zu den Lizenznutzungskarten.

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>Startdatum</b></td>
   <td width="80%">Datum, an dem die Lizenz beginnt.</td>
  </tr>
  <tr>
   <td width="20%"><b>Ablaufdatum</b></td>
   <td width="80%">Datum, an dem die Lizenz abläuft.</td>
  </tr>
  <tr>
   <td width="20%"><b>Typ</b></td>
   <td width="80%">Der Typ der erworbenen Lizenz. Es stehen drei Typen zur Verfügung: Shared Events License, Shared Rooms License, Additional Storage License.</td>
  </tr>
  <tr>
   <td width="20%"><b>Veranstaltungskapazität</b></td>
   <td width="80%">Die maximale Anzahl von Teilnehmern, die in einer Veranstaltung untergebracht werden können.</td>
  </tr>
  <tr>
   <td width="20%"><b>Veranstaltungen insgesamt</b></td>
   <td width="80%">Die Gesamtzahl der Ereignisse, die mit dieser Lizenz bereitgestellt wurden.</td>
  </tr>
  <tr>
   <td width="20%"><b>Verbrauchte Ereignisse</b></td>
   <td width="80%">Alle abgeschlossenen und aktuell geplanten Events. <a href="#things-to-note">Weitere Informationen</a></td>
  </tr>
  <tr>
   <td width="20%"><b>Speicherkapazität</b></td>
   <td width="80%">Speichermenge, die für die Speicherung von Aufzeichnungen, Begleitmaterial, Hero-Bildern, Dokumentation und anderen Assets verfügbar ist.</td>
  </tr>
  </tbody>
</table>

### Zu beachtende Punkte {#things-to-note}

* Jedes Mal, wenn ein Ereignis erstellt wird, zählt es als „genutzt“ aus der jeweiligen Lizenz (es sei denn, es handelt sich um eine Shared Room-Lizenz). „Shared Event License“ wird bevorzugt, wenn sowohl „Shared Event License“ als auch „Shared Room License“ derselben Kapazität vorhanden sind. Wenn das Ereignis nicht zugestellt wurde und das Ereignisprogramm vor dem geplanten Zeitpunkt gelöscht wird, wird die Ereignisanzahl wieder aufgefüllt. Wenn das Ereignis nicht zugestellt wird und das Ereignisprogramm nicht vor dem geplanten Zeitpunkt gelöscht wird, wird das Ereignis nicht wieder aufgefüllt.

* Der Typ „Zusätzliche Speicherlizenz“ bietet nur Speicher, daher wird der Wert in jedem Feld _außer_ Speicherkapazität einfach als &quot;-&quot; aufgeführt.

* Der Typ „Shared Room License“ verfügt über unbegrenzte Ereignisse und „Additional Storage License“ bietet nur Speicher, sodass das Feld Gesamtereignisse für diese Lizenzen einfach als &quot;-&quot; aufgeführt wird.

* Sobald eine Lizenz erschöpft ist, bleibt ihre Kachel auf dem interaktiven Webinar-Bildschirm im Admin-Bereich mit dem gleichen Wert für „Gesamte Ereignisse“ und „Genutzte Ereignisse“. Nur wenn die Lizenz abläuft, wird sie vom Bildschirm entfernt.

## Benutzerzugang {#user-access}

Interaktive Webinare bieten die Möglichkeit, die Nutzung zu regulieren, indem sie Marketo Engage-Benutzern die Berechtigung erteilen, interaktive Webinare zu erstellen und bereitzustellen. Ein Benutzer eines interaktiven Webinars (oder ein Nicht-Benutzer) kann jedoch weiterhin Lese-/Bearbeitungszugriff auf Veranstaltungsprogramme für interaktive Webinare haben, die von anderen Benutzern erstellt wurden.

Marketo-Benutzende, denen Berechtigungen für interaktive Webinare erteilt wurden und die Inhaber eines bestimmten Veranstaltungsprogramms für interaktive Webinare sind, können alle Funktionen für interaktive Webinare im Zusammenhang mit diesem Programm ausführen. Dazu gehören: Erstellen, Zugreifen auf, Ändern, Klonen, Verschieben und Löschen dieses Programms. Sobald dieser Benutzer jedoch kein Benutzer des interaktiven Webinars mehr ist, kann der Besitzer des Programms auf das Programm zugreifen und es verschieben, jedoch keine anderen Funktionen ausführen.

Marketo-Benutzende, denen Berechtigungen für interaktive Webinare erteilt wurden und die _nicht_ Eigentümer eines bestimmten Veranstaltungsprogramms für interaktive Webinare sind, können mit diesen Programmen eingeschränkte Funktionen ausführen. Benutzende ohne Administratorrechte in Marketo können auf das Programm zugreifen und es klonen, aber keine anderen Funktionen ausführen, wenn sie über Berechtigungen für interaktive Webinare verfügen. Marketo-Admin _Benutzende können jedoch_ alle Funktionen ausführen, z. B. auf dieses Programm zugreifen, es ändern, klonen, verschieben und löschen (sofern sie über Berechtigungen für interaktive Webinare verfügen). Sobald diese Berechtigung für Benutzende ohne Administratorrechte in Marketo widerrufen wurde, können diese nur auf das Veranstaltungsprogramm für interaktive Webinare zugreifen und keine anderen Funktionen mehr ausführen.

Die Einschränkung der ausführbaren Funktionen würde durch eine ausgegraute Aktionsschaltfläche und eine Hover-Meldung angezeigt. Beispiele für die ausgegrauten Aktionsschaltflächen sind „Webinar gestalten“ oder „Webinar eingeben“. Für nicht ausführbare Funktionen würde eine Meldung mit den Einschränkungen bereitgestellt. Siehe Beispiel unten:

![](assets/user-and-license-management-12.png)
