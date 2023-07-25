---
unique-page-id: 10097613
description: Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 1%

---

# Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen {#add-marketo-custom-object-link-fields}

Wenn Sie benutzerdefinierte Objekte erstellen, müssen Sie Verknüpfungsfelder bereitstellen, um den benutzerdefinierten Objektdatensatz mit dem richtigen übergeordneten Datensatz zu verbinden.

* Verwenden Sie für eine 1:n-benutzerdefinierte Struktur das Linkfeld im benutzerdefinierten Objekt, um es mit einer Person oder einem Unternehmen zu verbinden.
* Für eine n:n-Struktur verwenden Sie zwei Verknüpfungsfelder, die mit einem separat erstellten Intermediär-Objekt verbunden sind (auch ein benutzerdefinierter Objekttyp). Eine Verknüpfung stellt eine Verbindung zu Personen oder Unternehmen in Ihrer Datenbank her, die andere eine Verbindung zum benutzerdefinierten Objekt. In diesem Fall befindet sich das Linkfeld nicht im benutzerdefinierten Objekt selbst.

## Erstellen eines Link-Felds für eine 1:n-Struktur {#create-a-link-field-for-a-one-to-many-structure}

So erstellen Sie ein Verknüpfungsfeld in einem benutzerdefinierten Objekt für eine 1:n-Struktur.

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Klicken **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Wählen Sie das benutzerdefinierte Objekt in der Liste aus.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. Im **[!UICONTROL Felder]** Registerkarte, klicken Sie auf **[!UICONTROL Neues Feld]**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Benennen Sie das Link-Feld und fügen Sie eine optionale [!UICONTROL Beschreibung]. Stellen Sie sicher, dass Sie die [!UICONTROL Link] Datentyp.

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Sie können nicht zurückkehren und eine [!UICONTROL Link] oder [!UICONTROL Deduplizierungsfeld] sobald das benutzerdefinierte Objekt genehmigt wurde.

1. Wählen Sie aus, ob die [!UICONTROL Link-Objekt] ist für [!UICONTROL Lead] (Person) oder [!UICONTROL Firma].

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Wenn Sie [!UICONTROL Lead]angezeigt, werden in der Liste &quot;ID&quot;, &quot;E-Mail-Adresse&quot;und alle benutzerdefinierten Felder angezeigt.
   >
   >Wenn Sie [!UICONTROL Firma]angezeigt, werden die ID und alle benutzerdefinierten Felder in der Liste angezeigt.

1. Wählen Sie die [!UICONTROL Link-Feld] Sie möchten eine Verbindung mit als übergeordnetes Element des neuen Felds herstellen.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >Im Linkfeld werden nur Zeichenfolgenfeldtypen unterstützt.

1. Klicken **[!UICONTROL Speichern]**.

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Erstellen eines Verknüpfungsfelds für eine Viele-zu-viele-Struktur {#create-a-link-field-for-a-many-to-many-structure}

So erstellen Sie ein Verknüpfungsfeld in einem zwischengeschalteten Objekt zur Verwendung in einer n:n-Struktur.

>[!PREREQUISITES]
>
>Sie müssen das Zwischenobjekt und alle benutzerdefinierten Objekte, mit denen Sie es verknüpfen möchten, bereits erstellt haben.

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Klicken **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Wählen Sie das zwischengeschaltete Objekt aus, dem Sie das Feld hinzufügen möchten.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. Im **[!UICONTROL Felder]** Registerkarte, klicken Sie auf **[!UICONTROL Neues Feld]**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Sie müssen zwei Verknüpfungsfelder erstellen. Erstellen Sie sie einzeln. Benennen Sie zunächst das Feld für die Mitglieder Ihrer Datenbankliste (z. B. leadID). Hinzufügen eines optionalen [!UICONTROL Beschreibung]. Stellen Sie sicher, dass Sie die [!UICONTROL link] [!UICONTROL Datentyp].

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Sie können nicht zurückkehren und eine [!UICONTROL Link] oder [!UICONTROL Deduplizierungsfeld] sobald das benutzerdefinierte Objekt genehmigt wurde.

1. Wählen Sie die [!UICONTROL Link-Objekt] aus Ihrer Datenbank; in diesem Fall [!UICONTROL Lead].

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Wählen Sie die [!UICONTROL Link-Feld] Sie möchten in diesem Fall eine Verbindung mit herstellen. [!UICONTROL ID].

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >Nur Zeichenfolgenfeldtypen werden im [!UICONTROL Link-Feld].

1. Klicken **[!UICONTROL Speichern]**.

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Wiederholen Sie diesen Vorgang für den zweiten Link zu Ihrem benutzerdefinierten Objekt, in diesem Beispiel &quot;kursID&quot;. Die [!UICONTROL Link-Objekt] name wird natürlich sein, und die [!UICONTROL Link-Feld] ist natürlich natürlichID. Da Sie das benutzerdefinierte Kursobjekt bereits erstellt und genehmigt haben, sind diese Auswahlmöglichkeiten in den Dropdown-Menüs verfügbar.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Erstellen Sie alle anderen Felder, die Sie in Ihrem Zwischenobjekt verwenden möchten, z. B. enrollmentID oder grade.

## Verwenden benutzerdefinierter Objekte {#using-custom-objects}

Der nächste Schritt besteht darin, diese benutzerdefinierten Objekte in Filtern in Ihren Smart-Kampagnen zu verwenden. Mit einer n:n-Beziehung können Sie mehrere Personen/Unternehmen und mehrere benutzerdefinierte Objekte auswählen. Im folgenden Beispiel wird jeder Benutzer in Ihrer Datenbank aufgelistet, der diese Kriterien erfüllt. Das Feld coursename stammt aus dem benutzerdefinierten Kurs-Objekt und die Registrierungsstufe stammt aus dem Zwischenobjekt.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objektfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
