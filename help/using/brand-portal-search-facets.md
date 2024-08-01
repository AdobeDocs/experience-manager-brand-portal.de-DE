---
title: Verwenden benutzerdefinierter Suchfacetten
description: Administratoren können Sucheigenschaften zum Bereich „Filter“ hinzufügen, um die Suche anzupassen und die Suchfunktion auf diese Weise vielseitiger zu gestalten.
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 4c701781e7dc62b9d2b018fd13b1ae9616bbb840
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 59%

---

# Verwenden benutzerdefinierter Suchfacetten {#use-custom-search-facets}

Administratoren können Sucheigenschaften zum Bereich [!UICONTROL Filter] hinzufügen, um die Suche anzupassen und die Suchfunktion auf diese Weise vielseitiger zu gestalten.

Brand Portal unterstützt die [Facettensuche](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) für die detaillierte Suche nach genehmigten Marken-Assets, was aufgrund des Bereichs [**Filter**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) möglich ist. Suchfacetten werden im Bereich &quot;Filter&quot;über das **[!UICONTROL Suchformular]** in den Admin Tools bereitgestellt. In den Admin Tools ist auf der Seite &quot;Forms suchen&quot;ein standardmäßiges Suchformular mit dem Namen Asset-Admin-Suchschiene vorhanden. Administratoren können jedoch den Bereich &quot;Standardfilter&quot;anpassen. Sie können das standardmäßige Suchformular (Asset-Admin-Suchschiene) bearbeiten, indem sie Sucheigenschaften hinzufügen, bearbeiten oder entfernen, wodurch die Suchfunktion vielseitiger wird.

Sie können verschiedene Sucheigenschaften verwenden, um den Bereich **[!UICONTROL Filter]** anzupassen. Fügen Sie beispielsweise das Eigenschaftsprädikat hinzu, um nach Assets zu suchen, die einer einzelnen Eigenschaft entsprechen, die Sie in diesem Prädikat angeben. Fügen Sie das Optionsprädikat hinzu, um nach Assets zu suchen, die einem oder mehreren Werten entsprechen, die Sie für eine bestimmte Eigenschaft angeben. Fügen Sie das Datumsbereichsprädikat hinzu, um nach Assets zu suchen, die innerhalb eines bestimmten Datumsbereichs erstellt wurden.

>[!NOTE]
>
>In Experience Manager Assets können Unternehmen [die angepassten Suchformulare aus der AEM-Autoreninstanz](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) in Brand Portal veröffentlichen, anstatt dieselben Formulare noch einmal in Brand Portal zu erstellen.

## Hinzufügen von Sucheigenschaften zum Bereich &quot;Filter&quot; {#add-a-search-predicate}

1. Klicken Sie auf das Experience Manager-Logo oben in der Symbolleiste, um auf weitere Admin-Tools zuzugreifen.

   ![](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Suchformulare]**.

   ![](assets/navigation-panel-1.png)

1. Wählen Sie auf der Seite **[!UICONTROL Suchformulare]** die Option **[!UICONTROL Asset-Admin-Suchschiene]** aus.

   ![](assets/search-forms-page.png)

1. Klicken Sie in der Symbolleiste oben auf **[!UICONTROL Bearbeiten]** , um das Suchformular zu öffnen, damit Sie es bearbeiten können.

   ![](assets/edit-search-form-1.png)

1. Ziehen Sie auf der Seite [!UICONTROL Suchformular bearbeiten] eine Eigenschaft von der Registerkarte [!UICONTROL Eigenschaft auswählen] in den Hauptbereich. Ziehen Sie beispielsweise **[!UICONTROL Eigenschaftsprädikat]**.

   Das Feld **[!UICONTROL Eigenschaft]** wird im Hauptbereich angezeigt und die Registerkarte **[!UICONTROL Einstellungen]** auf der rechten Seite zeigt die Eigenschaftsprädikate an.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Mit der Kopfzeilenbeschriftung auf der Registerkarte **[!UICONTROL Einstellungen]** wird der Typ des gewählten Prädikats identifiziert.

1. Geben Sie auf der Registerkarte **[!UICONTROL Einstellungen]** eine Beschriftung, Platzhaltertext und eine Beschreibung für das Eigenschaftsprädikat ein.

   * Wählen Sie **[!UICONTROL Teilsuche]**, wenn Sie eine Teilphrasensuche (und Platzhaltersuche) für Assets basierend auf dem angegebenen Eigenschaftswert zulassen möchten. Das Prädikat unterstützt standardmäßig die Volltextsuche.
   * Wählen Sie **[!UICONTROL Groß-/Kleinschreibung ignorieren]**, wenn bei der auf dem Eigenschaftswert basierenden Asset-Suche nicht zwischen Groß- und Kleinschreibung unterschieden werden soll. Bei der Suche nach Eigenschaftswerten im Suchfilter wird standardmäßig zwischen Groß- und Kleinschreibung unterschieden.

   >[!NOTE]
   >
   >Wenn Sie das Kontrollkästchen **[!UICONTROL Teilsuche]** aktivieren, wird standardmäßig **[!UICONTROL Groß-/Kleinschreibung ignorieren]** ausgewählt.

