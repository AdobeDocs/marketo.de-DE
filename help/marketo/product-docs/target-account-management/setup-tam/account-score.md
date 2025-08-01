---
unique-page-id: 11380774
description: Kontobewertung - Marketo-Dokumente - Produktdokumentation
title: Kontobewertung
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 2%

---

# [!UICONTROL Kontobewertung] {#account-score}

Die Kontobewertung ist ein wichtiger Bestandteil der [!UICONTROL Target-]&quot;. Damit können Sie den Grad der Interaktion mit Ihren Konten ermitteln.

## Was ist die Kontobewertung? {#what-is-account-scoring}

Dieser systematische Ansatz unterstützt Vertriebs- und Marketing-Teams bei der Identifizierung und Priorisierung der Unternehmen (einschließlich Interessenten), die mit hoher Wahrscheinlichkeit einen Kauf tätigen werden.

In der komplexen Welt der B2B-Kaufprozesse ist es selten, dass eine einzelne Person eine Kaufentscheidung trifft. Häufig sind verschiedene Rollen mit jeweils eigenen Bedürfnissen beteiligt. Die kontobasierte Bewertung berücksichtigt dies, indem die Lead-Bewertungen aus mehreren Leads aggregiert und eine Bewertung auf Kontoebene bereitgestellt werden.

## Häufige Beispiele {#common-examples}

<table>
 <tbody>
  <tr>
   <td><strong>Kundeninteraktions-Score</strong></td>
   <td>Interaktionstiefe basierend auf Verhaltensaktivitäten, die über verschiedene Kanäle (z. B. E-Mail, Internet und Werbung) von Personen in bestimmten Zielkonten verfolgt werden.</td>
  </tr>
  <tr>
   <td><strong>Kontoprodukt-Interessensbewertung</strong></td>
   <td>Personen aus Zielkonten, die Interesse an den Inhalten eines bestimmten Produkts zeigen (z. B. Herunterladen eines Whitepapers).</td>
  </tr>
  <tr>
   <td><strong>Web-Interaktionswert für Konto</strong></td>
   <td>Personen aus Zielkonten, die den Web-Kanal besuchen. Derselbe Score kann erstellt werden, um die Kanalinteraktion in E-Mails, Anzeigen oder anderen Kanälen zu messen.</td>
  </tr>
 </tbody>
</table>

## Konfigurieren der Kontobewertung {#how-to-configure-account-score}

>[!NOTE]
>
>Zur Berechnung der Kontobewertungen müssen Sie zunächst Lead-Bewertungen erstellen. Marketo TAM aggregiert Lead-Bewertungen automatisch zu Konto-Bewertungen. Als Beispiel nehmen wir zwei der oben genannten Beispiele (_Account Product Interest Score_ und _Account Web Engagement Score_).
>
>Erstellen Sie zunächst Lead-Bewertungsfelder, die relevante Details aus jedem Lead eines Zielkontos erfassen.
>&#x200B;>Weisen Sie dann diese Lead-Bewertungen ihren jeweiligen Account-Bewertungen zu:
>&#x200B;>Kontobewertung für Produktzinsen = SUM (Bewertung für Lead-Produktzinsen)
>&#x200B;>Account Web Engagement Score = SUM (Lead Web Engagement Score)

>[!NOTE]
>
>Benutzer können mehrere Kontointeraktionswerte erstellen und verschiedene Personenwerte verschiedenen Kontobewertungen zuweisen.

Nachdem Sie die Lead-Bewertung konfiguriert haben, fahren Sie mit den folgenden Schritten fort.

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/account-score-1.png)

1. Klicken Sie **[!UICONTROL Target-Kontoverwaltung]**.

   ![](assets/account-score-2.png)

1. Klicken [!UICONTROL &#x200B; in „Bewertungsfelder] auf **[!UICONTROL Bearbeiten]**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Sie können bis zu **fünf** Felder zur Berechnung des [!UICONTROL Kontowerts] auswählen.

1. Geben Sie [!UICONTROL &#x200B; Namen „Kontobewertung] ein, klicken Sie auf die **[!UICONTROL Personenbewertung auswählen]** und wählen Sie den entsprechenden Wert aus.

   ![](assets/account-score-4.png)

1. Klicken Sie auf **[!UICONTROL +]**, um weitere Scores hinzuzufügen.

   ![](assets/account-score-5.png)

1. Fügen Sie alle gewünschten Werte hinzu. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

   ![](assets/account-score-6.png)
