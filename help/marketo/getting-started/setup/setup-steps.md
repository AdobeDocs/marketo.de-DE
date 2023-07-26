---
unique-page-id: 2949469
description: Einrichtungsschritte - Marketo-Dokumente - Produktdokumentation
title: Einrichtungsschritte
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 0%

---

# Einrichtungsschritte {#setup-steps}

**Willkommen bei Marketo Engage!**

Bevor Sie sich mit der Verwendung von Marketo befassen, müssen Sie einige Schritte ausführen.

Zu diesen Schritten gehören:

* Grundlegende Kontoeinstellungen
* Branding von Landingpage-URLs und E-Mail-Links zur Verbesserung von Vertrauen und Zustellbarkeit
* Synchronisieren Ihres CRM
* Hinzufügen von Trackingcode zur Website Ihres Unternehmens

>[!NOTE]
>
>Sie müssen diese Schritte nur ausführen, wenn Ihr Unternehmen **neu in Marketo**. Ist dies nicht der Fall, ist das Setup möglicherweise bereits abgeschlossen.

Einige Schritte erfordern Hilfe von Ihrem IT-Team.

>[!TIP]
>
>Wenn Sie [Diese Checkliste ausdrucken](/help/marketo/getting-started/setup/setup-checklist.md){target="_blank"}, können Sie die Elemente bei ihrem Abschluss abwählen.

## Anmelden und Erstellen zusätzlicher Marketo-Benutzer {#log-in-and-create-additional-marketo-users}

