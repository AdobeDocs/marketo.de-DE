---
description: Flow Step Service - Marketo Docs - Produktdokumentation
title: Flussschritt-Dienst
exl-id: 81367562-8b27-4ec5-8a9b-b02083a2e999
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 0%

---

# Flussschritt-Dienst {#flow-step-service}

Die Fluss-Schritte für Self-Service sind ein Framework und eine Reihe von Funktionen für die Erstellung, Veröffentlichung und Integration von Webdiensten in Smart-Kampagnen von Adobe Marketo Engage. Dieses Handbuch richtet sich an Marketo Engage-Endbenutzer, die Dienste installieren und verwenden möchten, die bereits erstellt und veröffentlicht wurden. Informationen zum Erstellen und Veröffentlichen Ihres eigenen Dienstes finden Sie im Abschnitt [GitHub-Repository für die Service Provider-Schnittstelle](https://github.com/adobe/Marketo-SSFS-Service-Provider-Interface){target="_blank"}. A Proof-of-Concept Lookup Table implementation may be found [here](https://github.com/adobe/mkto-flow-lookup){target="_blank"}.

## Onboarding und Verwalten von Diensten {#onboarding-and-managing-services}

Für die Installation eines benutzerdefinierten Flussschritts sind Administratorberechtigungen in Marketo erforderlich (**Webhooks verwalten** in der Version vom 21. Januar, Änderung in der Version vom 11. März). Abgesehen von der Installations-URL können alle anderen Aspekte eines Dienstes nach dem ersten Onboarding bearbeitet werden, indem Sie über das Raster &quot;Service Provider&quot;in den Detailbildschirm des Dienstes navigieren.

## Installations-URL {#installation-url}

Um mit der Installation zu beginnen, müssen Sie zunächst die URL des OpenAPI-Dokuments abrufen, das Ihren Dienst definiert. Ihr Dienstleister sollte in der Lage sein, dies Ihnen bereitzustellen, und wird normalerweise über eine URL verfügen, die auf `/openapi.json`. Vollständige URLs sehen in etwa wie folgt aus: `https://www.example.com/OpenAPI.json`. Sobald Sie über diese URL verfügen, wechseln Sie zum Menü &quot;Dienstanbieter&quot;in Ihrem Admin-Bereich.

Klicken **Nächste** , um zum Abschnitt Dienstanmeldeinformationen eingeben zu wechseln.

![](assets/flow-step-service-1.png)

## Dienstberechtigungen eingeben {#enter-service-credentials}

Um auf den installierten Dienst zugreifen zu können, muss Marketo über gültige API-Anmeldeinformationen verfügen. Diese Anmeldeinformationen sollten Sie von Ihrem Dienstleister erhalten. Dienste haben drei verschiedene Authentifizierungsoptionen, sodass möglicherweise eine von drei verschiedenen Eingabeaufforderungen zur Eingabe von Anmeldeinformationen angezeigt wird: **API-Schlüssel** , das nur ein Eingabefeld hat, **Grundlegende Authentifizierung** , für die ein Benutzername und ein Kennwort erforderlich sind und möglicherweise auch ein Feld mit dem Namen Realm erforderlich ist, und **OAuth2** mithilfe der _Client-Anmeldedaten_ einen _Client-ID_ und _Client Secret_.

Wenn Sie Ihre Anmeldeinformationen speichern, versucht Marketo, den Statusendpunkt des Dienstes aufzurufen, um zu überprüfen, ob sie gültig sind. Wenn die angegebenen Anmeldeinformationen ungültig sind, wird ein Fehler angezeigt, der dies angibt.

## Onboarding-Anleitung (optional) {#onboarding-guide}

Einige Dienstleister werden einen optionalen Schritt zur Onboarding-Anleitung enthalten. Dieser Schritt enthält alle zusätzlichen Anweisungen zum Abschluss des Onboarding-Dienstes, die für diesen Dienst spezifisch sind.

## Feldzuordnung {#field-mapping}

Um Daten von einem bestimmten Lead-Feld zu empfangen oder zurückzugeben, muss dieses Feld zugeordnet werden. Während die Zuordnung ein erforderlicher Schritt beim Onboarding ist, können Sie jederzeit zurückkehren, um die Zuordnungen später zu ändern. Es gibt zwei Arten von Zuordnungen, die in separaten Bildschirmen konfiguriert sind: **Ausgehende Felder**, die an den Dienst gesendet werden, wenn Marketo den Flussschritt aufruft, und **Eingehende Felder** Hierbei handelt es sich um Felder, die Daten vom Dienst empfangen können, wenn er Daten an Marketo zurückgibt.

>[!NOTE]
>
>Durch die Zuordnung eines ausgehenden Felds gewähren Sie Marketo die Erlaubnis, Daten aus diesem Feld zu Leads zu übertragen, die vom zugehörigen Dienst verarbeitet werden. Stellen Sie sicher, dass Sie über eine geeignete Rechtsfähigkeit und Autorität verfügen, um diese Daten an Ihren Dienstleister zu übermitteln, da diese Felder personenbezogene Daten umfassen können, die unter Datenschutz-, Schutz- und Mandantenrecht fallen.

Optionale Feldzuordnungen können ohne Unterbrechung Ihres Dienstes deaktiviert werden, erforderliche Zuordnungen können jedoch nicht vollständig entfernt oder deaktiviert werden.

## Service-gesteuerte Zuordnungen {#service-driven-mappings}

Dienste mit einem festen Satz von Ein- und Ausgabe, wie z. B. ein Schritt zum Registrieren von Ereignissen, verwenden **Service-gesteuerte Zuordnungen**. Für diese Art der Zuordnung stellt der Dienstleister sowohl einen Datentyp als auch einen Hinweis in Form eines API-Namens bereit. Wenn der Tipp mit dem API-Namen eines vorhandenen Lead-Felds übereinstimmt, wird dieses Feld automatisch im Zuordnungsabschnitt ausgefüllt. Bei Feldern ohne entsprechenden Hinweis müssen Sie die Zuordnung manuell aus der Liste der Felder mit dem entsprechenden Datentyp ausfüllen. Zuordnungen, die erforderlich sind, müssen ausgefüllt werden, um das Onboarding abzuschließen.

![](assets/flow-step-service-2.png)

## Benutzergesteuerte Zuordnungen {#user-driven-mappings}

Dienste ohne feste Eingabe- und Ausgabesätze, wie z. B. einen Datumsformatierungsdienst, verwenden **Benutzergesteuerte Zuordnungen**. Dies bedeutet, dass jedes eingehende und ausgehende Feld von einem Administrator konfiguriert werden muss.

![](assets/flow-step-service-3.png)

## Ausgehende Felder {#outgoing-fields}

Ausgehende Felder werden an den Flow Step Service gesendet, wenn dieser Flussschritt in einer intelligenten Kampagne verwendet wird.

## Eingehende Felder {#incoming-fields}

Eingehende Felder sind diejenigen, in die der Flow Step Service Daten schreiben darf.

## Konfigurationsoptionen (optional) {#configuration-options}

Einige Dienste verfügen entweder über optionale oder erforderliche globale Konfigurationsoptionen. Wenn eine Option erforderlich ist, muss für alle erforderlichen Optionen ein Wert festgelegt werden, bevor das Onboarding gespeichert oder abgeschlossen werden kann. Parameter, deren Namen kursiv sind, werden als Kopfzeilen an den aufgerufenen Dienst gesendet.

![](assets/flow-step-service-4.png)

## Wiedergeben eines Dienstes {#retiring-a-service}

Um den Übergang zu neuen oder alternativen Versionen eines Dienstes zu erleichtern, ohne die aktive Nutzung zu unterbrechen, können Dienste aus dem Menü Dienstanbieter entfernt werden. **Wiedergeben eines Dienstes** entfernt den entsprechenden Flussschritt aus der Palette &quot;Fluss intelligenter Kampagnen&quot;, sodass keine neuen Verwendungen erstellt werden können. In den meisten Fällen sollten Sie über einen Ersatzdienst verfügen, der den vorhandenen Dienst ersetzen kann, wenn Sie sich für die Einstellung eines Dienstes entscheiden.

## Service Deprecation {#service-deprecation}

Manchmal müssen Dienstanbieter Flussschrittdienste als normalen Teil des Software-Lebenszyklus nicht mehr unterstützen. Wenn ein Dienstleister dies ankündigt, werden das Verfallsdatum und die Nachricht in die Rasteransicht &quot;Dienstanbieter&quot;eingetragen. Wenn Sie einen veralteten Dienst weiter verwenden, kann dies zu einer Dienstunterbrechung führen, wenn dieser nicht mehr die erwartete Antwort liefert oder die Annahme von Anforderungen von Smart Campaigns aus Marketo beendet wird. Achten Sie daher besonders auf alle Benachrichtigungen zur Dienstveraltung, die Sie erhalten, und ergreifen Sie geeignete Maßnahmen, um alle noch verwendeten Schritte des Dienstes zurückzuziehen oder zu ersetzen.

## Verwenden von Drittanbieter- und benutzerdefinierten Flussschritten {#using-third-party-and-custom-flow-steps}

Installierte Durchsatzschritte können weitgehend auf die gleiche Weise wie normale Durchsatzschritte verwendet werden. Alle vom Dienst definierten Flussparameter werden Endbenutzern angezeigt.

## Aktualisieren von Picklists {#refreshing-picklists}

Marketo aktualisiert jede Nacht die Auswahlmöglichkeiten der Auswahllisten für Dienste. Es gibt jedoch Situationen, in denen Sie neue Auswahlmöglichkeiten benötigen, z. B. die Erstellung von Kampagnen. Sie können diese einfach von jeder Instanz Ihres Flussprotokolls aktualisieren, indem Sie die Schaltfläche &quot;Aktualisieren&quot;verwenden oder im Menü Admin > Dienstanbieter auf Auswahlliste aktualisieren klicken, sobald Sie Ihren Dienst ausgewählt haben.

## Eingehende Felder überprüfen {#checking-incoming-fields}

Sie können überprüfen, welche eingehenden Felder für einen bestimmten Flussschritt konfiguriert sind, indem Sie den Mauszeiger über das QuickInfo-Symbol bewegen. Dies ist nützlich, um zu bestimmen, welche Felder sich ändern können, wenn ein Lead durch ihn fließt, sodass Sie Optionen in nachfolgenden Schritten mit diesen Feldern konfigurieren können.

![](assets/flow-step-service-5.png)

## Eingehende Felder und Datenwertänderungen {#incoming-fields-and-data-value-changes}

Im Gegensatz zu den meisten anderen Flussschritten können solche, die mit dem SSFS-Framework implementiert werden, Daten in Lead-Felder zurückschreiben, die von einem Administrator zugeordnet werden, und diese Änderungen als Datenwertänderung-Aktivitäten aufzeichnen.  Wenn ein Flussschritt Daten auf diese Weise schreibt, werden alle diese Änderungen abgeschlossen, bevor die Smart-Kampagne zu allen nachfolgenden Schritten wechselt, sodass sich alle geschriebenen Daten bei nachfolgenden Flussschritt-Entscheidungen auf sie verlassen können.

## Dienstprotokolle und Statistiken {#service-logs-and-statistics}

Jedem Flow Step Service sind verschiedene Arten der Protokollierung zugeordnet, um den Zustand zu überwachen und Probleme im Zusammenhang mit der Integration zu beheben.

## Service Statistics {#service-statistics}

Das Protokoll Dienststatistiken aggregiert die Ergebnisse von Aufrufen und Rückrufen für jeden Dienst. Sie werden nach Zeit, Ebene (Chunk oder Datensatz) und Code gruppiert und liefern Zählungen sowie die aktuellste Protokollmeldung für jeden empfangenen Code. Dieses Dashboard soll vor allem die Überwachung des Zustands der Dienste unterstützen.
