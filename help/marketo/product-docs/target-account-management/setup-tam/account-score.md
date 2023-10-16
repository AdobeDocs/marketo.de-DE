---
unique-page-id: 11380774
description: Kontobewertung - Marketo-Dokumente - Produktdokumentation
title: Kontobewertung
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Kontobewertung {#account-score}

Die Kontobewertung ist ein wichtiger Bestandteil der Target-Kontoverwaltung. Dies hilft Ihnen bei der Bestimmung der Interaktionsstufe Ihrer Konten.

## Was ist Kontobewertung? {#what-is-account-scoring}

Es handelt sich dabei um einen systematischen Ansatz, der Vertriebs- und Marketingteams dabei hilft, Unternehmen (einschließlich Interessenten) zu identifizieren und zu priorisieren, die am ehesten einen Kauf tätigen.

In der komplexen Welt von B2B-Kaufprozessen ist es selten, dass eine Einzelperson eine Kaufentscheidung trifft. Es gibt oft verschiedene Rollen, die jeweils eigene Bedürfnisse haben. Bei der kontobasierten Auswertung wird dies berücksichtigt, indem die Lead-Bewertungen aus mehreren Leads aggregiert und eine Bewertung auf Kontoebene bereitgestellt wird.

## Häufige Beispiele {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Kundeninteraktions-Score</strong></td> 
   <td>Tiefe der Interaktion basierend auf Verhaltensaktivitäten, die über verschiedene Kanäle (z. B. E-Mail, Web und Anzeige) von Personen in bestimmten Zielkonten verfolgt werden.</td>
  </tr>
  <tr>
   <td><strong>Bewertung der Kundenproduktinteressen</strong></td>
   <td>Personen aus Zielkonten, die von einem bestimmten Produkt aus Interesse an dem Inhalt zeigen (z. B. das Herunterladen eines Whitepaper).</td> 
  </tr>
  <tr>
   <td><strong>Bewertung der Web-Interaktion des Kontos</strong></td>
   <td>Personen aus Zielkonten, die den Webkanal besuchen. Dieselbe Punktzahl kann erstellt werden, um die Kanalinteraktion aus E-Mail, Anzeigen oder anderen Kanälen zu messen.</td> 
  </tr>
 </tbody>
</table>

## Konfigurieren der Kontobewertung {#how-to-configure-account-score}

>[!NOTE]
>
>Um Kontobewertungen zu berechnen, müssen Sie zunächst Lead-Bewertungen erstellen. Marketo TAM aggregiert automatisch Lead-Bewertungen zu Kontobewertungen. Als Beispiel nehmen wir zwei der oben genannten Beispiele (_Bewertung der Kundenproduktinteressen_ und _Bewertung der Web-Interaktion des Kontos_).
>
>Erstellen Sie zunächst Lead-Punktfelder, die relevante Details aus jedem Lead eines Zielkontos erfassen.\
>Weisen Sie dann diese Lead-Bewertungen ihren jeweiligen Kontobewertungen zu:\
>Account Product Interest Score = SUM (Lead Product Interest Score)\
>Bewertung der Web-Interaktion des Kontos = SUM (Lead Web Engagement Score)

>[!NOTE]
>
>Benutzer können mehrere Kontointeraktionsbewertungen erstellen und unterschiedliche Personenergebnisse verschiedenen Kontobewertungen zuweisen.

Nachdem Sie die Lead-Punktzahl konfiguriert haben, fahren Sie mit den folgenden Schritten fort.

1. Klicks **Admin**.

   ![](assets/account-score-1.png)

1. Klicks **Verwaltung von Target-Konten**.

   ![](assets/account-score-2.png)

1. Klicken Sie in den Scoring-Feldern auf **Bearbeiten**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Sie können bis zu **fünf** -Felder zur Berechnung der Kontobewertung.

1. Geben Sie den Namen der Kontobewertung ein und klicken Sie auf **Personenbewertung auswählen** und wählen Sie den entsprechenden Wert aus.

   ![](assets/account-score-4.png)

1. Klicks **+Hinzufügen** , um weitere Bewertungen hinzuzufügen.

   ![](assets/account-score-5.png)

1. Fügen Sie alle gewünschten Bewertungen hinzu. Klicks **Speichern** wann geschehen.

   ![](assets/account-score-6.png)
