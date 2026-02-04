---
unique-page-id: 2949469
description: Einrichtungsschritte – Marketo-Dokumente – Produktdokumentation
title: Einrichtungsschritte
hide: true
hidefromtoc: true
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2086'
ht-degree: 69%

---

# Einrichtungsschritte {#setup-steps}

**Willkommen bei Adobe Marketo Engage.**

Bevor Sie sich mit der Verwendung von Marketo vertraut machen, müssen Sie einige Schritte ausführen.

Diese Schritte sind:

* Einige grundlegende Kontoeinstellungen
* Branding von Landingpage-URLs und E-Mail-Links zur Verbesserung von Vertrauen und Zustellbarkeit
* Synchronisieren des CRM
* Hinzufügen von Trackingcode zu Ihrer Unternehmens-Website

>[!NOTE]
>
>Sie müssen diese Schritte nur ausführen, wenn Ihr Unternehmen **mit der Verwendung von Marketo gerade erst beginnt**. Andernfalls ist die Einrichtung möglicherweise bereits abgeschlossen.

Einige Schritte erfordern Unterstützung von Ihrem IT-Team.

>[!TIP]
>
>Wenn Sie [Checkliste ausdrucken](/help/marketo/getting-started/initial-setup/setup-checklist.md){target="_blank"} können Sie Elemente beim Ausfüllen abhaken.

## Anmelden und zusätzliche Marketo-Benutzer erstellen {#log-in-and-create-additional-marketo-users}

