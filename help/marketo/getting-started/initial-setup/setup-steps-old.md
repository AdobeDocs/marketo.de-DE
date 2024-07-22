---
unique-page-id: 2949469
description: Einrichtungsschritte - Marketo-Dokumente - Produktdokumentation
title: Einrichtungsschritte
hide: true
hidefromtoc: true
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: d41a43d7579775c0c866e867f778962ff61ff044
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 0%

---

# Einrichtungsschritte {#setup-steps}

**Willkommen bei Adobe Marketo Engage!**

Bevor Sie sich mit der Verwendung von Marketo befassen, müssen Sie einige Schritte ausführen.

Zu diesen Schritten gehören:

* Grundlegende Kontoeinstellungen
* Branding von Landingpage-URLs und E-Mail-Links zur Verbesserung von Vertrauen und Zustellbarkeit
* Synchronisieren Ihres CRM
* Hinzufügen von Trackingcode zur Website Ihres Unternehmens

>[!NOTE]
>
>Sie müssen diese Schritte nur ausführen, wenn Ihr Unternehmen **neu bei Marketo** ist. Ist dies nicht der Fall, ist das Setup möglicherweise bereits abgeschlossen.

Einige Schritte erfordern Hilfe von Ihrem IT-Team.

>[!TIP]
>
>Wenn Sie [diese Checkliste ausdrucken](/help/marketo/getting-started/initial-setup/setup-checklist.md){target="_blank"}, können Sie Elemente abwählen, während Sie sie abschließen.

## Anmelden und Erstellen zusätzlicher Marketo-Benutzer {#log-in-and-create-additional-marketo-users}

>[!IMPORTANT]
>
>Wenn Ihr Marketo-Abonnement am/nach dem 31. Juli 2023 erstellt wurde oder bereits auf [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"} migriert wurde, gelten die unten beschriebenen Schritte zum Hinzufügen eines Benutzers nicht für Sie. Lesen Sie stattdessen [diesen Artikel](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"} .