Bei Marketo anmelden [here](https://app.marketo.com/){target="_blank"} die Anmeldedaten verwenden, die Sie per E-Mail erhalten haben.

![](assets/setup-steps-1.png)

Herzlichen Glückwunsch! Sie befinden sich jetzt in Marketo und können mit der Erforschung beginnen. Möglicherweise möchten Sie Ihre Kollegen aus dem Marketing-Team einladen, sich Ihnen anzuschließen. Fügen Sie dazu neue Benutzer hinzu.

Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

>[!TIP]
>
>Wenn Sie hier sind, können Sie auf **[!UICONTROL Mein Konto]** , um Ihre Konto- und Standorteinstellungen zu ändern und einen neuen Anmeldenamen festzulegen.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Klicks **[!UICONTROL Benutzer und Rollen]**.

![](assets/setup-steps-3.png)

Klicks **[!UICONTROL Neuen Benutzer einladen]**.

![](assets/setup-steps-4.png)

Füllen Sie die E-Mail-Adresse, den Vor- und Nachnamen Ihres Kollegen aus. _Das Festlegen des Ablaufdatums für den Zugriff ist optional._. Klicks **[!UICONTROL Nächste]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Ein Ablaufdatum eignet sich hervorragend für kurzfristige externe Interessengruppen oder Berater, die nur für kurze Zeit Zugriff auf Marketo benötigen.

>[!NOTE]
>
>Wenn das Ablaufdatum eintrifft, erhält der Benutzer eine Ablaufbenachrichtigung und das Konto wird gesperrt.

Rollen auswählen und auf **[!UICONTROL Nächste]**. Standardbenutzer haben Zugriff auf alle Bereiche außer Admin.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Neben den fünf integrierten Rollen können Sie auch benutzerdefinierte Rollen erstellen. Weitere Informationen [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

Sie können den Einladungstext anpassen. Klicks **Senden**.

![](assets/setup-steps-7.png)

Der neue Benutzer wird jetzt im **[!UICONTROL Benutzer]** und sollte eine E-Mail mit einem Link erhalten, um ein Kennwort und eine Anmeldung zu erstellen. Nächster Schritt!

![](assets/setup-steps-8.png)

## Einrichten autorisierter Support-Kontakte {#set-up-your-authorized-support-contacts}

Möglicherweise haben Sie vom Marketo-Support eine E-Mail erhalten, in der Sie als Marketo-Support-Administrator für Ihr Unternehmen angegeben haben. Wenn ja, können Sie **autorisierte Support-Kontakte** für Ihr Team. Nur autorisierte Supportkontakte können den Marketo-Kundensupport direkt über die [Marketo Support Portal](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>Die Anzahl der Support-Kontakte, die Sie erstellen können, hängt vom von Ihnen erworbenen Package ab. Diese Beschränkung wird in Ihrer E-Mail vom Marketo-Support festgelegt.

Die autorisierten Support-Kontaktdokumente wurden in die Marketo-Community verschoben. Siehe [diesem Artikel](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

>[!NOTE]
>
>Nur Personen, die sich bei der Marketo-Community angemeldet haben, werden in der Liste angezeigt. Wenn Sie die Person nicht finden können, müssen Sie sich zuerst bei der Community anmelden.

## Anpassen der Landingpage-URLs mit einem CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Sind Sie Launch Pack-Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen während Ihres Startaufrufs ein Dokument mit IT-Setup-Anweisungen zur Verfügung stellen.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Wählen Sie einen CNAME für Ihre Landingpages aus. Beispiele:

    * **go**.[Unternehmensdomäne].com
    * **www2**.[Unternehmensdomäne].com
    * **lp**.[Unternehmensdomäne].com

>[!TIP]
>
>Halten Sie es kurz! Kürzere URLs sind leichter zu merken. Wir empfehlen &quot;go&quot; als Domäne.

Der erste fettgedruckte Teil ist der `[LandingPageCNAME]`. Sie werden es in Schritt 5 benötigen.

Um die Munchkin-ID abzurufen, die Sie durch Ihren Landingpage-CNAME ersetzen, gehen Sie zum Admin-Bereich.

![](assets/setup-steps-9.png)

Klicks **Mein Konto**.

![](assets/setup-steps-10.png)

Kopieren Sie die [!UICONTROL Kontozeichenfolge] aus den Landingpage-Einstellungen.

![](assets/setup-steps-11.png)

Dies ist die `[Munchkin ID]`. Speichern Sie sie. Sie müssen es IT in Schritt 5 geben.

Konfigurieren Sie Ihre Domäneneinstellungen so, dass Landingpages die Domäne Ihres Unternehmens anstelle von Marketo verwenden (wo sie gehostet werden).

## E-Mail-Zustellbarkeit sicherstellen {#ensure-email-deliverability}

>[!NOTE]
>
>Sind Sie Launch Pack-Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen während Ihres Startaufrufs ein Dokument mit IT-Setup-Anweisungen zur Verfügung stellen.

Es gibt verschiedene Maßnahmen, mit denen Sie sicherstellen können, dass die E-Mails möglichst viele Ihrer Personen erreichen.

* **Markieren von Tracking-Links**. Sie können einen CNAME auswählen, um Ihre eigene Domäne (anstelle von Marketo) in den Links zu verwenden, die Sie in E-Mails von Marketo einfügen. Dies stärkt das Domain-Branding und erhöht das Vertrauen und die Zustellbarkeit für Ihre Empfänger.
* **Fügen Sie Marketo zu Ihrer E-Mail-Zulassungsliste Ihres Unternehmens hinzu.** Es ist eine gängige Best Practice, vor dem Versand von E-Mails an Personen Testversand an Testkonten durchzuführen. Durch die Zulassungsauflistung von Marketo können Sie verhindern, dass diese Test-E-Mails blockiert oder als Spam gekennzeichnet werden.
* **Einrichten von SPF und DKIM.** Mit diesen Technologien können Sie Ihren Empfängern versichern, dass Ihre Marketo-E-Mails keine Spam sind. Um zu verhindern, dass die Spamfilter der Empfänger Ihre Marketo-E-Mails ablehnen, gehen Sie wie folgt vor: [Einrichten einer SPF und eines DKIM für Ihre E-Mail-Zustellbarkeit](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Richten Sie einen MX-Datensatz für Ihre Domäne ein.** Ein MX-Datensatz ermöglicht es Ihnen, E-Mails an die Domain zu erhalten, von der Sie E-Mails senden, um Antworten und automatische Antworten zu verarbeiten. Wenn Sie von Ihrer Unternehmensdomäne aus senden, ist diese wahrscheinlich bereits konfiguriert. Wenn nicht, können Sie normalerweise so einrichten, dass die Zuordnung zum MX-Datensatz Ihrer Unternehmensdomäne erfolgt.
* **Empfohlene Einstellungen für die Absenderadresse.** Sie müssen in allen E-Mail-Kampagnen in der Absenderadresse eine gültige, vorhandene und funktionierende E-Mail-Domäne verwenden. Es kann von Vorteil sein, eine Subdomain Ihrer Unternehmensdomäne zu konfigurieren, anstatt sie von Ihrer Unternehmensdomäne aus zu senden. Dadurch wird sichergestellt, dass Probleme aus Ihrem Unternehmens-Mailstream keine Auswirkungen auf Ihren Marketo-Mailstream haben und umgekehrt. Darüber hinaus senden Sie E-Mails von `something@nonexistentdomain.com` wird E-Mail gefiltert oder blockiert. Jede Domäne, die in der Absenderadresse verwendet wird, muss über ein gültiges und funktionierendes Postmaster@- und Missbrauch@-Konto verfügen.

Wenn Sie Google Apps zum Hosten Ihrer E-Mail im Unternehmen verwenden, können Sie keine E-Mails vom Typ &quot;misshandelt@&quot;oder &quot;postmaster@&quot;unter Ihrer Domäne erstellen. Um dies zu umgehen, müssen Sie Gruppen mit den Namen &quot;Missbrauch&quot;und &quot;Postmaster&quot;erstellen. Benutzer, die Mitglieder dieser Gruppen sind, erhalten E-Mails, die an diese Adressen gesendet werden (z. B. postmaster@domain.com). Detaillierte Anweisungen zum Erstellen von Gruppen finden Sie unter [here](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Wählen Sie einen CNAME für E-Mail-Tracking-Links aus (wählen Sie einen aus, der _distinct_ aus dem in Schritt 3 ausgewählten CNAME der Landingpage). Beispiele:

* go2.[CompanyDomain].com
* em.[CompanyDomain].com
* Wow.[CompanyDomain].com

Der erste Teil ist der E-Mail-Tracking-CNAME, `[EmailTrackingCNAME]`. Sie müssen es IT in Schritt 5 geben.

>[!CAUTION]
>
>E-Mail- und Landingpage-CNAMEs müssen unterschiedlich sein. Vermeiden Sie außerdem CNAMEs wie &quot;track&quot;oder &quot;link&quot;. Er wird oft als Spam gekennzeichnet

Um Ihren Marketo-Tracking-Link zu finden, navigieren Sie zum **[!UICONTROL Admin]** Bereich.

![](assets/setup-steps-12.png)

Klicks **[!UICONTROL Email]**.

![](assets/setup-steps-13.png)

Kopieren Sie die [!UICONTROL Tracking-Link] aus Ihren E-Mail-Einstellungen.

Die [!UICONTROL Tracking-Link] im Formular: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Dies ist Ihr `[MktoTrackingLink]`. Speichern Sie sie. Sie müssen es IT in Schritt 5 geben.

Erfassen Sie &quot;Von&quot;-Domänen. Erstellen Sie eine Liste aller &quot;Von&quot;-Domänen (wie in, `[Sender]@[FromDomain].com`), die Sie zum Senden von E-Mails aus Marketo verwenden möchten. Für die meisten gibt es nur einen.

Beispiel: &quot;marketo.com,&quot;&quot;info.marketo.com,&quot;. Diese `[FromDomain1]`,`[FromDomain2]`, usw. Speichern Sie sie. Sie müssen sie in Schritt 5 IT übergeben.

Sie haben jetzt alle Informationen, die Sie benötigen, um Ihre Anfrage an IT zu senden!

## IT bitten, Protokolle zu konfigurieren {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Sind Sie Launch Pack-Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen während Ihres Startaufrufs ein Dokument mit IT-Setup-Anweisungen zur Verfügung stellen.

Sobald Sie alle erforderlichen Informationen gesammelt haben, können Sie eine Anfrage an die IT senden. Sie können den unten stehenden Text als Vorlage verwenden und den fett gedruckten Text durch Ihre eigenen Informationen ersetzen.

[Link zu diesem Artikel einschließen](/help/marketo/getting-started/setup/configure-protocols-for-marketo.md).

Fügen Sie diesen Text in die E-Mail ein und ersetzen Sie die fett hervorgehobenen Platzhalter:

>[!NOTE]
>
>Informationen zum Ersetzen der Platzhalter finden Sie in den Schritten 3 und 4 oben. Beachten Sie Folgendes: `[LandingPageCNAME]` und `[EmailTrackingCNAME]` muss anders sein.

`----------------------------------------------`

Sehr geehrter IT-Administrator,

Unser Marketingteam verwendet jetzt die Marketo-Plattform, um mit unseren Mitarbeitern zu kommunizieren. Um eine großartige Zustellbarkeit der E-Mail zu gewährleisten, müssen wir folgende Änderungen vornehmen:

`1)` Fügen Sie für unsere Landingpages einen DNS-Eintrag (CNAME) hinzu für **[LandingPageCNAME]**.**[CompanyDomain]**.com, auf **[Munchkin-ID]**.mktoweb.com

`2)` Fügen Sie für unsere Tracking-Links in E-Mails einen DNS-Eintrag (CNAME) hinzu für **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, auf **[MktoTrackingLink]**.

`3)` Zulassungsliste Marketo.

    * Wenn wir IP-Adressen in unserer E-Mail-Zulassungsliste verwenden, fügen Sie die unten aufgeführten IPs hinzu:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

>[!NOTE]
>
>Wenden Sie sich an den Marketo-Support , wenn Sie eine gekürzte Liste von IPs für eine spezifische Zulassungsliste Ihrer Umgebung wünschen.

    * Wenn unser Anti-Spam-System Von Domänen verwendet, fügen Sie Folgendes hinzu:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Wir müssen SPF und DKIM einrichten, damit Marketo signierte E-Mails in unserem Namen versenden kann.

`a.` Um SPF einzurichten, fügen Sie bitte unseren DNS-Einträgen die folgende Zeile hinzu:

IN TXT **[Von Domäne]**: v=spf1 mx ip4:**[Firmen-IPs]**
<br/>include: mktomail.com ~all

Wenn wir bereits einen vorhandenen SPF-Eintrag in unserem DNS-Eintrag haben, fügen Sie einfach Folgendes hinzu:

include:mktomail.com

`[`Ersetzen **Von Domäne** mit Ihrer E-Mail von der Domäne (z. B.: company.com) und **CorpIP** mit der IP-Adresse Ihres Unternehmens-E-Mail-Servers (z. B.: 255.255.255).  Wenn Sie E-Mails von mehreren Domänen über Marketo versenden möchten, sollten Ihre IT-Mitarbeiter diese Zeile für jede Domäne hinzufügen (in einer Zeile).`]`

`b.` Erstellen Sie für DKIM DNS-Ressourcendatensätze für jede Domäne, die wir einrichten möchten. Im Folgenden finden Sie die Hostdatensätze und TXT-Werte für jede Domäne, für die wir Signieren werden:

**`[DKIMDomain1]`**: Hostdatensatz ist **`[HostRecord1]`** und der TXT-Wert **[TXTValue1]**.

**`[DKIMDomain2]`**: Hostdatensatz ist **`[HostRecord2]`** und der TXT-Wert **`[TXTValue2]`**.

`[`Kopieren Sie die **HostRecord** und **TXTValue** für jeden **DKIMDomain** Sie haben sich eingerichtet, nachdem Sie die [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Vergessen Sie nicht, jede Domäne in zu überprüfen. **Admin > E-Mail > DKIM** nachdem Ihr IT-Personal diesen Schritt abgeschlossen hat.`]`

`5)` Wir müssen sicherstellen, dass es einen gültigen MX-Eintrag für unsere FROM-Domänen gibt. **[FromDomain1]**, **[FromDomain2]**, usw. Können Sie das bestätigen? Wenn nicht, konfigurieren Sie bitte, um der Unternehmensdomäne MX-Datensatz zuzuordnen. Dadurch wird sichergestellt, dass wir Antworten/Autoreaktoren auf unsere Marketo Mailings verarbeiten können.

Teilen Sie mir mit, wenn Sie diese Schritte ausgeführt haben, damit ich den Einrichtungsprozess mit Marketo abschließen kann.

Vielen Dank! Du bist der Beste!

Liebe,

**`[Your Name]`**

`----------------------------------------------`

Senden Sie die E-Mail an IT. Wir wissen, dass es einige Zeit dauern kann, bis IT diese Aufgaben erledigt. Sie können mit Schritt 7 fortfahren. Denken Sie jedoch daran, dass Sie Schritt 6 zurückgeben müssen, um Ihre Marketo-Einrichtung abzuschließen.

## Abschluss der Marketo-Einrichtung nach Abschluss der IT {#complete-your-marketo-setup-after-it-finishes}

Nachdem die IT-Abteilung ihre Aufgaben abgeschlossen hat, führen Sie die folgenden Schritte aus, um Ihre Landingpage und E-Mail-CNAMEs hinzuzufügen und die DKIM-Signatur zu aktivieren.

Navigieren Sie zu **[!UICONTROL Admin]** Bereich zum Hinzufügen des CNAME Ihrer Landingpage

![](assets/setup-steps-15.png)

Wählen Sie Einstiegsseiten aus und klicken Sie auf **[!UICONTROL Bearbeiten]** im [!UICONTROL Einstellungen] Bereich.

![](assets/setup-steps-16.png)

Geben Sie Ihren neuen Domänennamen in das Feld ein. **[!UICONTROL Domänenname für Einstiegsseiten]**. Dies sollte folgende Form aufweisen:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

Im **[!UICONTROL Fallback]** -Seite, geben Sie die URL ein, zu der Personen wechseln sollen, wenn eine Landingpage nicht verfügbar ist. Wenn Sie keine Fallback-Seite haben, können Sie die Startseite Ihres Unternehmens verwenden. Im **[!UICONTROL Homepage]** eingeben, geben Sie Ihre Firmenwebsite ein.

![](assets/setup-steps-18.png)

Im [!UICONTROL Admin] Bereich, auswählen **[!UICONTROL Email]** Hinzufügen des E-Mail-CNAME

![](assets/setup-steps-19.png)

Nach unten scrollen zu [!UICONTROL Branding-Domänen]. Wählen Sie Ihre Domäne aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

![](assets/setup-steps-20.png)

Geben Sie im Feld Domäne Ihre E-Mail-Tracking-Domäne ein. Dies sollte folgende Form aufweisen:

`[EmailTrackingCNAME].[CompanyDomain].com`. Klicks **[!UICONTROL Speichern]**.

![](assets/setup-steps-21.png)

## CRM integrieren {#integrate-your-crm}

Dies ist wahrscheinlich der aufregendste Schritt Ihres Setups - es ist an der Zeit, Marketo mit all den Leads und Kontakten zu füllen, die Sie in Ihrem CRM-System gespeichert haben!

Wählen Sie je nach dem CRM-System, das Ihr Unternehmen verwendet, eine der folgenden Optionen aus:

    * [Integrieren von Marketo mit [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integrieren von Marketo mit [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Sie benötigen die Unterstützung des CRM-Administrators Ihres Unternehmens, um diese Schritte durchzuführen.

## Hinzufügen von Trackingcode zu Ihrer Website {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Bist du ein [!DNL Launch Pack] Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen mit [!DNL Munchkin] Code-Anweisungen in Ihrem Dokument mit IT-Setup-Anweisungen.

Marketo verfügt über benutzerdefiniertes Tracking-JavaScript (namens [!DNL Munchkin]), mit dem Sie Personenaktivitäten auf jeder Webseite verfolgen können. [!DNL Munchkin] ist erforderlich, um Ihre Website in Marketo zu integrieren. Führen Sie die folgenden Schritte aus, um [Hinzufügen [!DNL Munchkin] Trackingcode auf Ihrer Website](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Erlebnis mit HTML erforderlich, um den Trackingcode hinzuzufügen.

## Leistungserwartungen {#performance-expectations}

Was ist mit der Leistung von Marketo zu erwarten? Diese kann je nach Größe und Komplexität Ihrer Marketing-Kampagnen variieren. Sie können jedoch Leistungsstufen erwarten, die dem entsprechen, was in der Spalte &quot;Standard&quot;in mehreren Tabellen im Abschnitt [Marketo Engage-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. The "Performance" and "Performance Plus" columns refer to performance tier packages that provide [higher performance levels](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Alle Einrichtungsschritte sind vorbei. Das Einzige, was noch übrig ist, ist in Marketo zu tauchen und zu benutzen!
