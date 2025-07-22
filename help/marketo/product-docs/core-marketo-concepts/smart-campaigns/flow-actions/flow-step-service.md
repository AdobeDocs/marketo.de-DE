---
description: Flow Step Service - Marketo-Dokumente - Produktdokumentation
title: Flow-Schritt-Service
exl-id: 81367562-8b27-4ec5-8a9b-b02083a2e999
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 0%

---

# Flow-Schritt-Service {#flow-step-service}

Self-Service Flow Steps ist ein Framework und eine Reihe von Funktionen für das Verfassen, Veröffentlichen und Integrieren von Web-Services in Adobe Marketo Engage Smart Campaign. Dieses Handbuch richtet sich an Marketo Engage-Endbenutzer, die Services installieren und verwenden möchten, die bereits erstellt und veröffentlicht wurden. Informationen zum Verfassen und Veröffentlichen Ihres eigenen Services finden Sie im [[!DNL GitHub] Repository für die Benutzeroberfläche des Dienstleisters](https://github.com/adobe/Marketo-SSFS-Service-Provider-Interface){target="_blank"}. Eine Implementierung der Proof-of-Concept-Lookup-Tabelle finden Sie [hier](https://github.com/adobe/mkto-flow-lookup){target="_blank"}.

## Onboarding und Verwalten von Services {#onboarding-and-managing-services}

Die Installation eines benutzerdefinierten Flussschritts erfordert Administratorberechtigungen in Marketo. Abgesehen von der Installations-URL können alle anderen Aspekte eines Services nach Abschluss des ersten Onboarding bearbeitet werden, indem ein Drilldown in den Bildschirm mit den Service-Details vom Raster der Service-Anbieter durchgeführt wird.

## Installations-URL {#installation-url}

Um mit der Installation zu beginnen, müssen Sie zunächst die URL des OpenAPI-Dokuments abrufen, das Ihren Dienst definiert. Ihr Dienstleister sollte Ihnen dies zur Verfügung stellen können und wird in der Regel eine URL haben, die auf `/openapi.json` endet. Vollständige URLs sehen in etwa so aus wie `https://www.example.com/OpenAPI.json`. Sobald Sie diese URL haben, gehen Sie zum Menü [!UICONTROL Dienstleister] in Ihrem [!UICONTROL Admin] Abschnitt.

Klicken Sie **[!UICONTROL Weiter]**, um zum Abschnitt Service-Anmeldeinformationen eingeben zu wechseln.

![](assets/flow-step-service-1.png)

## Service-Anmeldeinformationen eingeben {#enter-service-credentials}

Um auf den installierten Service zugreifen zu können, muss Marketo über gültige API-Anmeldeinformationen verfügen. Diese Anmeldeinformationen sollten Sie von Ihrem Dienstleister erhalten. Services verfügen über drei verschiedene Authentifizierungsoptionen, sodass möglicherweise eine von drei verschiedenen Eingabeaufforderungen für Anmeldeinformationen angezeigt wird: **API-Schlüssel** mit nur einem Eingabefeld, **Standardauthentifizierung** für die ein Benutzername und ein Kennwort erforderlich sind und möglicherweise auch ein Feld namens „Realm“ erforderlich ist, und **OAuth2** unter Verwendung der _Client-Anmeldeinformationen_, für die eine _Client-ID_ und _Client-Geheimnis_ erforderlich ist.

Wenn Sie Ihre Anmeldeinformationen speichern, versucht Marketo, den Status-Endpunkt des Services aufzurufen, um zu überprüfen, ob sie gültig sind. Wenn die angegebenen Anmeldeinformationen ungültig sind, wird ein Fehler angezeigt, der dies angibt.

>[!CAUTION]
>
>Wenn ein Dienstleister erstellt und gelöscht wird, können Sie seinen Dienstleister-, API-, Trigger- oder Filternamen künftig nicht mehr wiederverwenden.

## Onboarding-Handbuch (optional) {#onboarding-guide}

Bei einigen Dienstleistern wird ein optionaler Onboarding-Schritt integriert. Dieser Schritt enthält alle zusätzlichen Anweisungen zum Durchführen des Onboarding-Services, die für diesen Service spezifisch sind.

## Feldzuordnung {#field-mapping}

Um Daten von einem bestimmten Lead-Feld zu empfangen oder zurückzugeben, muss dieses Feld zugeordnet werden. Während die Zuordnung ein erforderlicher Schritt beim Onboarding ist, können Sie jederzeit zurückkehren, um die Zuordnungen später zu ändern. Es gibt zwei Arten von Zuordnungen, die in separaten Bildschirmen konfiguriert sind: **Ausgehende Felder**, die an den Service gesendet werden, wenn Marketo den Flussschritt aufruft, und **Eingehende Felder** bei denen es sich um Felder handelt, die Daten vom Service empfangen können, wenn sie Daten an Marketo zurückgeben.

>[!NOTE]
>
>Durch die Zuordnung eines ausgehenden Felds erteilen Sie Marketo die Berechtigung, Daten aus diesem Feld zu übertragen, die sich auf Leads beziehen, die vom zugehörigen Service verarbeitet werden. Stellen Sie sicher, dass Sie über einen angemessenen rechtlichen Status und die Befugnis verfügen, diese Daten an Ihren Dienstleister zu übermitteln, da diese Felder personenbezogene Daten enthalten können, die unter das Datenschutz-, Schutz- und Mietrecht fallen.

Optionale Feldzuordnungen können ohne Unterbrechung Ihres Service deaktiviert werden, aber die erforderlichen Zuordnungen können nicht entfernt oder vollständig deaktiviert werden.

## Service-gesteuerte Zuordnungen {#service-driven-mappings}

Dienste mit einem festen Satz von Eingaben und Ausgaben, z. B. ein Ereignisregistrierungsflussschritt, verwenden **Service-gesteuerte Zuordnungen**. Für diese Art der Zuordnung gibt der Dienstleister sowohl einen Datentyp als auch einen Hinweis in Form eines API-Namens an. Wenn der Hinweis mit dem API-Namen eines vorhandenen Lead-Felds übereinstimmt, wird dieses Feld automatisch im Abschnitt „Zuordnung“ ausgefüllt. Bei Feldern ohne übereinstimmenden Hinweis müssen Sie die Zuordnung manuell aus der Liste der Felder mit dem entsprechenden Datentyp ausfüllen. Erforderliche Zuordnungen müssen ausgefüllt werden, um das Onboarding abzuschließen.

![](assets/flow-step-service-2.png)

## Benutzergesteuerte Zuordnungen {#user-driven-mappings}

Dienste, die nicht über einen festen Satz von Eingaben und Ausgaben verfügen, wie z. B. ein Service zur Datumsformatierung, verwenden **benutzergesteuerte Zuordnungen**. Das bedeutet, dass jedes eingehende und ausgehende Feld von einem Administrator konfiguriert werden muss.

![](assets/flow-step-service-3.png)

## Ausgehende Felder {#outgoing-fields}

Ausgehende Felder sind diejenigen, die an den Fluss-Schritt-Service gesendet werden, wenn dieser Fluss-Schritt in einer intelligenten Kampagne verwendet wird.

## Eingehende Felder {#incoming-fields}

Eingehende Felder sind diejenigen, in die der Flow Step Service Daten schreiben darf.

## Konfigurationsoptionen (optional) {#configuration-options}

Einige Dienste verfügen entweder über optionale oder erforderliche globale Konfigurationsoptionen. Wenn Optionen erforderlich sind, muss ein Wert für alle erforderlichen Optionen festgelegt werden, bevor das Onboarding gespeichert oder abgeschlossen wird. Parameter, deren Namen kursiv gedruckt sind, werden als Kopfzeilen an den aufgerufenen Service gesendet.

![](assets/flow-step-service-4.png)

## Einstellen eines Services {#retiring-a-service}

Um den Übergang zu neuen oder alternativen Versionen eines Services zu erleichtern, ohne die aktive Nutzung zu unterbrechen, können Services aus dem Menü Service-Anbieter entfernt werden. **Einstellung eines** entfernt den entsprechenden Flussschritt aus der Smart Campaign-Flusspalette, sodass keine neuen Verwendungen mehr erstellt werden können. In den meisten Fällen sollten Sie einen Ersatz-Service haben, der bereit ist, den vorhandenen Service zu ersetzen, wenn Sie einen Service einstellen.

## Service-Einstellung {#service-deprecation}

Manchmal müssen Service-Anbieter Flow Step-Services als normalen Teil des Software-Lebenszyklus einstellen. Wenn ein Dienstleister dies ankündigt, werden das Datum der Einstellung und die Nachricht in der Rasteransicht Dienstleister angezeigt. Die weitere Verwendung eines veralteten Services kann zu einer Unterbrechung des Services führen, wenn er nicht mehr wie erwartet reagiert oder keine Anfragen mehr von Marketo Smart Campaign akzeptiert. Daher sollten Sie besonders auf Benachrichtigungen zur Einstellung von Services achten, die Sie erhalten, und geeignete Schritte ergreifen, um den Service einzustellen oder zu ersetzen, der noch in Verwendung ist.

## Verwenden von Drittanbieter- und benutzerdefinierten Flussschritten {#using-third-party-and-custom-flow-steps}

Installierte Fließschritte können weitgehend genauso wie normale Fließschritte verwendet werden. Alle vom Service definierten Flussparameter werden den Endbenutzern angezeigt.

## Picklisten werden aktualisiert {#refreshing-picklists}

Marketo aktualisiert die Auswahllistenoptionen für Services jede Nacht. In manchen Fällen sind jedoch neue Auswahlmöglichkeiten erforderlich, z. B. bei der Kampagnenerstellung. Sie können diese einfach von jeder Instanz Ihres Flussschritts aus aktualisieren, indem Sie die Schaltfläche Aktualisieren verwenden, oder indem Sie zum Menü [!UICONTROL Admin] > [!UICONTROL Dienstleister] wechseln und auf [!UICONTROL Auswahlliste aktualisieren] klicken, nachdem Sie Ihren Dienst ausgewählt haben.

## Überprüfen eingehender Felder {#checking-incoming-fields}

Sie können überprüfen, welche eingehenden Felder für einen bestimmten Flussschritt konfiguriert sind, indem Sie den Mauszeiger über das QuickInfo-Symbol bewegen. Dies ist nützlich, um zu bestimmen, welche Felder sich ändern können, wenn ein Lead durch sie fließt, sodass Sie in nachfolgenden Schritten mithilfe dieser Felder Auswahlmöglichkeiten konfigurieren können.

![](assets/flow-step-service-5.png)

## Eingehende Felder und Änderungen von Datenwerten {#incoming-fields-and-data-value-changes}

Im Gegensatz zu den meisten anderen Flussschritten können diejenigen, die mit dem SSFS-Framework implementiert sind, Daten zurück in Lead-Felder schreiben, die von einer Administratorin bzw. einem Administrator zugeordnet werden, und diese Änderungen als Datenwertänderungsaktivitäten erfassen.  Wenn Daten in einem Flussschritt auf diese Weise geschrieben werden, werden alle diese Änderungen abgeschlossen, bevor die intelligente Kampagne mit allen nachfolgenden Schritten fortfährt, sodass alle geschriebenen Daten in nachfolgenden Flussschritt-Entscheidungen zuverlässig sind.

## Service-Protokolle und Statistiken {#service-logs-and-statistics}

Jedem Flow Step-Dienst sind mehrere Arten der Protokollierung zugeordnet, um den Zustand zu überwachen und Probleme im Zusammenhang mit der Integration zu beheben.

## Service Statistics {#service-statistics}

Das Statistikprotokoll zu Services aggregiert die Ergebnisse von Aufrufen und Callbacks für jeden Service. Sie werden nach Zeit, Ebene (Block oder Datensatz) und Code gruppiert und geben die Zählungen und die neueste Protokollmeldung für jeden empfangenen Code an. Dieses Dashboard dient hauptsächlich zur Überwachung des Service-Zustands.
