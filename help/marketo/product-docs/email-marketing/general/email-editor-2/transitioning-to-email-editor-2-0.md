---
unique-page-id: 11373011
description: Umstellung auf Email Editor 2.0 - Marketo-Dokumente - Produktdokumentation
title: Übergang zum E-Mail-Editor 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Übergang zum E-Mail-Editor 2.0 {#transitioning-to-email-editor}

Seit der Version vom 19. Juni wurden alle Marketo-Abonnements auf Email Editor 2.0 umgestellt. [Weitere Infos](https://nation.marketo.com/docs/DOC-7038) zur Einstellung von Email Editor 1.0 .

E-Mails und E-Mail-Vorlagen in Ihrem Abonnement sollten über eine Versionsnummer verfügen. Die Version finden Sie auf der Übersichtsseite des Assets.

![](assets/five-5.png)

Standardmäßig werden all Ihre vorhandenen E-Mails und E-Mail-Vorlagen als v1.0 gekennzeichnet, wenn sie entweder vor der Frühlingsversion 16 oder nach der Veröffentlichung erstellt wurden, wenn E-Mail-Editor 2.0 deaktiviert ist. Wenn Email Editor 2.0 jetzt automatisch aktiviert ist, sehen Sie folgendes Verhalten:

* Wenn Sie eine neue E-Mail erstellen, wird die [E-Mail-Vorlagenauswahl](email-template-picker-overview.md) wird angezeigt und Sie können eine E-Mail-Vorlage v2.0 auswählen.
* Bei jeder Erstellung oder Bearbeitung einer E-Mail mit Email Editor 2.0 wird die resultierende E-Mail **always** als v2.0 markiert sein (auch wenn Sie eine E-Mail-Vorlage v1.0 verwendet haben).

Wenn Ihr Abonnement v1.0-E-Mails vor dem Wechsel zu E-Mail-Editor 2.0 enthält, wird das folgende Verhalten basierend auf dem aktuellen Status des Assets angezeigt:

**Genehmigt** - Wenn Sie auf &quot;Entwurf bearbeiten&quot;klicken, wird ein Entwurf der genehmigten E-Mail der Version 2.0 erstellt. Wenn Sie dann den Entwurf der Version 2.0 genehmigen, wird der genehmigte Status der E-Mail zu v2.0 und es gibt keine Möglichkeit, zurück zu v1.0 zu wechseln.\
**Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als v2.0 markiert. Zu diesem Zeitpunkt ist es nicht möglich, v1.0 zu verwerfen und wiederherzustellen, da keine genehmigte Version des Assets vorhanden ist.
**Genehmigt mit Entwurf** - Wenn Sie auf &quot;Entwurf bearbeiten&quot;klicken, wird dieser Entwurf automatisch als v2.0 markiert. Aus diesem Grund gibt es auch keine Möglichkeit, den Entwurf zurück auf v1.0 zu setzen.

Wenn Ihr Abonnement über E-Mail-Vorlagen der Version 1.0 verfügt, bevor Sie zu Email Editor 2.0 wechseln, wird Folgendes angezeigt:

**Genehmigt** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird ein Entwurf der vorhandenen E-Mail-Vorlage der Version 2.0 erstellt.
**Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als v2.0 markiert. Zu diesem Zeitpunkt ist es nicht möglich, v1.0 zu verwerfen und wiederherzustellen, da keine genehmigte Version des Assets vorhanden ist.
**Genehmigt mit Entwurf** - Durch Klicken auf &quot;Entwurf bearbeiten&quot;wird dieser Entwurf automatisch als v2.0 markiert. Aus diesem Grund gibt es auch keine Möglichkeit, den Entwurf zurück auf v1.0 zu setzen.

Wenn Sie eine E-Mail-Vorlage genehmigen, die zuvor v1.0 war (in einem der oben genannten Status), sehen Sie folgendes Verhalten:

Für vorhandene E-Mails der Version 1.0, die die (zuvor v1.0)-Vorlage verwendeten:\
**Genehmigte E-Mail-Version 1.0** - Für diese E-Mail wird ein Entwurf der Version 2.0 erstellt, der weiterhin die neu genehmigte Vorlage der Version 2.0 verwendet. Sie erhält auch alle Vorlagenänderungen.\
**Entwurf v1.0-E-Mail** - Der Entwurf bleibt v1.0, bis Sie auf &quot;Entwurf bearbeiten&quot;klicken. Danach wird er automatisch als v2.0 markiert und erhält alle Vorlagenänderungen.\
**Genehmigt mit Entwurf v1.0-E-Mail** - Der Entwurf bleibt v1.0, bis Sie auf &quot;Entwurf bearbeiten&quot;klicken. Danach wird er automatisch als v2.0 markiert und erhält alle Vorlagenänderungen.

Für vorhandene E-Mails der Version 2.0, die die (zuvor v1.0)-Vorlage verwendeten:\
**Genehmigte E-Mail-Version 2.0** - Für diese E-Mail wird ein Entwurf der Version 2.0 erstellt, der die neu genehmigte Vorlage weiterhin &quot;verwendet&quot;, und alle Vorlagenänderungen erhält.\
**Entwurf v2.0-E-Mail** - Der Entwurf bleibt unverändert (v2.0) und erhält alle Vorlagenänderungen.\
**Genehmigt mit Entwurf v2.0-E-Mail** - Der Entwurf bleibt unverändert (v2.0) und erhält alle Vorlagenänderungen.

>[!CAUTION]
>
>Wenn Sie den Entwurf einer E-Mail-Vorlage der Version 2.0 genehmigen, wird die Vorlage zu Version 2.0. Es gibt **no way** , um es auf v1.0 zurückzusetzen.

Zu beachten

* Genehmigte E-Mails sind **never** geändert.

* Genehmigte E-Mail-Vorlagen sind **never** geändert.

* In einigen **selten** kann in E-Mail-Editor 2.0 keine E-Mail der Version 1.0 geöffnet werden. Wenn dies der Fall ist, verwerfen Sie den Entwurf und wenden Sie sich an den Marketo-Support.

>[!MORELIKETHIS]
>
>* [Übersicht über Email Editor 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Syntax der E-Mail-Vorlage](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
