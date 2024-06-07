---
unique-page-id: 4719093
description: Web-Segmente - Marketo-Dokumente - Produktdokumentation
title: Websegmente
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 5%

---

# Websegmente {#web-segments}

## Segment anzeigen {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

Auf der Registerkarte Segmente werden alle benutzerdefinierten definierten Segmente angezeigt, die Sie basierend auf verschiedenen Attributen einrichten.  **Ein Segment ist eine Sammlung von Besuchern, die die auf der Seite &quot;Segment festlegen&quot;definierten Kriterien erfüllen.**  Ein Segment kann Besucher aus einer bestimmten Branche, einem bestimmten Ort oder basierend auf der Onsite-Aktivität des Besuchers sein.

Bei der Web-Personalisierung kann ein Besucher mehr als einem Segment zuordnen. Wenn es beispielsweise ein Segment für Besucher aus den USA und ein Segment für Finanzunternehmen gibt, würde ein Webbesucher aus der Bank of America **both** das Segment für US-Besucher und das Segment für Finanzunternehmen.

**GRAPH:**  Auf der Seite Segmente wird ein Balkendiagramm der ausgewählten Segmente angezeigt, das der Anzahl der Besucher aus dem Segment (Y-Achse) und dem Segmentnamen (X-Achse) entspricht.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Name</th> 
   <th colspan="1" rowspan="1">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Name</strong></td> 
   <td colspan="1" rowspan="1">Der Titel des Segments</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Abgleiche</strong></p></td> 
   <td colspan="1" rowspan="1">Die Anzahl der Besucher, die die benutzerdefinierten, definierten Kriterien des Segments erfüllen</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Kampagne einstellen</strong></td> 
   <td colspan="1" rowspan="1">Ermöglicht die Einrichtung eines Campaign CTA, der dem ausgewählten Suchbegriff zugeordnet ist</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Besucher</strong></td> 
   <td colspan="1">Vorschau der mit dem ausgewählten Suchbegriff verknüpften Besuchertabelle</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Clickstream</strong></td> 
   <td colspan="1" rowspan="1">Zeigt eine Tabelle der Besucheraktivität und des URL-Pfads auf der Site sowie die Dauer des Besuchs auf den einzelnen Seiten an </td> 
  </tr> 
 </tbody> 
</table>