1. Öffnen Sie im Feld **[!UICONTROL Eigenschaftsname]** die Eigenschaftsauswahl und wählen Sie die Eigenschaft basierend auf der Suche aus. Alternativ können Sie einen Namen für die Eigenschaft eingeben. Geben Sie beispielsweise `jcr :content/metadata/dc:title` oder `./jcr:content/metadata/dc:title` ein.

   >[!NOTE]
   >
   >In Brand Portal werden alle Zeichenfolgen-Eigenschaften (mit Ausnahme der Eigenschaften, die mit `xmp` beginnen) in `jcrcontent/metadata` von `dam:asset` standardmäßig indiziert. Alle anderen benutzerdefinierten Eigenschaften eines beliebigen Typs werden nicht standardmäßig indiziert.
   >
   >Jede indizierte Eigenschaft kann beim Erstellen eines Eigenschaftsprädikats verwendet werden. Wenn eine nicht indizierte Eigenschaft konfiguriert ist, liefert die Suchanfrage für eine nicht indizierte Eigenschaft möglicherweise kein Suchergebnis.

   ![](assets/title-prop.png)

1. Klicken Sie auf **[!UICONTROL Fertig]**, um die Einstellungen zu speichern.
1. Klicken Sie in der Benutzeroberfläche von [!UICONTROL Assets] auf das Überlagerungssymbol und wählen Sie **[!UICONTROL Filter]**, um zum Bereich **[!UICONTROL Filter]** zu wechseln. Das Prädikat **[!UICONTROL Eigenschaft]** wird dem Bereich hinzugefügt.

   ![](assets/property-filter-panel.png)

1. Geben Sie in das Textfeld **[!UICONTROL Eigenschaft]** einen Titel für das Asset ein, das gesucht werden soll. Beispiel: &quot;Adobe.&quot; Wenn Sie eine Suche durchführen, werden Assets, deren Titel „Adobe“ entspricht, in den Suchergebnissen angezeigt.

## Liste der Sucheigenschaften {#list-of-search-predicates}

Sie können die folgenden Prädikate auf ähnliche Weise wie **[!UICONTROL Eigenschaftsprädikate]** zum Bereich **[!UICONTROL Filter]** hinzufügen:

