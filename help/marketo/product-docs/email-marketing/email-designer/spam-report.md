---
solution: Marketo Engage
product: marketo
title: Spam-Attentäter
description: Erfahren Sie, wie Sie mit SpamAssassin Ihren E-Mail-Inhalt testen und die Wahrscheinlichkeit sehen können, dass er als Spam gekennzeichnet wird.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
exl-id: 6954850e-2b1a-4bf5-b918-1c54d6926b7e
source-git-commit: d13bf2943f493579f75fe8c9a0c3f675f74a09f0
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 7%

---

# Spam-Attentäter {#spam-assassin}

Mit SpamAssassin in Marketo Engage können Sie Ihren E-Mail-Inhalt testen und die Wahrscheinlichkeit sehen, dass ISPs/Postfachanbieter ihn als Spam markieren.

SpamAssassin analysiert Ihre Inhalte und weist eine Bewertung anhand verschiedener Kriterien zu. Dabei gilt: Je niedriger der Wert, desto besser. Es ist wichtig, einen niedrigen Wert beizubehalten, da sich der Versand von E-Mails mit einem hohen Wert negativ auf die Zustellbarkeit insgesamt auswirken kann.

## Zugriff auf den Spam-Bericht {#access-the-spam-report}

1. Klicken Sie auf dem Bildschirm Simulieren auf die Schaltfläche **Spam-Bericht**.

SCREENSHOT

1. Ein Spam-Bericht wird generiert.

SCREENSHOT

1. Überprüfen Sie die Bewertungen und Beschreibungen für jedes Element.

>[!IMPORTANT]
>
>Wenn die Gesamtpunktzahl höher als 5 ist, wird Ihre E-Mail bei der Zustellung möglicherweise blockiert oder als Spam gekennzeichnet.

1. Wenn Sie die Punktzahl für zu hoch halten, bearbeiten Sie den Inhalt in der E-Mail-Designer und führen Sie den Spam-Bericht erneut aus, bis die Punktzahl an der gewünschten Stelle liegt.

SCREENSHOT

>[!NOTE]
>
>Der Spam-Wert wird über SpamAssassin ermittelt, und die Regeln gehören nicht Adobe. Weitere Informationen zu diesen Regeln finden Sie in der [SpamAssassin-Dokumentation](https://spamassassin.apache.org/#_blank). Eine vollständige Liste der Fehler [finden Sie hier](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com).
