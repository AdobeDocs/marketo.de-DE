---
unique-page-id: 2360219
description: Einrichten einer benutzerdefinierten DKIM-Signatur - Marketo-Dokumente - Produktdokumentation
title: Einrichten einer benutzerdefinierten DKIM-Signatur
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# Einrichten einer benutzerdefinierten DKIM-Signatur {#set-up-a-custom-dkim-signature}

Um eine erstklassige Zustellbarkeit zu gewährleisten, signieren wir automatisch alle ausgehenden E-Mails mit einer freigegebenen Marketo DKIM-Signatur.

>[!NOTE]
>
>Möglicherweise benötigen Sie die Hilfe Ihres IT-Teams, um einige der Schritte in diesem Artikel auszuführen.

Sie können die DKIM-Signatur personalisieren, um die Domain(s) Ihrer Wahl widerzuspiegeln. So geht&#39;s.

1. Navigieren Sie zum Abschnitt **[!UICONTROL Admin]**.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Wenn Sie eine benutzerdefinierte DKIM-Signatur auf altmodische Weise einrichten, funktioniert sie weiterhin und sollte hier angezeigt werden.

1. Klicken Sie auf **E-Mail**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Klicken Sie auf die **SPF/DKIM** und dann auf **Domain hinzufügen**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Geben Sie als Absenderadresse die Domain ein, die Sie in Marketo-E-Mails verwenden werden. Wählen Sie einen Selektor und eine Schlüsselgröße aus. Klicken Sie abschließend **Hinzufügen**.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   <table>
   <tr>
   <td width="20%"><b>Selektor</b></td>
   <td>Eine eindeutige Zeichenfolge/Kennung, die verwendet wird, um den öffentlichen Schlüsselteil des DKIM-Eintrags zu finden. Es kann sich um eine beliebige Zeichenfolge oder eine eindeutige Kennung handeln, um den Zweck dieses DKIM-Schlüssels/Datensatzes zu trennen und zu identifizieren.</td>
   </tr>
   <tr>
   <td width="20%"><b>Schlüsselgröße</b></td>
   <td>Die Sicherheitsstufe, mit der Ihre DKIM-Signatur verschlüsselt werden soll.</td>
   </tr>
   </tbody>
   </table>

   <p>

   >[!TIP]
   >
   >* Wir empfehlen eine Schlüsselgröße von 2048.
   >* Wenn Sie in Ihrer Absenderadresse eine andere Domain verwenden, verwenden wir die von Marketo freigegebene DKIM-Signatur.

   >[!IMPORTANT]
   >
   >Wenn Sie entweder den DKIM-Selektor oder die DKIM-Verschlüsselungsgröße für Ihre Domain aktualisieren müssen, müssen Sie den vorhandenen Eintrag löschen und den neu generierten Eintrag mit den neuen Werten erneut veröffentlichen.
   >
   >Beachten Sie dabei, dass DKIM erst dann für Ihre Domain signiert wird, wenn Ihr neuer Eintrag veröffentlicht und von unserem System validiert wurde. Planen Sie Ihre Änderung entsprechend, da es 24 bis 48 Stunden dauern kann, bis der neue DKIM-Eintrag vollständig über das Internet verbreitet wird.

1. Senden Sie den **[!UICONTROL Hosteintrag]** und den **[!UICONTROL TXT-Wert]** an Ihre IT. Bitten Sie sie, den Eintrag für Sie zu erstellen, und stellen Sie sicher, dass er an alle Nameserver weitergegeben wird, die mit der Formular-Domain verknüpft sind. Die DKIM-Überprüfung von Marketo erfordert, dass der DKIM-Schlüssel an alle Nameserver weitergegeben wird, die mit der Domain verknüpft sind, die DKIM-signiert wird.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Sobald sie bestätigen, dass sie den Eintrag erstellt haben, kehren sie zu Marketo zurück, wählen Ihre Domain aus und klicken auf **[!UICONTROL DNS überprüfen]**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Wenn die Bestätigung fehlschlägt und Ihre IT den Eintrag korrekt erstellt hat, kann es sich um eine DNS-Übertragung handeln. Versuchen Sie es später erneut.

   >[!CAUTION]
   >
   >Das Ändern/Entfernen des entsprechenden DNS-Eintrags beeinträchtigt die Zustellbarkeit. Stellen Sie sicher, dass Sie den Eintrag in Marketo löschen, bevor Sie DNS-Änderungen vornehmen.

   Dies wird absolut bei der Zustellbarkeit Ihrer E-Mails helfen. Sie sollten überprüfen lassen, ob der Datensatz vorhanden und korrekt ist.