| **Prädikatsname** | **Beschreibung** | **Eigenschaften** |
|-------|-------|----------|
| **[!UICONTROL Pfadbrowser]** | Die Sucheigenschaft, um Assets an einem bestimmten Ort zu suchen. **Hinweis:** *Für einen angemeldeten Benutzer zeigt der Pfadbrowser beim Filter nur die Inhaltsstruktur der Ordner (und ihrer Vorgängerelemente) an, die für den Benutzer freigegeben sind.* <br> Administratoren können nach Assets in einem beliebigen Ordner suchen, indem sie mit dem Pfadbrowser zu diesem Ordner navigieren. <br> Nicht-Administratoren können dagegen Assets in einem Ordner suchen, auf den sie zugreifen können, indem sie im Pfadbrowser zu diesem Ordner navigieren. | <ul><li>Feldbezeichnung</li><li>Pfad</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Eigenschaft]** | Sucht nach Assets basierend auf einer bestimmten Metadaten-Eigenschaft. **Hinweis:** *Nach Aktivierung der Teilsuche wird standardmäßig „Groß-/Kleinschreibung ignorieren“ aktiviert*. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Teilsuche</li><li>Groß-/Kleinschreibung ignorieren</li><li> Beschreibung</li></ul> |
| **[!UICONTROL Mehrwert-Eigenschaft]** | Ähnlich wie ein Eigenschaftsprädikat, aber mehrere Eingabewerte zulassen, die durch ein Trennzeichen (standardmäßig ein Komma) getrennt sind, werden Assets, die mit einem der Eingabewerte übereinstimmen, in den Ergebnissen zurückgegeben. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Unterstützung von Trennzeichen</li><li>Groß-/Kleinschreibung ignorieren</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Tags]** | Die Sucheigenschaft, um Assets basierend auf Tags zu suchen. Sie können die Pfadeigenschaft konfigurieren, um verschiedene Tags in der Tag-Liste zu füllen. Administratoren müssen möglicherweise den Pfadwert ändern, z. B. [!UICONTROL /`etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]. Dies ist erforderlich, wenn sie das Suchformular aus AEM veröffentlichen, in dem der Pfad keine Mandanteninformationen enthält, z. B. [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Pfad</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Pfad]** | Die Sucheigenschaft, um Assets an einem bestimmten Ort zu suchen. | <ul><li>Feldbezeichnung</li><li>Pfad</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Relatives Datum]** | Mit der Sucheigenschaft können Sie Assets basierend auf dem relativen Datum ihrer Erstellung suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Relatives Datum</li></ul> |
| **[!UICONTROL Bereich]** | Mit der Sucheigenschaft können Sie nach Assets suchen, die in einem bestimmten Bereich von Eigenschaftswerten liegen. Im Bereich „Filter“ können Sie den Mindest- und den Höchstwert für den Bereich angeben. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Datumsbereich]** | Die Sucheigenschaft, um Assets zu suchen, die innerhalb eines bestimmten Bereichs für eine Datumseigenschaft erstellt wurden. Im Bereich „Filter“ können Sie das Start- und das Enddatum angeben. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Textbereich (von)</li><li>Textbereich (bis)</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Datum]** | Sucheigenschaft für eine Schieberegler-basierte Suche nach Assets basierend auf einer Datumseigenschaft | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Dateigröße]** | Die Sucheigenschaft, um Assets basierend auf ihrer Größe zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Pfad</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Asset zuletzt geändert]** | Die Sucheigenschaft, um Assets basierend auf dem Datum der letzten Änderung zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Genehmigungsstatus]** | Die Sucheigenschaft, um Assets basierend auf der Genehmigungsmetadateneigenschaft zu suchen. Der standardmäßige Eigenschaftsname lautet **`dam:status`**. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Checkout-Status]** | Mit der Sucheigenschaft können Sie Assets basierend auf dem Checkout-Status eines Assets beim Veröffentlichen aus AEM Assets suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Ausgecheckt von]** | Die Sucheigenschaft, um Assets basierend auf dem Benutzer zu suchen, der das Asset ausgecheckt hat. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Gültigkeitsstatus]** | Die Sucheigenschaft, um Assets basierend auf dem Ablaufstatus zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| **[!UICONTROL Mitglied der Sammlung]** | Mit der Sucheigenschaft können Sie Assets basierend darauf suchen, ob ein Asset Teil einer Sammlung ist. | Beschreibung |
| **[!UICONTROL Ausgeblendet]** | Diese Eigenschaft ist für Endbenutzer nicht explizit sichtbar und wird für versteckte Begrenzungen verwendet, die normalerweise dazu dienen, den Suchergebnistyp auf **`dam:Asset`** zu beschränken. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |

>[!NOTE]
>
>* Verwenden Sie nicht die Eigenschaften **[!UICONTROL Optionen]**, **[!UICONTROL Status veröffentlichen]** oder **[!UICONTROL Bewertung]**, da diese Eigenschaften in Brand Portal nicht funktionsfähig sind.
>* Die Ordnertyp-Eigenschaft `(nt:folder type)` wird in Brand Portal nicht unterstützt und kann Leistungsprobleme verursachen. Wenn es in einem veröffentlichten benutzerdefinierten Suchformular vorhanden ist, kann es durch Bearbeiten des Suchformulars gelöscht werden.

## Löschen von Sucheigenschaften {#delete-a-search-predicate}

Um eine Eigenschaft zu löschen, gehen Sie folgendermaßen vor:

1. Klicken Sie auf das Adobe-Logo, um auf die Admin-Tools zuzugreifen.

   ![](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Suchformulare]**.

   ![](assets/navigation-panel-2.png)

1. Wählen Sie auf der Seite **[!UICONTROL Suchformulare]** die Option **[!UICONTROL Asset-Admin-Suchschiene]** aus.

   ![](assets/search-forms-page.png)

1. Klicken Sie in der Symbolleiste oben auf **[!UICONTROL Bearbeiten]** , um das Suchformular zu öffnen, damit Sie es bearbeiten können.

   ![](assets/edit-search-form-2.png)

1. Wählen Sie auf der Seite [!UICONTROL Suchformular bearbeiten] im Hauptbereich die Eigenschaft aus, die Sie löschen möchten. Wählen Sie beispielsweise **[!UICONTROL Eigenschaftsprädikat]**.

   Die Registerkarte **[!UICONTROL Einstellungen]** auf der rechten Seite zeigt die Eigenschaftsprädikat-Felder an.

1. Klicken Sie zum Löschen des Eigenschaftsprädikats auf das Papierkorbsymbol. Klicken Sie im Dialogfeld **[!UICONTROL Feld löschen]** auf **[!UICONTROL Löschen]**, um die Löschaktion zu bestätigen.

   Das Feld **[!UICONTROL Eigenschaftsprädikat]** wird vom Hauptbereich entfernt und die Registerkarte **[!UICONTROL Eigenschaften]** wird leer angezeigt.

   ![](assets/search-form-delete-predicate.png)

1. Klicken Sie zum Speichern der Änderungen in der Symbolleiste auf **[!UICONTROL Fertig]**.
1. Klicken Sie in der Benutzeroberfläche von **[!UICONTROL Assets]** auf das Überlagerungssymbol und wählen Sie **[!UICONTROL Filter]**, um zum Bereich **[!UICONTROL Filter]** zu wechseln. Das Prädikat **[!UICONTROL Eigenschaft]** wurde aus dem Bereich entfernt.

   ![](assets/property-predicate-removed.png)
