---
unique-page-id: 11373011
description: Übergang zum E-Mail-Editor 2.0 - Marketing-Dokumente - Produktdokumentation
title: Übergang zum E-Mail-Editor 2.0
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Übergang zum E-Mail-Editor 2.0 {#transitioning-to-email-editor}

Seit der Version [vom](../../../../release-notes/2016/release-notes-spring-16.md)19. Juni wurden alle Marketo-Abonnement auf Email Editor 2.0 umgestellt. [Erfahren Sie mehr](https://nation.marketo.com/docs/DOC-7038) über die Einstellung des E-Mail-Editors 1.0.

E-Mails und E-Mail-Vorlagen in Ihrem Abonnement sollten eine Versionsnummer haben. Die Version befindet sich auf der Zusammenfassungsseite des Assets.

![](assets/five-5.png)

Standardmäßig werden alle vorhandenen E-Mails und E-Mail-Vorlagen als v1.0 markiert, wenn sie entweder vor der Version Frühjahr 2016 oder nach der Veröffentlichung erstellt wurden, wenn E-Mail Editor 2.0 deaktiviert ist. Bei aktiviertem E-Mail-Editor 2.0 wird das folgende Verhalten angezeigt:

* Wenn Sie eine neue E-Mail erstellen, wird der [E-Mail-Vorlagenwähler](email-template-picker-overview.md) angezeigt und Sie können eine E-Mail-Vorlage der Version 2.0 auswählen.
* Wenn Sie eine E-Mail mit E-Mail-Editor 2.0 erstellen oder bearbeiten, wird die resultierende E-Mail **immer** als v2.0 gekennzeichnet (auch wenn Sie eine E-Mail-Vorlage der Version 1.0 verwendet haben).

Wenn Ihr Abonnement E-Mails der Version 1.0 vor dem Wechsel zu E-Mail Editor 2.0 enthält, wird das folgende Verhalten je nach dem aktuellen Status des Assets angezeigt:

**Genehmigt** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird ein Entwurf der genehmigten E-Mail der Version 2.0 erstellt. Wenn Sie dann den Entwurf der Version 2.0 genehmigen, wird der genehmigte Status der E-Mail zu Version 2.0 und es gibt keine Möglichkeit, zu Version 1.0 zurückzukehren.\
**Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als v2.0 markiert. Zu diesem Zeitpunkt ist es nicht möglich, v1.0 zu verwerfen und wiederherzustellen, da es keine genehmigte Version des Assets gibt.\
**Genehmigt mit Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als Version 2.0 markiert. Aus diesem Grund gibt es auch keine Möglichkeit, den Entwurf zurück auf v1.0 zurückzusetzen.

Wenn Ihr Abonnement E-Mail-Vorlagen der Version 1.0 vor dem Wechsel zu E-Mail-Editor 2.0 enthält, wird folgendes Verhalten festgestellt:

**Genehmigt** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird ein Entwurf der vorhandenen E-Mail-Vorlage der Version 2.0 erstellt.\
**Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als v2.0 markiert. Zu diesem Zeitpunkt ist es nicht möglich, v1.0 zu verwerfen und wiederherzustellen, da keine genehmigte Version des Assets vorhanden ist.\
**Genehmigt mit Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als v2.0 markiert. Aus diesem Grund gibt es auch keine Möglichkeit, den Entwurf zurück auf v1.0 zurückzusetzen.

Wenn Sie eine E-Mail-Vorlage genehmigen, die zuvor v1.0 war (in einem der oben genannten Status), sehen Sie das folgende Verhalten:

Für vorhandene E-Mails der Version 1.0, die die (zuvor v1.0)-Vorlage verwendeten:\
**Genehmigte E-Mail** der Version 1.0 - Für diese E-Mail wird ein Entwurf der Version 2.0 erstellt, wobei die neu genehmigte Vorlage der Version 2.0 verwendet wird. Es werden auch alle Vorlagenänderungen empfangen.\
**Entwurf der E-Mail** v1.0 - Der Entwurf bleibt v1.0, bis Sie auf &quot;Entwurf bearbeiten&quot;klicken. Danach wird es automatisch als v2.0 markiert und alle Vorlagenänderungen erhalten.\
**Mit Entwurf v1.0 E-Mail** genehmigt - Der Entwurf bleibt v1.0, bis Sie auf &quot;Entwurf bearbeiten&quot;klicken. Danach wird es automatisch als v2.0 markiert und alle Vorlagenänderungen erhalten.

Für vorhandene E-Mails der Version 2.0, die die (zuvor v1.0)-Vorlage verwendeten:\
**Genehmigte E-Mail** der Version 2.0 - Für diese E-Mail wird ein Entwurf der Version 2.0 erstellt, die neu genehmigte Vorlage wird weiterhin &quot;verwendet&quot;und alle Vorlagenänderungen werden empfangen.\
**Entwurf der E-Mail** v2.0 - Der Entwurf bleibt unverändert (v2.0) und erhält alle Vorlagenänderungen.\
**Genehmigt mit Entwurf v2.0 E-Mail** - Der Entwurf bleibt unverändert (v2.0) und erhält alle Vorlagenänderungen.

>[!CAUTION]
>
>Wenn Sie den Entwurf einer E-Mail-Vorlage der Version 2.0 genehmigen, wird die Vorlage zu Version 2.0. Es gibt **keine Möglichkeit** , sie auf v1.0 zurückzukehren.

Hinweise

* Genehmigte E-Mails werden **nie** geändert.

* Genehmigte E-Mail-Vorlagen werden **nie** geändert.

* In einigen **seltenen** Fällen kann eine E-Mail der Version 1.0 nicht im E-Mail-Editor 2.0 geöffnet werden. Falls dies der Fall ist, verwerfen Sie den Entwurf und wenden Sie sich an den Support von Marketing.

>[!MORELIKETHIS]
>
>* [Übersicht über Email Editor 2.0](email-editor-v2-0-overview.md)
>* [Syntax der E-Mail-Vorlage](email-template-syntax.md)

>



