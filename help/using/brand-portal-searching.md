---
title: Suchen von Assets in Brand Portal
description: Mit der Brand Portal-Suchfunktion können Sie mithilfe von Omnisearch schnell nach relevanten Assets suchen. Suchfilter helfen Ihnen dabei, Ihre Suche weiter einzugrenzen. Speichern Sie Ihre Suchvorgänge als Smart-Sammlungen für die Zukunft.
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 52%

---

# Suchen von Assets in Brand Portal {#search-assets-on-brand-portal}

Mit der Brand Portal-Suchfunktion können Sie relevante Assets schnell mit der Omnisearch- und Facettensuche suchen, die Filter verwendet, um Ihre Suche weiter einzugrenzen. Sie können Elemente auf Dateien- oder Ordnerebene suchen und Ihre Suchergebnisse als Smart-Sammlungen speichern.

>[!NOTE]
>
>Brand Portal unterstützt keine Sammlungssuche mit Omnisearch.
>
>Sie können jedoch [Suchfilter zum Abrufen der Liste relevanter Sammlungen](#search-collection) verwenden.

## Suchen von Assets mithilfe von Omnisearch {#search-assets-using-omnisearch}

Gehen Sie wie folgt vor, um in Brand Portal nach Assets zu suchen:

1. Klicken Sie auf der Symbolleiste auf **[!UICONTROL Suchen]** oder drücken Sie die **[!UICONTROL /]**-Taste (Schrägstrich), um Omnisearch zu starten.

   ![](assets/omnisearchicon-1.png)

1. Geben Sie in das Suchfeld einen Suchbegriff für die Assets ein, die Sie suchen möchten.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* In Omnisearch sind mindestens 3 Zeichen erforderlich, damit Suchvorschläge angezeigt werden.
   >* Wenn Sie nach `mountain biking` suchen, gibt Omnisearch alle Assets in den Suchergebnissen zurück, für die sowohl `mountain` als auch `biking` in den Metadatenfeldern verfügbar sind. Zum Beispiel `mountain` im Feld `Title` und `biking` im Feld `Description`. Beide Begriffe müssen in den Metadatenfeldern verfügbar sein, damit sie in den Suchergebnissen angezeigt werden können. Omnisearch gibt das Asset jedoch in den Suchergebnissen selbst dann zurück, wenn im Metadatenfeld der Smart-Tags nur einer der beiden Begriffe verfügbar ist. Angenommen, ein Asset wurde als Smart-Tag `mountain`, in einem anderen Metadatenfeld fehlt jedoch `biking`. Dann suchen Sie nach `mountain biking`. Omnisearch gibt das Asset weiterhin in den Suchergebnissen zurück. Dieser Workflow stellt sicher, dass Assets mit relevanten Tags nicht übersehen werden.

1. Wählen Sie aus den entsprechenden Vorschlägen in der Dropdown-Liste aus, um schnell auf relevante Assets zuzugreifen.

   ![](assets/assets-search-result.png)

   *Asset-Suche mit Omnisearch*

Weitere Informationen zum Suchverhalten bei mit Smart-Tags versehenen Assets finden Sie unter [Suchergebnisse und -verhalten verstehen](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/using/search-assets).

## Suche mithilfe von Facetten im Bereich „Filter“ {#search-using-facets-in-filters-panel}

Suchfacetten im Bedienfeld „Filter“ erhöhen die Granularität Ihres Sucherlebnisses und verbessern die Suchfunktion. Suchfacetten verwenden mehrere Dimensionen (Prädikate), mit denen Sie komplexe Suchvorgänge durchführen können. Sie können für eine zielgerichtetere Suche einfach einen Drilldown zur gewünschten Detailtiefe durchführen.

Wenn Sie beispielsweise nach einem Bild suchen, können Sie auswählen, ob Sie ein Bitmap- oder ein Vektorbild möchten. Sie können den Suchbereich weiter eingrenzen, indem Sie den MIME-Typ des Bildes in der Suchfacette Dateityp angeben. Wenn Sie nach Dokumenten suchen, können Sie auf ähnliche Weise das gewünschte Format festlegen, zum Beispiel PDF oder MS® Word.

![Bereich „Filter“ in Brand Portal](assets/file-type-search.png "Bereich „Filter“ in Brand Portal")

Das Bedienfeld **[!UICONTROL Filter]** enthält einige Standardfacetten, z. B. **[!UICONTROL Pfad-Browser]**, **[!UICONTROL Dateityp]**, **[!UICONTROL Dateigröße]**, **[!UICONTROL Status]** und **[!UICONTROL Ausrichtung]**.
Sie können jedoch [benutzerdefinierte Suchfacetten hinzufügen](../using/brand-portal-search-facets.md) oder bestimmte aus dem Bedienfeld **[!UICONTROL Filter]** entfernen. Bearbeiten Sie einfach die Eigenschaften im zugrunde liegenden Suchformular. Siehe die Liste aller verfügbaren und verwendbaren [Suchprädikate in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

So können Sie mit den verfügbaren [Suchfacetten](../using/brand-portal-search-facets.md) die Filter auf Ihre Suche anwenden:

1. Klicken Sie auf das Symbol „Überlagerung“ und wählen Sie **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

1. Wählen Sie im Bereich **[!UICONTROL Filter]** auf der linken Seite die entsprechenden Optionen aus, um die relevanten Filter anzuwenden.
Verwenden Sie beispielsweise die folgenden Standardfilter:

   * Nutzen Sie den **[!UICONTROL Pfadbrowser]** um Assets in einem bestimmten Verzeichnis zu suchen. Der Standardsuchpfad des Prädikats für Pfad-Browser lautet `/content/dam/mac/<tenant-id>/`. Dieser kann durch Bearbeiten des Standard-Suchformulars konfiguriert werden.

   >[!NOTE]
   >
   >Für Benutzer ohne Administratorrechte zeigt der [!UICONTROL Pfad-Browser] im Bedienfeld [!UICONTROL Filter] nur die Inhaltsstruktur der Ordner (und der ihnen übergeordneten Ordner) an, die für sie freigegeben sind.\
   >Administratoren können über den Pfadbrowser zu einem beliebigen Ordner in Brand Portal navigieren.

   * **[!UICONTROL Dateityp]**, um den Typ (Bild, Dokument, Multimedia, Archiv) der gesuchten Asset-Datei anzugeben. Darüber hinaus können Sie den Umfang Ihrer Suche einschränken. Geben Sie zum Beispiel den MIME-Typ (TIFF, Bitmap, GIMP-Bilder) für Bilder oder das Format (PDF oder MS® Word) für die Dokumente an.
   * **[!UICONTROL Dateigröße]**, um nach Assets basierend auf ihrer Größe zu suchen. Sie können die untere und obere Grenze für den Größenbereich ausgeben, um Ihre Suche einzuschränken und die Maßeinheit für die Suche anzugeben.
   * **[!UICONTROL Status]**, um basierend auf dem Asset-Status, z. B. Genehmigung (Genehmigt, Änderung angefordert, Abgelehnt, Ausstehend) und Ablauf, nach Assets zu suchen.
   * **[!UICONTROL Durchschnittliche Bewertung]**, um nach Assets, basierend auf ihrer Bewertung, zu suchen.
   * **[!UICONTROL Ausrichtung]**, um nach Assets, basierend auf ihrer Ausrichtung (horizontal, vertikal, quadratisch), zu suchen.
   * **[!UICONTROL Stil]**, um basierend auf dem Stil (farbig, einfarbig) der Assets nach Assets zu suchen.
   * **[!UICONTROL Videoformat]**, um basierend auf dem Format von Video-Assets (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM) nach Video-Assets zu suchen.

   Sie können im Bedienfeld „Filter“ [benutzerdefinierte Suchfacetten](../using/brand-portal-search-facets.md) verwenden, indem Sie das zugrunde liegende Suchformular bearbeiten.

   * **[!UICONTROL Eigenschaftsprädikat]** ermöglicht es Ihnen, bei Verwendung im Suchformular nach Assets zu suchen, die mit einer Metadateneigenschaft übereinstimmen, der das Prädikat zugeordnet ist.\
     Wenn beispielsweise das Eigenschaftsprädikat `jcr:content/metadata/dc:title` zugeordnet ist, können Sie Assets auf Grundlage ihres Titels suchen.\
     Das [!UICONTROL Eigenschaftsprädikat] unterstützt die Textsuche nach Folgendem:

     **Teilsätze**
Um die Asset-Suche mithilfe teilweiser Sätze im Eigenschaftsprädikat zuzulassen, aktivieren Sie im Suchformular **[!UICONTROL Kontrollkästchen]** Teilsuche“. Mit dieser Methode können Sie nach den gewünschten Assets suchen, auch wenn Sie nicht die genauen Wörter oder Ausdrücke angeben, die in den Asset-Metadaten verwendet werden.

     >[!NOTE]
     >
     > Brand Portal unterstützt die folgenden Felder für die Teilsuche:
     >
     >* `jcr:content/metadata/dc:title`
     >* `jcr:content/jcr:title`
     >* `jcr:content/metadata/dc:format`

     Sie haben folgende Möglichkeiten:
      * Geben Sie ein Wort im Suchbegriff in der Facette im Bedienfeld Filter an. Wenn Sie beispielsweise nach dem Begriff **klettern** suchen (und das Eigenschaftsprädikat der `dc:title` Eigenschaft zugeordnet ist), werden alle Assets mit dem Wort **klettern** im Titelsatz zurückgegeben.
      * Geben Sie einen Teil des Wortes ein, das im Suchbegriff vorkommt, und füllen Sie die Lücken mit einem Platzhalterzeichen (&#42;).
Zum Beispiel gibt die Suche nach:
         * **klettern&#42;** alle Elemente zurück, deren Titelphrase Wörter enthält, die mit der Zeichenfolge „klettern“ beginnen.
         * **&#42;klettern** gibt alle Elemente zurück, deren Titelphrase Wörter enthält, die mit den Zeichen „klettern“ enden.
         * **&#42;klettern&#42;** gibt alle Elemente zurück, deren Titelphrase Wörter enthält, die die Zeichenfolge „klettern“ enthalten.

     **Text ohne Unterscheidung von Groß- und Kleinschreibung**
Sie können die Suche ohne Unterscheidung von Groß- und Kleinschreibung im Eigenschaftsprädikat zulassen. Aktivieren Sie einfach das **[!UICONTROL Groß-/Kleinschreibung ignorieren]** im Suchformular. Standardmäßig wird bei der Textsuche im Eigenschaftsprädikat zwischen Groß- und Kleinschreibung unterschieden.

   >[!NOTE]
   >
   >Wenn Sie das Kontrollkästchen **[!UICONTROL Teilsuche]** aktivieren, wird **[!UICONTROL Groß-/Kleinschreibung ignorieren]** standardmäßig aktiviert.

   ![](assets/wildcard-prop-1.png)

   Die Suchergebnisse werden entsprechend den angewendeten Filtern zusammen mit der Anzahl der Suchergebnisse angezeigt.

   ![](assets/omnisearch-with-filters.png)

   Asset-Suchergebnis mit der Anzahl der Suchergebnisse.

1. Sie können einfach zu einem Element in den Suchergebnissen navigieren und mit der Schaltfläche „Zurück“ in Ihrem Browser zum selben Suchergebnis zurückkehren, ohne die Suchabfrage erneut starten zu müssen.

## Suchen als Smart-Sammlung speichern {#save-your-searches-as-smart-collection}

Sie können die Sucheinstellungen als Smart-Sammlung speichern, um dieselbe Suche schnell wiederholen zu können, ohne dieselben Einstellungen später wiederholen zu müssen. Sie können jedoch keine Suchfilter in einer Sammlung anwenden.

So speichern Sie die Sucheinstellungen als Smart-Sammlung:

1. Klicken Sie **[!UICONTROL Smart-Sammlung speichern]** und geben Sie einen Namen für die Smart-Sammlung ein.

   Damit die Smart-Sammlung von allen Benutzern verwendet werden kann, aktivieren Sie die Option **[!UICONTROL Öffentlich]**. Eine Meldung bestätigt, dass die Smart-Sammlung erstellt und zur Liste der gespeicherten Suchen hinzugefügt wurde.

   >[!NOTE]
   >
   >Sie können Benutzerinnen und Benutzer ohne Administratorrechte daran hindern, Smart-Sammlungen öffentlich zu machen, um zu vermeiden, dass im Brand Portal des Unternehmens eine große Anzahl öffentlicher Smart-Sammlungen von Benutzerinnen und Benutzern ohne Administratorrechte erstellt wird. Unternehmen können die Konfiguration **[!UICONTROL Erstellung öffentlicher Smart-Sammlungen zulassen]** in den **[!UICONTROL Allgemein]** Einstellungen im Admin-Tools-Bereich deaktivieren.

   ![](assets/save_smartcollectionui.png)

1. Um die Smart-Sammlung unter einem anderen Namen zu speichern, aktivieren oder deaktivieren Sie das Kontrollkästchen **[!UICONTROL Öffentlich]** und klicken Sie auf **[!UICONTROL Smart-Sammlung bearbeiten]**.

   ![](assets/edit_smartcollection.png)

1. Wählen Sie im Dialogfeld **[!UICONTROL Smart-Sammlung bearbeiten]** die Option **[!UICONTROL Speichern unter]** aus und geben Sie einen Namen für die Smart-Sammlung ein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/saveas_smartsearch.png)


## Suchsammlung {#search-collection}

Omnisearch wird für Sammlungen nicht unterstützt. Sie können jedoch Suchfilter anwenden, um die relevanten Sammlungen aus der Oberfläche [!UICONTROL Sammlungen] aufzulisten.

Klicken Sie in der Oberfläche [!UICONTROL Sammlungen] auf das Überlagerungssymbol, um den Filterbereich in der linken Leiste zu öffnen. Wenden Sie einzelne oder mehrere Suchfilter aus den verfügbaren Filtern an (`modified date`, `access type` und `tags`). Es wird der relevanteste Satz von Sammlungen basierend auf den angewendeten Filtern aufgelistet.

![](assets/collection-search.png)
