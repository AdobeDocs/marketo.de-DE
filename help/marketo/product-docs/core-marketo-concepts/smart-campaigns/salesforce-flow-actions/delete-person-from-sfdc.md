---
unique-page-id: 1147031
description: Person aus dem SFDC löschen - Marketing Docs - Produktdokumentation
title: Person aus dem SFDC löschen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Person aus dem SFDC löschen {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Interessenten aus Salesforce entfernen, diese jedoch als Personen in Marketo belassen müssen, können Sie die Flusshandlung &quot;Person aus SFDC löschen&quot;verwenden.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Nur verfügbar, wenn in Salesforce integriert.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie dann auf **Benutzeraktionen** und wählen Sie **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Wählen Sie &quot;Person aus dem **SFDC** löschen&quot;.

   ![](assets/delete-person-from-sfdc.png)

1. Vergewissern Sie sich, dass die Einstellung &quot; **Löschen in Marker** &quot; **false** lautet, und klicken Sie dann auf **&quot;Jetzt** ausführen&quot;.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Nachdem der Flussschritt ausgeführt wurde, wird Ihre Person nicht mehr ein Lead in Salesforce sein, sondern in Marketo bleiben.

   >[!CAUTION]
   >
   >Wenn Sie **Löschen in Marketo** auf **true** einstellen und die Leute aus Marketo und die Interessenten aus Salesforce löschen, sind sie für immer weg. Das kann nicht rückgängig gemacht werden.