>[!IMPORTANT]
>
>Wenn Ihr Marketo-Abonnement am/nach dem 31. Juli 2023 erstellt wurde oder bereits zu [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"} migriert wurde, gelten die unten beschriebenen Schritte zum Hinzufügen eines Benutzers nicht für Sie. Siehe stattdessen [diesen Artikel](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}.

Melden Sie sich bei Marketo [hier](https://app.marketo.com/){target="_blank"} mit den Anmeldedaten an, die Sie per E-Mail erhalten haben.

![](assets/setup-steps-1.png)

Herzlichen Glückwunsch! Sie befinden sich jetzt in Marketo und können beginnen, etwas zu entdecken. Vielleicht möchten Sie Ihre Kollegen aus dem Marketing-Team einladen, sich Ihnen anzuschließen. Sie können dies tun, indem Sie neue Benutzer hinzufügen.

Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

>[!TIP]
>
>Wenn Sie hier sind, können Sie auf **[!UICONTROL Mein Konto]** klicken, um Ihre Konto- und Standorteinstellungen zu ändern und einen neuen Abonnementnamen festzulegen.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

![](assets/setup-steps-3.png)

Klicken Sie **[!UICONTROL Neuen Benutzer einladen]**.

![](assets/setup-steps-4.png)

Geben Sie die E-Mail-Adresse, den Vornamen und den Nachnamen Ihres Kollegen ein. _Das Festlegen eines Ablaufdatums für den Zugriff ist optional_. Klicken Sie auf **[!UICONTROL Weiter]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Ein Ablaufdatum ist ideal für kurzfristige externe Stakeholder oder Berater, die nur für einen kurzen Zeitraum Zugriff auf Marketo benötigen.

>[!NOTE]
>
>Wenn das Ablaufdatum eintrifft, erhält der Benutzer eine Ablaufbenachrichtigung, und das Konto wird gesperrt.

Wählen Sie eine Rolle aus und klicken Sie auf **[!UICONTROL Weiter]**. Standardbenutzer haben Zugriff auf alle Bereiche außer Admin.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Zusätzlich zu den fünf integrierten Rollen können Sie auch benutzerdefinierte Rollen erstellen. Weitere Informationen zu [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

Sie können den Einladungstext anpassen. Klicken Sie auf **Senden**.

![](assets/setup-steps-7.png)

Der neue Benutzer wird jetzt auf der Registerkarte **[!UICONTROL Benutzer]** aufgeführt und sollte eine E-Mail mit einem Link erhalten, um ein Kennwort und eine Anmeldung zu erstellen. Nächster Schritt!

![](assets/setup-steps-8.png)

## Einrichten autorisierter Support-Kontakte {#set-up-your-authorized-support-contacts}

Möglicherweise haben Sie eine E-Mail vom Marketo-Support erhalten, in der Sie darauf hingewiesen werden, dass Sie der Marketo-Support-Administrator für Ihr Unternehmen sind. In diesem Fall können Sie **autorisierte Support-Kontakte** für Ihr Team einrichten. Nur autorisierte Support-Kontakte können sich direkt über das [Marketo Support-Portal an den Marketo-Support &#x200B;](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>Die Anzahl der Support-Kontakte, die Sie erstellen können, wird durch das von Ihnen erworbene Paket bestimmt. Dieser Grenzwert wird in Ihrer E-Mail vom Marketo-Support angegeben.

Autorisierte Support-Kontaktdokumente wurden in die Marketo-Community verschoben. Siehe [&#x200B; Artikel](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

>[!NOTE]
>
>In der Liste werden nur Personen angezeigt, die sich bei der Marketo-Community angemeldet haben. Wenn Sie die Person nicht finden können, stellen Sie sicher, dass sie sich zuerst bei der Community anmeldet.

## Anpassen der Landingpage-URLs mit einem CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Sind Sie Launch-Pack-Kundin bzw. -Kunde? Dann können Sie diesen Schritt überspringen. Ihre Beraterin bzw. Ihr Berater stellt Ihnen während Ihres Einstiegsgesprächs eine Anleitung zur Einrichtung des IT-Systems zur Verfügung.

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

Wählen Sie einen CNAME für Ihre Landingpages aus. Einige Beispiele:

    * **go**.[UnternehmensDomain].com
    * **www2**.[UnternehmensDomain].com
    * **lp**.[UnternehmensDomain].com

>[!TIP]
>
>Halten Sie es kurz. Kürzere URLs sind leichter zu merken. Wir schlagen „go“ als Domain vor.

Der erste Teil (fett gedruckt) ist der `[LandingPageCNAME]`. Sie benötigen ihn in Schritt 5.

Um die Munchkin-ID abzurufen, die Sie durch Ihren Landingpage-CNAME ersetzen werden, navigieren Sie zum Bereich Admin .

![](assets/setup-steps-9.png)

Klicken Sie auf **Mein Konto**.

![](assets/setup-steps-10.png)

Kopieren Sie die [!UICONTROL Kontozeichenfolge] aus den Landingpage-Einstellungen.

![](assets/setup-steps-11.png)

Dies ist die `[Munchkin ID]`. Speichern Sie diese Information. Sie müssen sie in Schritt 5 der IT-Abteilung bereitstellen.

Konfigurieren Sie Ihre Domain-Einstellungen so, dass Landingpages die Domain Ihres Unternehmens anstelle der von Marketo (wo sie gehostet werden) verwenden.

## Sicherstellen der E-Mail-Zustellbarkeit {#ensure-email-deliverability}

>[!NOTE]
>
>Sind Sie Launch-Pack-Kundin bzw. -Kunde? Dann können Sie diesen Schritt überspringen. Ihre Beraterin bzw. Ihr Berater stellt Ihnen während Ihres Einstiegsgesprächs eine Anleitung zur Einrichtung des IT-Systems zur Verfügung.

Es gibt verschiedene Maßnahmen, mit denen Sie sicherstellen können, dass Ihre E-Mails so viele Personen wie möglich erreichen.

* **Versehen Sie Ihre Tracking-Links mit Branding**. Sie können einen CNAME auswählen, um Ihre eigene Domain (anstelle der von Marketo) in den Links zu verwenden, die Sie in E-Mails von Marketo einschließen. Dies stärkt das Domain-Branding und erhöht das Vertrauen und die Zustellbarkeit bei Ihren Empfängerinnen und Empfängern.
* **Marketo zu Ihrer Unternehmens-E-Mail-Zulassungsliste hinzufügen.** Es ist eine gängige Best Practice, Test-E-Mails an Testkonten zu senden, bevor E-Mails an tatsächliche Personen gesendet werden. Durch das Hinzufügen von Marketo zur Zulassungsliste können Sie verhindern, dass diese Test-E-Mails blockiert oder als Spam gekennzeichnet werden.
* **Richten Sie SPF und DKIM ein.** Diese Technologien stellen sicher, dass Ihre Marketo-E-Mails keine Spam-Mails sind. Führen Sie die folgenden Schritte aus, um [SPF und DKIM für die E-Mail-Zustellbarkeit einzurichten](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md) und so zu verhindern, dass die Spam-Filter von Empfängerinnen und Empfänger Ihre Marketo-E-Mails ablehnen.
* **Richten Sie einen MX-Eintrag für Ihre Domain ein.** Ein MX-Eintrag ermöglicht es Ihnen, E-Mails über die Domain zu empfangen, von der aus Sie E-Mails senden, um Antworten und Abwesenheitsnachrichten zu verarbeiten. Wenn Sie E-Mails von Ihrer Unternehmens-Domain aus senden, haben Sie dies wahrscheinlich bereits konfiguriert. Falls nicht, können Sie dies in der Regel so einrichten, dass eine Zuordnung zum MX-Eintrag Ihrer Unternehmens-Domain erfolgt.
* **Empfohlene Einstellungen für die Absenderadresse.** Sie müssen in allen E-Mail-Kampagnen eine gültige, vorhandene und funktionierende E-Mail-Domain in der Absenderadresse verwenden. Es kann von Vorteil sein, eine Subdomain Ihrer Unternehmens-Domain zu konfigurieren, anstatt von Ihrer Unternehmens-Domain aus zu senden. Dadurch wird sichergestellt, dass Probleme aus Ihrem Unternehmens-Mailstream sich nicht auf Ihren Marketo-Mailstream auswirken und umgekehrt. Darüber hinaus führt der Versand von E-Mails von `something@nonexistentdomain.com` dazu, dass E-Mails gefiltert oder blockiert werden. Jede Domain, die in der Absenderadresse verwendet wird, muss über ein gültiges und funktionierendes postmaster@- und abuse@-Konto verfügen.

Wenn Sie Google-Apps zum Hosten Ihrer Unternehmens-E-Mail-Adresse verwenden, können Sie unter Ihrer Domain keine abuse@- oder postmaster@-E-Mails erstellen. Um dies zu umgehen, müssen Sie Gruppen mit den Namen „abuse“ und „postmaster“ erstellen. Benutzende, die Mitglieder dieser Gruppen sind, erhalten E-Mails, die an diese Adressen gesendet werden (z. B. <postmaster@domain.com>). Detaillierte Anleitungen zum Erstellen von Gruppen finden Sie [hier](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Wählen Sie einen CNAME für E-Mail-Tracking-Links aus (wählen Sie einen CNAME aus, der sich von dem in Schritt 3 ausgewählten Landingpage-CNAME _unterscheidet_). Einige Beispiele:

* go2.[UnternehmensDomain].com
* em.[UnternehmensDomain].com
* wow.[UnternehmensDomain].com

Der erste Teil ist des E-Mail-Tracking-CNAME, `[EmailTrackingCNAME]`. In Schritt 5 müssen Sie es der IT-Abteilung geben.

>[!CAUTION]
>
>E-Mail- und Landingpage-CNAME müssen unterschiedlich sein. Vermeiden Sie außerdem CNAMEs wie „track“ oder „link“. Diese werden oft als Spam gekennzeichnet.

Um Ihren Marketo-Tracking-Link abzurufen, navigieren Sie in den Bereich **[!UICONTROL Admin]**.

![](assets/setup-steps-12.png)

Klicken Sie auf **[!UICONTROL E-Mail]**.

![](assets/setup-steps-13.png)

Kopieren Sie den [!UICONTROL Tracking-Link] aus Ihren E-Mail-Einstellungen.

Der [!UICONTROL Tracking-Link] weist folgende Struktur auf: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Dies ist Ihr `[MktoTrackingLink]`. Speichern Sie diese Information. Sie müssen sie in Schritt 5 der IT-Abteilung bereitstellen.

Erfassen Sie Absender-Domains. Erstellen Sie eine Liste aller Absender-Domains (also `[Sender]@[FromDomain].com`), die Sie für den Versand von E-Mails aus Marketo verwenden möchten. Für die meisten gibt es nur eine.

Zum Beispiel „marketo.com“, „info.marketo.com“. Dies sind `[FromDomain1]`, `[FromDomain2]` usw. Speichern Sie diese Informationen. Sie müssen sie in Schritt 5 der IT-Abteilung bereitstellen.

Sie verfügen jetzt über alle Informationen, die Sie benötigen, um Ihre Anfrage an die IT-Abteilung zu senden.

## Anfordern der Konfiguration von Protokollen bei der IT-Abteilung {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Sind Sie Launch-Pack-Kundin bzw. -Kunde? Dann können Sie diesen Schritt überspringen. Ihre Beraterin bzw. Ihr Berater stellt Ihnen während Ihres Einstiegsgesprächs eine Anleitung zur Einrichtung des IT-Systems zur Verfügung.

Sobald Sie alle erforderlichen Informationen gesammelt haben, können Sie eine Anfrage an die IT-Abteilung senden. Sie können den unten stehenden Text als Vorlage verwenden und den fett gedruckten Text durch Ihre eigenen Informationen ersetzen.

[Fügen Sie einen Link zu diesem Artikel hinzu](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Fügen Sie diesen Text in die E-Mail ein und ersetzen Sie die fett gedruckten Platzhalter:

>[!NOTE]
>
>Informationen dazu, durch welchen Text die Platzhalter ersetzt werden sollen, finden Sie oben in Schritt 3 und 4. Denken Sie daran, dass `[LandingPageCNAME]` und `[EmailTrackingCNAME]` unterschiedlich sein müssen.

`----------------------------------------------`

Sehr geehrter IT-Administrator,

unser Marketing-Team nutzt jetzt die Marketo-Plattform zur Kommunikation mit Personen. Um eine optimale Zustellbarkeit von E-Mails zu gewährleisten, müssen wir die folgenden Änderungen vornehmen:

`1)` Fügen Sie für unsere Landingpages einen DNS-Eintrag (CNAME) für **[LandingPageCNAME]**.**[UnternehmensDomain]**.com hinzu, der auf **[Munchkin-ID]**.mktoweb.com verweist.

`2)` Fügen Sie für unsere Tracking-Links in E-Mails einen DNS-Eintrag (CNAME) für **[EmailTrackingCNAME]**.**[UnternehmensDomain]**.com hinzu, der auf **[MktoTrackingLink]** verweist.

`3)` Setzen Sie Marketo auf die Zulassungsliste.

    * Wenn wir IP-Adressen in unserer E-Mail-Zulassungsliste verwenden, fügen Sie die unten aufgeführten IP-Adressen hinzu:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    94.236.119.0/26

>[!NOTE]
>
>Wenden Sie sich an den Marketo-Support, wenn Sie gerne eine gekürzte Liste von IP-Adressen speziell für Ihre Umgebung hätten, um diese der Zulassungsliste hinzuzufügen.

    * Wenn unser Anti-Spam-System Absender-Domains verwendet, fügen Sie diese hinzu:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Wir müssen SPF und DKIM einrichten, damit Marketo autorisiert ist, signierte E-Mails in unserem Namen zu senden.

`a.` Fügen Sie zur SPF-Einrichtung den DNS-Einträgen die folgende Zeile hinzu:

IN TXT **[Absender-Domain]**: v=spf1 mx ip4:**[Unternehmens-IP(s)]**
<br/>include: mktomail.com ~all

Wenn bereits ein SPF-Eintrag im DNS-Eintrag vorhanden ist, fügen Sie einfach Folgendes hinzu:

include:mktomail.com

`[`Ersetzen Sie die **Absender-Domain** durch Ihre E-Mail-Absender-Domain (z. B.: unternehmen.com) und die **Unternehmens-IP** durch die IP-Adresse Ihres E-Mail-Servers (z. B.: 255.255.255.255).  Wenn Sie E-Mails von mehreren Domains über Marketo senden möchten, sollte Ihr IT-Team diese Zeile für jede Domain hinzufügen (in einer Zeile).`]`

`b.` Erstellen Sie für DKIM DNS-Ressourceneinträge für jede Domain, die eingerichtet werden soll. Nachfolgend finden Sie die Host-Einträge und TXT-Werte für jede Domain, die signiert werden soll: 

**`[DKIMDomain1]`**: Hosteintrag ist **`[HostRecord1]`** und der TXT-Wert ist **[TXTValue1]**.

**`[DKIMDomain2]`**: Der Host-Eintrag lautet **`[HostRecord2]`** und der TXT-Wert **`[TXTValue2]`**.

`[`Kopieren Sie den **Host-Eintrag** und den **TXT-Wert** für jede **DKIM-Domain**, die Sie eingerichtet haben, nachdem Sie die [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md) befolgt haben. Vergessen Sie nicht, jede Domain unter **Administrator > E-Mail > DKIM** zu überprüfen, nachdem Ihr IT-Team diesen Schritt abgeschlossen hat.`]`

`5)` Wir müssen sicherstellen, dass ein gültiger MX-Eintrag für unsere FROM-Domains **[FromDomain1]**, **[FromDomain2]** usw. vorhanden ist. Können Sie das bestätigen? Falls nicht, konfigurieren Sie bitte die Zuordnung zum MX-Eintrag unserer Unternehmens-Domain. Dadurch stellen wir sicher, dass Antworten/Abwesenheitsnachrichten auf unsere Marketo-E-Mails verarbeitet werden können.

Teilen Sie mir mit, wenn Sie diese Schritte abgeschlossen haben, damit ich den Einrichtungsprozess mit Marketo abschließen kann.

Vielen Dank! Sie sind großartig!

Liebe,

**`[Your Name]`**

`----------------------------------------------`

Senden Sie die E-Mail an die IT-Abteilung. Uns ist bewusst, dass es einige Zeit dauern kann, bis die IT-Abteilung diese Aufgaben abgeschlossen hat. Sie können mit Schritt 7 fortfahren, aber denken Sie daran, dass Sie zu Schritt 6 zurückkehren müssen, um die Einrichtung von Marketo abzuschließen.

## Abschließen der Marketo-Einrichtung nach Fertigstellen durch die IT-Abteilung {#complete-your-marketo-setup-after-it-finishes}

Nachdem die IT-Abteilung ihre Aufgaben abgeschlossen hat, führen Sie die folgenden Schritte aus, um Ihre Landingpage und E-Mail-CNAMEs hinzuzufügen und das Signieren mit DKIM zu aktivieren.

Navigieren Sie zum Bereich **[!UICONTROL Admin]**, um Ihren Landingpage-CNAME hinzuzufügen.

![](assets/setup-steps-15.png)

Wählen Sie „Landingpages“ aus und klicken Sie im Bereich [!UICONTROL Einstellungen] auf **[!UICONTROL Bearbeiten]**.

![](assets/setup-steps-16.png)

Geben Sie den neuen Domain-Namen in das Feld **[!UICONTROL Domänenname für Landing Pages]** ein. Dieser sollte die folgende Struktur aufweisen:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

Geben Sie im Feld **[!UICONTROL Fallback-Seite]** die URL ein, zu der Personen weitergeleitet werden sollen, wenn eine Landingpage nicht verfügbar ist. Wenn Sie über keine Fallback-Seite verfügen, können Sie die Startseite Ihres Unternehmens verwenden. Geben Sie im Feld **[!UICONTROL Startseite]** Ihre Unternehmens-Website ein.

![](assets/setup-steps-18.png)

Wählen Sie im Bereich [!UICONTROL Admin] die Option **[!UICONTROL E-Mail]** aus, um Ihren E-Mail-CNAME hinzuzufügen.

![](assets/setup-steps-19.png)

Scrollen Sie nach unten zu [!UICONTROL Branding-Domains]. Wählen Sie Ihre Domain aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

![](assets/setup-steps-20.png)

Geben Sie im Feld „Domäne“ Ihre E-Mail-Tracking-Domain ein. Diese sollte die folgende Struktur aufweisen:

`[EmailTrackingCNAME].[CompanyDomain].com`. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/setup-steps-21.png)

## Integrieren des CRM {#integrate-your-crm}

Dies ist wahrscheinlich der aufregendste Schritt Ihres Setups - es ist an der Zeit, Marketo mit all den Leads und Kontakten zu füllen, die Sie in Ihrem CRM gespeichert haben!

Wählen Sie je nach CRM, das Ihr Unternehmen verwendet, eine der folgenden Optionen aus.

    * [Integrieren von Marketo mit [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integrieren von Marketo mit [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Sie benötigen die Unterstützung der CRM-Administration Ihres Unternehmens, um diese Schritte abzuschließen.

## Hinzufügen von Trackingcode zu Ihrer Website {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Sind Sie [!DNL Launch Pack]-Kundin oder -Kunde? Dann können Sie diesen Schritt überspringen. Ihre Beraterin bzw. Ihr Berater stellt Ihnen [!DNL Munchkin]-Code-Anleitungen im Anleitungsdokument zur Einrichtung des IT-Systems zur Verfügung.

Marketo verfügt über eine benutzerdefinierte Tracking-JavaScript ([!DNL Munchkin] genannt), mit der Sie Personenaktivitäten auf jeder Web-Seite verfolgen können. [!DNL Munchkin] ist für die Integration Ihrer Website in Marketo erforderlich. Führen Sie die folgenden Schritte aus, um [Trackingcode zu Ihrer Website [!DNL Munchkin] hinzuzufügen](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Zum Hinzufügen des Trackingcodes ist Erfahrung mit HTML erforderlich.

## Erwartungen an die Leistung {#performance-expectations}

Was können Sie von Marketo hinsichtlich Leistung erwarten? Diese kann je nach Größe und Komplexität Ihrer Marketing-Kampagnen variieren. Sie können jedoch Leistung erwarten, die den Werten in der Spalte „Standard“ in mehreren Tabellen in der [Marketo Engage-Produktbeschreibung](https://helpx.adobe.com/de/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"} entsprechen. Die Spalten „Performance“ und „Performance Plus“ beziehen sich auf Leistungspakete, die [höhere Leistungsstufen](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"} bereitstellen.

Alle Einrichtungsschritte sind abgeschlossen. Das Einzige, was noch übrig ist, ist einzutauchen und Marketo zu benutzen!
