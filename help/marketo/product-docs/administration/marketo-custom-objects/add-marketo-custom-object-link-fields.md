---
unique-page-id: 10097613
description: hinzufügen "Marketo Custom Object Link"-Felder - "Marketing to Docs"- Produktdokumentation
title: hinzufügen "Markieren in benutzerdefinierten Objektverknüpfungsfeldern"
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# hinzufügen Felder für die Verknüpfung mit benutzerdefinierten Objekten {#add-marketo-custom-object-link-fields}

Wenn Sie benutzerdefinierte Objekte erstellen, müssen Sie Verknüpfungsfelder bereitstellen, um den benutzerdefinierten Objektdatensatz mit dem richtigen übergeordneten Datensatz zu verbinden.

* Verwenden Sie für eine benutzerdefinierte Eins-zu-viele-Struktur das Linkfeld im benutzerdefinierten Objekt, um eine Verbindung zu einer Person oder Firma herzustellen.
* Für eine Viele-zu-viele-Struktur verwenden Sie zwei Verknüpfungsfelder, die mit einem separat erstellten Zwischenobjekt verbunden sind (auch ein benutzerdefinierter Objekttyp). Ein Link stellt eine Verbindung zu Personen oder Firmen in Ihrer Datenbank her, der andere eine Verbindung zum benutzerdefinierten Objekt. In diesem Fall befindet sich das Feld &quot;Link&quot;nicht im benutzerdefinierten Objekt selbst.

## Erstellen eines Linkfelds für eine 1-zu-viele-Struktur {#create-a-link-field-for-a-one-to-many-structure}

So erstellen Sie ein Verknüpfungsfeld in einem benutzerdefinierten Objekt für eine Eins-zu-viele-Struktur.

1. Klicken Sie auf **Admin** und wählen Sie in **Datenbankverwaltung** **Markieren Sie die Option**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Wählen Sie das benutzerdefinierte Objekt in der Liste aus.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. Klicken Sie auf der Registerkarte **Felder** auf **Neues Feld**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Benennen Sie das Linkfeld und fügen Sie eine optionale Beschreibung hinzu. Wählen Sie unbedingt den Datentyp &quot;Link&quot;aus.

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Sie können ein Verknüpfungs- oder Deduplizierungsfeld nicht mehr erstellen, bearbeiten oder löschen, nachdem das benutzerdefinierte Objekt genehmigt wurde.

1. Wählen Sie aus, ob das Linkobjekt für einen Interessenten (eine Person) oder eine Firma bestimmt ist.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Lead&quot;auswählen, werden ID, E-Mail-Adresse und alle benutzerdefinierten Felder in der Liste angezeigt.
   >
   >
   >Wenn Sie &quot;Firma&quot;auswählen, werden in der Liste &quot;ID&quot;und alle benutzerdefinierten Felder angezeigt.

1. Wählen Sie das Verknüpfungsfeld aus, mit dem Sie eine Verbindung herstellen möchten, als übergeordnetes Element des neuen Felds.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >Im Feld &quot;Link&quot;werden nur Zeichenfolgen-Feldtypen unterstützt.

1. Klicken Sie auf **Speichern.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Erstellen eines Linkfelds für eine Viele-zu-viele-Struktur {#create-a-link-field-for-a-many-to-many-structure}

So erstellen Sie ein Verknüpfungsfeld in einem Zwischenobjekt, das in einer Viele-zu-viele-Struktur verwendet werden kann.

>[!PREREQUISITES]
>
>Sie müssen das intermediäre Objekt und alle benutzerdefinierten Objekte, mit denen Sie es verknüpfen möchten, bereits erstellt haben.

1. Klicken Sie auf **Admin** und wählen Sie in **Datenbankverwaltung** **Markieren Sie die Option**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Wählen Sie das Zwischenobjekt aus, dem Sie das Feld hinzufügen möchten.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. Klicken Sie auf der Registerkarte **Felder **auf **Neues Feld**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. Sie müssen zwei Verknüpfungsfelder erstellen. Erstellen Sie sie einzeln. Benennen Sie zunächst das Feld für die Mitglieder Ihrer Datenbankkomponente (z. B. leadID). hinzufügen eine optionale Beschreibung. Stellen Sie sicher, dass Sie den Linkdatentyp auswählen.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Sie können ein Verknüpfungs- oder Deduplizierungsfeld nicht mehr erstellen, bearbeiten oder löschen, nachdem das benutzerdefinierte Objekt genehmigt wurde.

1. Wählen Sie das Link-Objekt aus Ihrer Datenbank, in diesem Fall Interessent.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Wählen Sie das Verknüpfungsfeld aus, mit dem Sie eine Verbindung herstellen möchten, in diesem Fall &quot;ID&quot;.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >Im Feld &quot;Link&quot;werden nur Zeichenfolgen-Feldtypen unterstützt.

1. Klicken Sie auf **Speichern.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Wiederholen Sie diesen Vorgang für die zweite Verknüpfung zu Ihrem benutzerdefinierten Objekt, in diesem Beispiel, natürlichID. Der Link-Objektname lautet natürlich, und das Link-Feld lautet kursID. Da Sie das benutzerdefinierte Kursobjekt bereits erstellt und genehmigt haben, stehen diese Auswahlen in den Dropdownmenüs zur Verfügung.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Erstellen Sie alle anderen Felder, die Sie in Ihrem Zwischenobjekt verwenden möchten, z. B. enrollmentID oder grade.

## Verwenden benutzerdefinierter Objekte {#using-custom-objects}

Der nächste Schritt besteht darin, diese benutzerdefinierten Objekte in Filtern in Ihren intelligenten Kampagnen zu verwenden. In einer Viele-zu-viele-Beziehung können Sie mehrere Personen/Firmen und mehrere benutzerdefinierte Objekte auswählen. Im folgenden Beispiel wird jeder Benutzer in Ihrer Datenbank aufgelistet, der diese Kriterien erfüllt. Das Feld coursename stammt aus dem benutzerdefinierten Kursobjekt und die Registrierungsstufe stammt aus dem Zwischenobjekt.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [hinzufügen &quot;Markieren in benutzerdefinierten Objektfeldern&quot;](add-marketo-custom-object-fields.md)
>* [Bearbeiten und Löschen eines Markierungen zu einem benutzerdefinierten Objekt](edit-and-delete-a-marketo-custom-object.md)
>* [Erläuterungen zu benutzerdefinierten Objekten](understanding-marketo-custom-objects.md)
>* [Bearbeiten und Löschen von Markierungen in benutzerdefinierten Objektfeldern](edit-and-delete-marketo-custom-object-fields.md)

>