Melden Sie sich bei Marketo [hier](https://app.marketo.com/){target="_blank"} mit den E-Mail-Anmeldeinformationen an, die Sie erhalten haben.

![](assets/setup-steps-1.png)

Herzlichen Glückwunsch! Sie befinden sich jetzt in Marketo und können mit der Erforschung beginnen. Möglicherweise möchten Sie Ihre Kollegen aus dem Marketing-Team einladen, sich Ihnen anzuschließen. Fügen Sie dazu neue Benutzer hinzu.

Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

>[!TIP]
>
>Während Sie hier sind, können Sie auf **[!UICONTROL Mein Konto]** klicken, um Ihre Konto- und Standorteinstellungen zu ändern und einen neuen Anmeldenamen festzulegen.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

![](assets/setup-steps-3.png)

Klicken Sie auf **[!UICONTROL Neuen Benutzer einladen]**.

![](assets/setup-steps-4.png)

Füllen Sie die E-Mail-Adresse, den Vor- und Nachnamen Ihres Kollegen aus. _Das Festlegen eines Zugriffs-Ablaufdatums ist optional_. Klicken Sie auf **[!UICONTROL Weiter]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Ein Ablaufdatum eignet sich hervorragend für kurzfristige externe Interessengruppen oder Berater, die nur für kurze Zeit Zugriff auf Marketo benötigen.

>[!NOTE]
>
>Wenn das Ablaufdatum eintrifft, erhält der Benutzer eine Ablaufbenachrichtigung und das Konto wird gesperrt.

Wählen Sie eine Rolle aus und klicken Sie auf **[!UICONTROL Weiter]**. Standardbenutzer haben Zugriff auf alle Bereiche außer Admin.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Neben den fünf integrierten Rollen können Sie auch benutzerdefinierte Rollen erstellen. Erfahren Sie mehr über [Verwalten von Benutzerrollen und Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

Sie können den Einladungstext anpassen. Klicken Sie auf **Senden**.

![](assets/setup-steps-7.png)

Der neue Benutzer wird jetzt auf der Registerkarte **[!UICONTROL Benutzer]** aufgelistet und sollte eine E-Mail mit einem Link erhalten, um ein Kennwort und eine Anmeldung zu erstellen. Nächster Schritt!

![](assets/setup-steps-8.png)

## Einrichten autorisierter Support-Kontakte {#set-up-your-authorized-support-contacts}

Möglicherweise haben Sie vom Marketo-Support eine E-Mail erhalten, in der Sie als Marketo-Support-Administrator für Ihr Unternehmen angegeben haben. Wenn ja, können Sie **autorisierte Support-Kontakte** für Ihr Team einrichten. Nur autorisierte Support-Mitarbeiter können den Marketo-Support direkt über das [Marketo Support Portal](https://support.marketo.com){target="_blank"} kontaktieren.

>[!NOTE]
>
>Die Anzahl der Support-Kontakte, die Sie erstellen können, hängt vom von Ihnen erworbenen Package ab. Diese Beschränkung wird in Ihrer E-Mail vom Marketo-Support festgelegt.

Die autorisierten Support-Kontaktdokumente wurden in die Marketo-Community verschoben. Weitere Informationen finden Sie in [diesem Artikel](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

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

Der erste (fettgedruckte) Teil ist der `[LandingPageCNAME]`. Sie werden es in Schritt 5 benötigen.

Um die Munchkin-ID abzurufen, die Sie durch Ihren Landingpage-CNAME ersetzen, gehen Sie zum Admin-Bereich.

![](assets/setup-steps-9.png)

Klicken Sie auf **Mein Konto**.

![](assets/setup-steps-10.png)

Kopieren Sie die [!UICONTROL Kontozeichenfolge] aus den Einstellungen der Landingpage.

![](assets/setup-steps-11.png)

Dies ist der `[Munchkin ID]`. Speichern Sie sie. Sie müssen es IT in Schritt 5 geben.

Konfigurieren Sie Ihre Domäneneinstellungen so, dass Landingpages die Domäne Ihres Unternehmens anstelle von Marketo verwenden (wo sie gehostet werden).

## E-Mail-Zustellbarkeit sicherstellen {#ensure-email-deliverability}

>[!NOTE]
>
>Sind Sie Launch Pack-Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen während Ihres Startaufrufs ein Dokument mit IT-Setup-Anweisungen zur Verfügung stellen.

Es gibt verschiedene Maßnahmen, die Sie ergreifen können, um sicherzustellen, dass die E-Mails möglichst viele Ihrer Personen erreichen.

* **Markieren Sie Ihre Tracking-Links**. Sie können einen CNAME auswählen, um Ihre eigene Domäne (anstelle von Marketo) in den Links zu verwenden, die Sie in E-Mails von Marketo einfügen. Dies stärkt das Domain-Branding und erhöht das Vertrauen und die Zustellbarkeit für Ihre Empfänger.
* **Fügen Sie Marketo zu Ihrer E-Mail-Zulassungsliste Ihres Unternehmens hinzu.** Es ist eine gängige Best Practice, Testadressen an Testkonten zu senden, bevor E-Mails an tatsächliche Personen gesendet werden. Durch die Zulassungsauflistung von Marketo können Sie verhindern, dass diese Test-E-Mails blockiert oder als Spam gekennzeichnet werden.
* **Richten Sie SPF und DKIM ein.** Diese Technologien garantieren Ihren Empfängern, dass Ihre Marketo-E-Mails keine Spam sind. Um zu verhindern, dass die Spam-Filter der Empfänger Ihre Marketo-E-Mails ablehnen, führen Sie die folgenden Schritte aus, um [Einrichten einer SPF und eines DKIM für die E-Mail-Zustellbarkeit](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md) durchzuführen.
* **Richten Sie einen MX-Eintrag für Ihre Domäne ein.** Ein MX-Eintrag ermöglicht es Ihnen, E-Mails an die Domain zu erhalten, von der Sie E-Mails senden, um Antworten und automatische Antworten zu verarbeiten. Wenn Sie von Ihrer Unternehmensdomäne aus senden, ist diese wahrscheinlich bereits konfiguriert. Wenn nicht, können Sie normalerweise so einrichten, dass die Zuordnung zum MX-Datensatz Ihrer Unternehmensdomäne erfolgt.
* **Empfohlene Einstellungen für die Absenderadresse.** Sie müssen in allen E-Mail-Kampagnen in der &quot;Von&quot;-Adresse eine gültige, vorhandene und funktionierende E-Mail-Domäne verwenden. Es kann von Vorteil sein, eine Subdomain Ihrer Unternehmensdomäne zu konfigurieren, anstatt sie von Ihrer Unternehmensdomäne aus zu senden. Dadurch wird sichergestellt, dass Probleme aus Ihrem Unternehmens-Mailstream keine Auswirkungen auf Ihren Marketo-Mailstream haben und umgekehrt. Darüber hinaus führt der Versand von Nachrichten von `something@nonexistentdomain.com` dazu, dass E-Mails gefiltert oder blockiert werden. Jede Domäne, die in der Absenderadresse verwendet wird, muss über ein gültiges und funktionierendes Postmaster@- und Missbrauch@-Konto verfügen.

Wenn Sie Google Apps zum Hosten Ihrer E-Mail im Unternehmen verwenden, können Sie keine E-Mails vom Typ &quot;misshandelt@&quot;oder &quot;postmaster@&quot;unter Ihrer Domäne erstellen. Um dies zu umgehen, müssen Sie Gruppen mit den Namen &quot;Missbrauch&quot;und &quot;Postmaster&quot;erstellen. Benutzer, die Mitglieder dieser Gruppen sind, erhalten E-Mails, die an diese Adressen gesendet werden (z. B. postmaster@domain.com). Detaillierte Anweisungen zum Erstellen von Gruppen finden Sie [hier](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Wählen Sie einen CNAME für E-Mail-Tracking-Links aus (wählen Sie einen aus, der _anders_ ist als der in Schritt 3 ausgewählte CNAME der Landingpage). Beispiele:

* go2.[Firmendomäne].com
* em.[Firmendomäne].com
* Wow.[Firmendomäne].com

Der erste Teil ist der E-Mail-Tracking-CNAME `[EmailTrackingCNAME]`. Sie müssen es IT in Schritt 5 geben.

>[!CAUTION]
>
>E-Mail- und Landingpage-CNAMEs müssen unterschiedlich sein. Vermeiden Sie außerdem CNAMEs wie &quot;track&quot;oder &quot;link&quot;. Er wird oft als Spam gekennzeichnet

Um Ihren Marketo-Tracking-Link zu finden, gehen Sie zum Bereich **[!UICONTROL Admin]** .

![](assets/setup-steps-12.png)

Klicken Sie auf **[!UICONTROL E-Mail]**.

![](assets/setup-steps-13.png)

Kopieren Sie den [!UICONTROL Tracking-Link] aus Ihren E-Mail-Einstellungen.

Der [!UICONTROL Tracking-Link] hat folgendes Format: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Dies ist Ihr `[MktoTrackingLink]`. Speichern Sie sie. Sie müssen es IT in Schritt 5 geben.

Erfassen Sie &quot;Von&quot;-Domänen. Erstellen Sie eine Liste aller &quot;Von&quot;-Domänen (wie in &quot;`[Sender]@[FromDomain].com`&quot;), die Sie zum Senden von E-Mails aus Marketo verwenden möchten. Für die meisten gibt es nur einen.

Beispiel: &quot;marketo.com,&quot;&quot;info.marketo.com,&quot;. Dies sind `[FromDomain1]`, `[FromDomain2]` usw. Speichern Sie sie. Sie müssen sie in Schritt 5 IT übergeben.

Sie haben jetzt alle Informationen, die Sie benötigen, um Ihre Anfrage an IT zu senden!

## IT bitten, Protokolle zu konfigurieren {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Sind Sie Launch Pack-Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen während Ihres Startaufrufs ein Dokument mit IT-Setup-Anweisungen zur Verfügung stellen.

Sobald Sie alle erforderlichen Informationen gesammelt haben, können Sie eine Anfrage an die IT senden. Sie können den unten stehenden Text als Vorlage verwenden und den fett gedruckten Text durch Ihre eigenen Informationen ersetzen.

[Fügen Sie einen Link zu diesem Artikel ein](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Fügen Sie diesen Text in die E-Mail ein und ersetzen Sie die fett hervorgehobenen Platzhalter:

>[!NOTE]
>
>Informationen zum Ersetzen der Platzhalter finden Sie in den Schritten 3 und 4 oben. Beachten Sie, dass `[LandingPageCNAME]` und `[EmailTrackingCNAME]` unterschiedlich sein müssen.

`----------------------------------------------`

Sehr geehrter IT-Administrator,

Unser Marketingteam verwendet jetzt die Marketo-Plattform, um mit unseren Mitarbeitern zu kommunizieren. Um eine großartige Zustellbarkeit der E-Mail zu gewährleisten, müssen wir folgende Änderungen vornehmen:

`1)` Fügen Sie für unsere Landingpages einen DNS-Eintrag (CNAME) für **[LandingPageCNAME]** hinzu.**[CompanyDomain]**.com, die auf **[Munchkin ID]**.mktoweb.com verweist.

`2)` Fügen Sie für unsere Tracking-Links in der E-Mail einen DNS-Eintrag (CNAME) für **[EmailTrackingCNAME]** hinzu.**[CompanyDomain]**.com, die auf **[MktoTrackingLink]** verweist.

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

    * Wenn unser Anti-Spam-System &quot;Von Domänen&quot;verwendet, fügen Sie Folgendes hinzu:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Wir müssen SPF und DKIM einrichten, damit Marketo berechtigt ist, signierte E-Mails in unserem Namen zu senden.

`a.` Um SPF einzurichten, fügen Sie bitte unseren DNS-Einträgen die folgende Zeile hinzu:

IN TXT **[From Domain]**: v=spf1 mx ip4:**[Corporate IP(s)]**
<br/>include: mktomail.com ~all

Wenn wir bereits einen vorhandenen SPF-Eintrag in unserem DNS-Eintrag haben, fügen Sie einfach Folgendes hinzu:

include:mktomail.com

`[`Ersetzen Sie **Von Domäne** durch Ihre E-Mail-Adresse von Domäne (z. B. company.com) und **CorpIP** durch die IP-Adresse Ihres E-Mail-Servers im Unternehmen (z. B.: 255.255.255).  Wenn Sie E-Mails von mehreren Domänen über Marketo senden möchten, sollten Ihre IT-Mitarbeiter diese Zeile für jede Domäne hinzufügen (in einer Zeile).`]`

`b.` Für DKIM erstellen Sie bitte DNS-Ressourcendatensätze für jede Domäne, die wir einrichten möchten. Im Folgenden finden Sie die Hostdatensätze und TXT-Werte für jede Domäne, für die wir Signieren werden:

**`[DKIMDomain1]`**: Host-Datensatz ist **`[HostRecord1]`** und der TXT-Wert ist **[TXTValue1]**.

**`[DKIMDomain2]`**: Host-Eintrag ist **`[HostRecord2]`** und der TXT-Wert ist **`[TXTValue2]`**.

`[`Kopieren Sie den **HostRecord** und den **TXTValue** für jeden **DKIMDomain**, den Sie eingerichtet haben, nachdem Sie die [Anweisungen hier](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md) befolgt haben. Vergessen Sie nicht, jede Domäne unter **Admin > E-Mail > DKIM** zu überprüfen, nachdem Ihre IT-Mitarbeiter diesen Schritt abgeschlossen haben.`]`

`5)` Wir müssen sicherstellen, dass ein gültiger MX-Eintrag für unsere FROM-Domänen **[FromDomain1]**, **[FromDomain2]** usw. vorhanden ist. Können Sie das bestätigen? Wenn nicht, konfigurieren Sie bitte, um der Unternehmensdomäne MX-Datensatz zuzuordnen. Dadurch wird sichergestellt, dass wir Antworten/Autoreaktoren auf unsere Marketo Mailings verarbeiten können.

Teilen Sie mir mit, wenn Sie diese Schritte ausgeführt haben, damit ich den Einrichtungsprozess mit Marketo abschließen kann.

Danke! Du bist der Beste!

Liebe,

**`[Your Name]`**

`----------------------------------------------`

Senden Sie die E-Mail an IT. Wir wissen, dass es einige Zeit dauern kann, bis IT diese Aufgaben erledigt. Sie können mit Schritt 7 fortfahren. Denken Sie jedoch daran, dass Sie Schritt 6 zurückgeben müssen, um Ihre Marketo-Einrichtung abzuschließen.

## Abschluss der Marketo-Einrichtung nach Abschluss der IT {#complete-your-marketo-setup-after-it-finishes}

Nachdem die IT-Abteilung ihre Aufgaben abgeschlossen hat, führen Sie die folgenden Schritte aus, um Ihre Landingpage und E-Mail-CNAMEs hinzuzufügen und die DKIM-Signatur zu aktivieren.

Navigieren Sie zum Bereich **[!UICONTROL Admin]** , um den CNAME Ihrer Landingpage hinzuzufügen.

![](assets/setup-steps-15.png)

Wählen Sie Landingpages aus und klicken Sie im Bereich [!UICONTROL Einstellungen] auf **[!UICONTROL Bearbeiten]** .

![](assets/setup-steps-16.png)

Geben Sie Ihren neuen Domänennamen in das Feld **[!UICONTROL Domänenname für Einstiegsseiten]** ein. Dies sollte folgende Form aufweisen:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

Geben Sie im Feld **[!UICONTROL Fallback]** die URL ein, zu der Personen wechseln sollen, wenn eine Landingpage nicht verfügbar ist. Wenn Sie keine Fallback-Seite haben, können Sie die Startseite Ihres Unternehmens verwenden. Geben Sie im Feld **[!UICONTROL Homepage]** Ihre Firmenwebsite ein.

![](assets/setup-steps-18.png)

Wählen Sie im Bereich [!UICONTROL Admin] die Option **[!UICONTROL E-Mail]** aus, um Ihren E-Mail-CNAME hinzuzufügen.

![](assets/setup-steps-19.png)

Scrollen Sie nach unten zu [!UICONTROL Branding Domains]. Wählen Sie Ihre Domäne aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

![](assets/setup-steps-20.png)

Geben Sie im Feld Domäne Ihre E-Mail-Tracking-Domäne ein. Dies sollte folgende Form aufweisen:

`[EmailTrackingCNAME].[CompanyDomain].com`. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/setup-steps-21.png)

## CRM integrieren {#integrate-your-crm}

Dies ist wahrscheinlich der aufregendste Schritt Ihres Setups - es ist an der Zeit, Marketo mit all den Leads und Kontakten zu füllen, die Sie in Ihrem CRM-System gespeichert haben!

Wählen Sie je nach dem CRM-System, das Ihr Unternehmen verwendet, eine der folgenden Optionen aus:

    * [Integrieren von Marketo mit  [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integrieren von Marketo mit  [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Sie benötigen die Unterstützung des CRM-Administrators Ihres Unternehmens, um diese Schritte durchzuführen.

## Hinzufügen von Trackingcode zu Ihrer Website {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Sind Sie ein [!DNL Launch Pack] -Kunde? Sie können diesen Schritt überspringen. Ihr Berater stellt Ihnen im Dokument mit den IT-Setup-Anweisungen [!DNL Munchkin] Code-Anweisungen zur Verfügung.

Marketo verfügt über eine benutzerdefinierte Tracking-JavaScript (namens [!DNL Munchkin]), mit der Sie Personenaktivitäten auf jeder Webseite verfolgen können. [!DNL Munchkin] ist zur Integration Ihrer Website in Marketo erforderlich. Führen Sie die folgenden Schritte aus, um [Trackingcode für  [!DNL Munchkin] zu Ihrer Website hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Erlebnis mit HTML erforderlich, um den Trackingcode hinzuzufügen.

## Leistungserwartungen {#performance-expectations}

Was ist mit der Leistung von Marketo zu erwarten? Diese kann je nach Größe und Komplexität Ihrer Marketing-Kampagnen variieren. Sie können jedoch Leistungsstufen erwarten, die dem entsprechen, was in der Spalte &quot;Standard&quot;in mehreren Tabellen in der [Marketo Engage-Produktbeschreibung](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"} beschrieben ist. Die Spalten &quot;Leistung&quot;und &quot;Leistung Plus&quot;beziehen sich auf Leistungs-Tier-Pakete, die [höhere Leistungsstufen bereitstellen](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Alle Einrichtungsschritte sind vorbei. Das Einzige, was noch übrig ist, ist in Marketo zu tauchen und zu benutzen!