Siehe [Erstellen und Anzeigen von Segmentbeschriftungen](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segmente - Rechtses Bedienfeld**

![](assets/image2014-11-12-10-3a46-3a32.png)

Wenn Sie ein Segment in der Tabelle auswählen, werden im rechten Bereich zusätzliche Details zum Segment angezeigt.

Zu diesen Details gehören:

* Name des Segments
* Erstellungsdatum des Segments
* Die zugehörigen Kampagnen, die die mit dem Segment betriebenen Kampagnen anzeigen. Durch Klicken auf die Anzahl der Reaktionen gelangen Sie zur Kampagnenseite, auf der der Kampagnen-CTA (Aktionsaufruf) für das Segment angezeigt wird.
* Die Anzahl der Übereinstimmungen (Anzahl der Besucher, die die Segmentkriterien erfüllten) für das Segment und die Anzahl der eindeutigen (individuellen) Besucher, die mit dem Segment übereinstimmten. Wenn Sie auf den Link &quot;Unique Visitor&quot;klicken, werden Sie zur Seite des Besuchers geleitet, auf der die Ergebnisse des Segments angezeigt werden.
* Der Inhaber/Benutzer, der das Segment erstellt
* Die mit dem Segment verbundenen Domänen
* Eine kurze Zusammenfassung der ausgewählten Kriterien des Segments

## Aktivieren oder Deaktivieren eines Segments {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Um ein Segment zu aktivieren oder zu deaktivieren, aktivieren Sie das Kontrollkästchen dieses Segments in der Tabelle und wählen Sie in der Dropdown-Liste &quot;Aktion auswählen&quot;unten in der Tabelle die Aktion &quot;Aktivieren&quot;oder &quot;Deaktivieren&quot;aus. Wenn ein Segment deaktiviert ist, wird unter der Spalte Status das Wort &quot;Deaktivieren&quot;angezeigt.

## Segmente erstellen {#create-segments}

Das erstellte Segment erfüllt alle spezifischen Kriterien, die Sie im **Segment festlegen** Seite. Sie können Ihre Segmente auch basierend auf einer Kombination von Kriterien anpassen und eine bestimmte Zielgruppe in Ihrer Kampagne auswählen.

So erstellen Sie ein neues Segment

Aus dem **Segmente** Seite, klicken **Neu erstellen** unter dem Diagramm. Der folgende Bildschirm wird angezeigt.

![](assets/four.png)

Definieren Sie allgemeine Parameter für Ihr Segment:

* **Name:**  Benennen Sie Ihr Segment.
* **Beschreibung:**  Stellen Sie eine detailliertere Erläuterung der Segmentkriterien bereit.
* **Domänen:**  Wählen Sie die Domänen aus, die Sie in das Segment einbeziehen möchten.
* **Segmentregellogik:**  Wählen Sie eine UND/ODER-Logik aus, um jedes Segmentierungsattribut zu erstellen.
* **Zeit:** Definieren Sie den Grad der Besucherinteraktion, den Sie in Ihrer Kampagne wünschen.

   * **Bei Eintritt**: Interagieren Sie vom Besucher auf die Website.
   * **Nach dem 1. bis 9. Klick**: Besucherinteraktion nach einer bestimmten Anzahl von Klicks auf die Website

>[!TIP]
>
>**Segment Rule Logic**
>
>Es gibt drei Filteroptionen:
>
>1. Alle Filter verwenden (1 und 2 und 3...)
>1. Verwenden Sie beliebige Filter (1, 2 oder 3...)
>1. Erweiterte Filter (mit - und / oder -Ausdrücken)
>
>    Mithilfe erweiterter Filter können Sie die Segmentbedingung steuern. Geben Sie die Filternummern getrennt durch „und“ und „oder“ ein.
>
>    * 1 und 2 und 3
>    * 1 oder 2 oder 3
>
>    Beim Kombinieren von „und“ und „oder“ sind Klammern erforderlich, um die Logik zu klären. beispielsweise muss &quot;1 oder 2 und 3&quot; wie folgt geschrieben werden:
>
>    * 1 und (2 oder 3)
>    * (1 und 2) oder 3
>
>    Für eine kompliziertere Logik sind auch verschachtelte Klammern erlaubt, z. B. 
>
>    * (1 und 2) oder (3 und 4)
>    * 1 und (2 oder (3 und 4))
>
>    Überprüfen Sie nach jedem Einfügen, Löschen oder Neuordnen Ihre Logik.

Ziehen Sie Segmentattribute aus der rechten Spalte in den Segmenteditor auf der linken Seite:

![](assets/five.png)

### Firmenbezogene Daten {#firmographics}

**Standort**

Drag &amp; Drop **Standort** in den Segmenteditor.

* Wählen Sie aus den folgenden Parametern aus:

   * **Einschließen** - Wählen Sie aus, ob die Kampagne einen Ort einschließen oder ausschließen soll.
   * **Land auswählen zum Hinzufügen** - Wählen Sie aus der Dropdown-Liste das Land aus, das Sie in das Segment aufnehmen möchten. Der Ländername wird rechts angezeigt. Sie können mehrere Länder auswählen.

Nachdem das Land hinzugefügt wurde, können Sie auch das Bundesland, die Stadt und die Postleitzahl des Segments angeben.

* **Bundesland oder Provinz zum Hinzufügen auswählen** - Wählen Sie aus der Dropdown-Liste den US-Bundesstaat oder die kanadische Provinz aus, die Sie einbeziehen möchten. Sie können mehrere Auswahlen vornehmen.
* **Postleitzahl** - Geben Sie die Postleitzahl ein, die Sie in Ihr Segment aufnehmen möchten.
* **Städte** - Geben Sie die Stadt(en) ein, die Sie einbeziehen möchten. Verwenden Sie ein Semikolon zwischen Städten.

>[!TIP]
>
>**Welche Segmentbedingungen wähle ich aus? &quot;AND&quot;oder &quot;OR&quot;?** OR fungiert in jedem Feld als zusätzliche Option. Die Aussichten müssen nur ein Kriterium aus mehreren Kriterien erfüllen, die in jedem Feld ausgewählt wurden, um für das Segment qualifiziert zu sein. (Zum Beispiel können potenzielle Kunden aus den USA kommen. *oder* von der Verteidigungsindustrie). UND fungiert als zusätzlicher obligatorischer Parameter, der für dieses Segment erfüllt werden muss. (Zum Beispiel müssen die Aussichten sowohl aus den USA als auch aus der Verteidigungsindustrie stammen.) In jedem Segmentierungsprofil kann jedes separate Feld je nach ausgewählter Segmentbedingung entweder als &quot;AND&quot;oder als &quot;OR&quot;funktionieren.

**Branchen** Unter dem **Profilsegmentierung** -Abschnitt, aktivieren Sie das Kontrollkästchen neben **Branche**.

* Wählen Sie aus den folgenden Parametern aus:

   * **Enthält** - Wählen Sie aus, ob das Segment eine Branche einschließen oder ausschließen soll.
   * **Zu hinzugefügte Branchen auswählen** - Wählen Sie die Branche aus, die Sie in das Segment aufnehmen möchten. Die Branche wird unter dem Dropdown-Feld angezeigt. Sie können mehrere Branchen auswählen.

**Organisationsgruppe**

Unter dem **Profilsegmentierung** -Abschnitt, aktivieren Sie das Kontrollkästchen neben **Organisationsgruppe.**

* Wählen Sie aus der Dropdown-Liste eine der folgenden Optionen aus:

   * Fortune 500 - Enthält nur Fortune 500-Unternehmen in diesem Segment
   * Fortune 1000 - Enthält nur Fortune 1000-Unternehmen in diesem Segment
   * Global 2000 - Einbeziehung der Global 2000-Unternehmen in dieses Segment
   * Unternehmen - Umfasst Organisationen mit mehr als 1.000 Mitarbeitern und einem Umsatz von mehr als 250 Mio. USD
   * KMU - Schließt nur kleine und mittlere Unternehmen in dieses Segment ein

**-Named Accounts-**

**Organisationen**

* **stammt von diesen Unternehmen (spezifische Namen)**

   * Wählen Sie aus der Dropdown-Liste &quot;Unternehmen zum Hinzufügen auswählen&quot;das Unternehmen aus, das als Ziel ausgewählt werden soll.
   * Sie können den genauen Organisationsnamen eingeben, den Sie als Ziel auswählen möchten. *Es ist _always_ Es wird empfohlen, Named Account Lists zu verwenden, anstatt die Namen manuell für bessere Übereinstimmungen einzugeben (siehe unten).

**Liste benannter Konten**

Wählen Sie aus einer [Liste benannter Konten](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) , um wichtige Zielgruppenkonten zu segmentieren.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>Die Zahl in den Klammern neben dem Namen der Liste &quot;Spezifisches Konto&quot;wird als Indexreferenz für die Liste für die Web-Personalisierung verwendet [API lesen](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization).

**ISP ausschließen**

Schließt Internet Service Provider (ISPs) aus dem Segment aus.

### Bekannte Personen {#known-people}

**Datenbank**

Die Web-Personalisierung wird in Ihre Marketo-Datenbank integriert, sodass Sie Kampagnen nach bekannten Personalattributen und Daten segmentieren und personalisieren können.

Wählen Sie Datenbank und danach ein Personendatenfeld aus der Dropdown-Liste aus. Wählen Sie die **+** , um Felder aus der Dropdown-Liste hinzuzufügen.

![](assets/seven.png)

Sie können Personendatenfelder über Kontoeinstellungen > Datenbank hinzufügen oder entfernen.

>[!TIP]
>
>Erstellen Sie Ihre Segmentkriterien gemäß allen Personendatenfeldern von Marketo-Mitarbeitern, z. B. Titel, Punktzahl, Rolle usw.
>
>Z. B. &quot;Job Title equals CMO&quot;und &quot;Score ist kleiner oder gleich 50&quot;

**Marketo Email Campaign** Segmentieren und personalisieren Sie Kampagnen per E-Mail-Verweis von einem Besucher, der auf eine Marketo-E-Mail klickt und auf die Site gelangt. Segmentieren Sie nach Marketo-Programmname oder Kampagnenname und fahren Sie mit der Konversation von E-Mail zu Web fort. Wählen Sie + aus, um Felder aus der Dropdown-Liste hinzuzufügen.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Status**

Definieren Sie Ihr Segment entsprechend dem Status eines Interessenten: bekannt oder anonym.

* Bekannt - Wählen Sie diese Option aus dem Dropdownfeld für bekannte Besucher aus. Ein Besucher ist bekannt, wenn er ein Formular auf Ihrer Website sendet und auf der Web Personalization People -Seite erscheint.
* Anonym - Wählen Sie diese Option aus dem Dropdownfeld für anonyme Besucher aus.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Verhaltens- {#behavioral}

**Besuche -** Definieren Sie Ihr Segment entsprechend dem Besucherverhalten oder der Identifizierung.

* Anzahl der Besuche - Wählen Sie diese Option aus dem Dropdown-Feld aus, um die Anzahl der Besuche für Interessenten auf der Website anzugeben.

   * Wählen Sie Gleich, Gleich oder Größer als oder Gleich oder Kleiner als aus dem Dropdownfeld aus.

* Spezifische Besuche - Wählen Sie diese Option aus dem Dropdownfeld aus, um einen bestimmten Besucher anzugeben.

   * Geben Sie im Textfeld auf der rechten Seite die Besuchernummer ein, die Sie verfolgen möchten. Die eindeutige Web-Personalisierung-Besucher-Identifikationsnummer finden Sie beim Klicken auf einen Besucher (auf der Besucherseite) und die Set Campaign -Funktion auf der rechten Seite. Die Besucher-ID befindet sich im Abschnitt Erweiterte Einstellungen . Die Besucher-ID finden Sie auch in der URL (z. B. VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Suchbegriffe** - Definieren Sie ein Segment entsprechend den Suchbegriffen eines Interessenten.

* Der gesuchte Besucher - Wählen Sie aus der Dropdownliste die Begriffe, die Sie verfolgen möchten, aus der Suche Ihrer Besucher aus oder fügen Sie Ihre eigenen Suchbegriffe hinzu. (Die &#42; Platzhalter für Suchbegriffe, da er als Standard festgelegt ist, um Suchbegriffe einzubeziehen, die den Suchbegriff enthalten).

**Verweise** - Fügen Sie URLs hinzu, auf die der Besucher verwiesen wurde.

* Verweise auswählen, die hinzugefügt werden sollen - Wählen Sie aus der Dropdownliste die Verweisseiten aus, die Sie verfolgen möchten, oder fügen Sie Ihre eigenen Verweise hinzu. Nach der Auswahl werden die Verweise im Feld unten angezeigt. (Verwendung &#42; als Platzhalter erlaubt ist)

**Seiten einschließen** - Verfolgen Sie spezifische Seitenaussichten, die auf Ihrer Website besucht werden.

* URL-Übereinstimmungen - Fügen Sie die URL bestimmter Webseiten hinzu, die Sie verfolgen möchten. Sie können mehrere URLs hinzufügen, indem Sie sie durch Semikolon trennen. (Verwendung &#42; als Platzhalter erlaubt ist).

**Ausschließen von Seiten** - Schließen Sie bestimmte Seiten aus, die Sie im Segment nicht abgleichen möchten. (Verwendung &#42; als Platzhalter erlaubt ist).

* URL stimmt nicht überein - Fügen Sie die URL bestimmter Webseiten hinzu, die vom Tracking ausgeschlossen werden sollen. Sie können mehrere URLs hinzufügen, indem Sie sie durch ein Semikolon trennen

![](assets/segment-extra.png)

### Gerät / Browser {#device-browser}

**Mobilbetriebssystem**

Ziehen Sie das mobile Betriebssystem in den Segmenteditor.

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Besuchertyp**<br />
  **Mobilbetriebssystem** - Wählen Sie aus dem Dropdownfeld ein oder mehrere aufgelistete mobile Betriebssysteme aus. Das ausgewählte mobile Betriebssystem wird unten angezeigt.

   * Der Besucher verwendet ein beliebiges Mobilgerät
   * Der Besucher verwendet dieses spezifische Gerät/Betriebssystem.
   * Der Besucher verwendet kein Mobilgerät

* **Gerät**  - Wählen Sie aus der Dropdownliste ein oder mehrere Geräte (Apple, Samsung, LG, HTC, Nexus, Blackberry usw.) aus. Die ausgewählten Geräte werden unten angezeigt.

**Browser**

Targeting von Besuchern, die bestimmte Browsertypen und/oder Versionen verwenden.

* Browsertyp - Wählen Sie aus dem Dropdownfeld einen oder mehrere Internet-Browser aus. Die ausgewählten Browser werden unten angezeigt.
* Browserversion - Geben Sie die Browser-Version ein, die Sie zum Segment hinzufügen möchten. Sie können mehrere Versionen auswählen, indem Sie jede durch ein Komma trennen. (Verwendung &#42; als Platzhalter erlaubt ist).

### API {#api}

**Datenereignisse** - Segmentieren von Besuchern, die bestimmte benutzerspezifische Datenereignisse Trigger haben

Fügen Sie den Ereigniswert hinzu, den Sie als Ziel auswählen möchten. z. B. aus Datenquellen von Dritten.

**Benutzerkontext-API**

Web Personalization-API-Aufruf  [Weitere Informationen dazu finden Sie hier .](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**Verwenden von Platzhaltern:** Wenn Sie Suchbegriffe oder URLs einbeziehen möchten, die etwas darin enthalten, d. h. &quot;[google.com](https://google.com)&quot; oder &quot;Suchbegriff Produkt&quot;, nennen wir dies einen Platzhalter und es sollte mit einem Sternchen eingegeben werden - dieser kleine Kerl&#42; - auf jeder Seite. Also alles, was aus [google.com](https://google.com) sollte als &#42; [google.com](https://google.com)&#42;

## Segmente bearbeiten {#edit-segments}

Sie können ein Segment bearbeiten, das erstellt wurde.

1. Um ein Segment zu bearbeiten, navigieren Sie zu **Segmente**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Im **Segmente** auf das Bearbeitungssymbol ( ![](assets/segment-edit.png)) des Segments, das Sie bearbeiten möchten. Die **Segment festlegen** Seite mit dem ausgewählten Segment geöffnet.
1. Wenden Sie alle Änderungen an, die Sie am Segment vornehmen möchten.
1. Klicken Sie auf **Speichern**.

## Segmente löschen {#delete-segments}

Sie können von Ihnen erstellte Segmente löschen.

1. Aus dem **Segmente** -Seite ein Segment auswählen.
1. Klicken Sie auf das Löschsymbol ( ![](assets/segment-delete.png) ) des Segments, das Sie löschen möchten.
1. Eine Bestätigungsmeldung wird angezeigt, die bestätigt, dass Sie im Begriff sind, die **Segment**.

>[!NOTE]
>
Ein Segment, das einer Kampagne zugeordnet ist, kann nicht gelöscht werden. Löschen Sie zunächst die Kampagne und dann das Segment.

Sehr gut! Nachdem Sie nun den Abschnitt Segmente verstanden haben, sollten wir uns mit Kampagnen vertraut machen.

>[!MORELIKETHIS]
>
* [Erstellen eines einfachen Websegments](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
* [Erstellen einer neuen Web-Kampagne für Dialogfelder](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Erstellen einer neuen Web-Kampagne in Zone](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Erstellen einer neuen Widget-Webkampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
