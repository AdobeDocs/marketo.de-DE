---
unique-page-id: 14352407
description: Übersicht über Versand Kanal - Marketing-Dokumente - Produktdokumentation
title: Übersicht über Versand Kanal
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Übersicht über Versand-Kanal {#delivery-channel-overview}

Wir unterteilen die drei verschiedenen Kanal, die Sie nutzen können, wie Sie sie auswählen, wann Sie sich gegenseitig aussuchen und die Nuancen um sie herum.

>[!NOTE]
>
>Diese Informationen sind nur relevant, wenn Sie Ihre E-Mails von der [Webanwendung](http://toutapp.com/login) senden. Wenn Sie Sales Connect in Gmail oder Outlook verwenden, werden Ihre E-Mails über diese E-Mail-Server gesendet.

## MSC-E-Mail-Server (Standard) {#msc-email-servers-default}

Standardmäßig wird diese Methode für den Versand Ihrer E-Mails ausgewählt. MSC-E-Mail-Server sind eine großartige Option für Benutzer, die Gmail oder Outlook nicht verwenden. Da es sich dabei um unsere Server handelt, können wir außerdem Fehlermeldungen über Absprünge oder fehlgeschlagene Versand aufnehmen und diese im Bereich &quot;Fehlgeschlagene Versand&quot;der Registerkarte &quot;Konversationen&quot;an Sie übergeben.

Ein weiterer Vorteil der Verwendung der MSC-Server ist, dass der Empfänger bei Verwendung einer [E-Mail-Identität](https://help.toutapp.com/hc/en-us/articles/215371427) die E-Mail-Adresse der von Ihnen erstellten Identität sehen kann.

Wenn Sie MSC-Server verwenden, sehen Ihre Empfänger möglicherweise das Tag &quot;via toutapp.com&quot;. Dies ist der E-Mail-Client, der ihnen mitteilt, dass die E-Mail mit Sales Connect gesendet wurde.

Weitere Informationen finden Sie in diesem [Gmail-Hilfeartikel](https://support.google.com/mail/answer/1311182?hl=en).

>[!NOTE]
>
>Unsere MSC-Server verfügen nicht über einen [DMARC-Datensatz](https://dmarc.org/), der zur Verfügung gestellt wird. Sie können nicht auf Ihren eigenen Servern in die Positivliste gesetzt werden.

## Gmail-Server {#gmail-server}

Wenn der E-Mail-Anbieter Ihrer Firma Gmail ist, können Sie Ihr bestehendes Konto nutzen, um Ihre Sales Connect-E-Mails zu senden. Dies ist eine großartige Option, wenn Sie die &quot;via toutapp.com&quot;-Informationen vermeiden möchten und wenn Sie sich lieber auf den Ruf Ihrer Firma und die Lieferbarkeit verlassen möchten. Ein weiterer Vorteil der Verwendung eines Gmail-Servers ist, dass alles, was Sie aus der Webanwendung senden, automatisch in Ihren Gmail-Ordner hinzugefügt wird.

Wir können nur ordnungsgemäß eine Verbindung mit einem einzelnen Gmail-Konto (eine E-Mail-Adresse) herstellen, das Ihre Sales Connect-E-Mails liefert. Das bedeutet, wenn Sie mehrere E-Mail-Identitäten verwenden, wird nur die Adresse des Kontos, mit dem wir verbunden sind, angezeigt, wenn Sie sich die Details ansehen.

In der Webanwendung wird Ihre Identität so angezeigt, wie Sie sie erstellt haben (oben). Beim Senden über die Gmail-Server wird jedoch die Adresse des angeschlossenen Kontos angezeigt.

>[!NOTE]
>
>Da Sales Connect Ihre Gmail-Server nicht direkt verwaltet, zeichnen wir keine abgeschnittenen E-Mail-Ereignis in der Webanwendung auf.

## Benutzerdefinierter SMTP-Server {#custom-smtp-server}

Bezahlen Sie für Ihren eigenen Server? Verwenden Sie eine Microsoft Exchange-Umgebung? Das ist eine Option für Sie. Sehen Sie sich [diese Anweisungen](http://docs.marketo.com/x/zYTS) beim Einrichten an. Wie bei Gmail-Servern, da Sales Connect Ihren Server nicht direkt verwaltet, zeichnen wir keine abgeschnittenen E-Mail-Ereignis in der Webanwendung auf.

