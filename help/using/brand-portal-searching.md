---
title: Suchen von Assets in Brand Portal
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Mit der Suchfunktion von Brand Portal können Sie mithilfe von Omnisearch schnell nach relevanten Assets suchen. Mit Suchfiltern können Sie die Suche weiter eingrenzen. Speichern Sie Ihre Suchen als Smart-Sammlungen für die Zukunft.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: cbdd943b904882cc9a455bab24c3cf732d5966ca
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 94%

---

# Suchen von Assets in Brand Portal {#search-assets-on-brand-portal}

Die Suchfunktion in Brand Portal ermöglicht Ihnen die schnelle Suche nach relevanten Elementen mittels Omnisearch und Facettensuche. Die Facettensuche verwendet Filter, um die Suche weiter einzugrenzen. Sie können Elemente auf Dateien- oder Ordnerebene suchen und Ihre Suchergebnisse als Smart-Sammlungen speichern.

>[!NOTE]
>
>Brand Portal unterstützt keine Sammlungssuche mit Omnisearch.
>
>Sie können jedoch [Suchfilter zum Abrufen der Liste relevanter Sammlungen](#search-collection) verwenden.

## Suchen von Assets mithilfe von Omnisearch {#search-assets-using-omnisearch}

Gehen Sie wie folgt vor, um in Brand Portal nach Assets zu suchen:

1. Klicken Sie in der Symbolleiste auf das Symbol **[!UICONTROL Suchen]** oder drücken Sie die „**[!UICONTROL /]**“-Taste, um Omnisearch zu starten.

   ![](assets/omnisearchicon-1.png)

1. Geben Sie in das Suchfeld einen Suchbegriff für die Assets ein, die Sie suchen möchten.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* Hierfür sind mindestens drei Zeichen in Omnisearch erforderlich, damit Suchvorschläge angezeigt werden.
   >* Wenn Sie nach `mountain biking` suchen, gibt Omnisearch alle Assets in den Suchergebnissen zurück, für die sowohl `mountain` als auch `biking` in den Metadatenfeldern verfügbar sind. Zum Beispiel `mountain` im Feld `Title` und `biking` im Feld `Description`. Beide Begriffe müssen in den Metadatenfeldern verfügbar sein, damit sie in den Suchergebnissen angezeigt werden können. Omnisearch gibt das Asset jedoch in den Suchergebnissen selbst dann zurück, wenn im Metadatenfeld der Smart-Tags nur einer der beiden Begriffe vorhanden ist. Wenn zum Beispiel ein Asset `mountain` als eines der Smart-Tags enthält, aber in keinem anderen Metadatenfeld `biking` enthält und Sie nach `mountain biking` suchen, gibt Omnisearch das Asset weiterhin in den Suchergebnissen zurück.

1. Wählen Sie aus den relevanten Vorschlägen in der Dropdown-Liste ein Asset aus, auf das Sie schnell zugreifen möchten.

   ![](assets/assets-search-result.png)

   *Asset-Suche mithilfe von Omnisearch*

Weitere Informationen zum Suchverhalten in Bezug auf mit Smart-Tags versehenen Assets finden Sie unter [Nachvollziehen von Suchergebnissen und -verhalten](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html?lang=de).

## Suche mithilfe von Facetten im Bereich „Filter“ {#search-using-facets-in-filters-panel}

Suchfacetten im Bereich „Filter“ fügen Granularität zu Ihrer Suche hinzu und machen die Suchfunktion effizient. Suchfacetten verwenden mehrere Dimensionen (Prädikate), mit denen Sie komplexe Suchvorgänge durchführen können. Sie können für eine zielgerichtetere Suche einfach einen Drilldown zur gewünschten Detailtiefe durchführen.

Wenn Sie beispielsweise nach einem Bild suchen, können Sie auswählen, ob Sie ein Bitmap- oder ein Vektorbild möchten. Sie können den Suchbereich weiter reduzieren, indem Sie in der Suchfacette Dateityp den MIME-Typ für das Bild angeben. Wenn Sie nach Dokumenten suchen, können Sie auf ähnliche Weise das gewünschte Format festlegen, zum Beispiel PDF oder MS® Word.

![Bereich „Filter“ in Brand Portal](assets/file-type-search.png "Bereich „Filter“ in Brand Portal")

Der Bereich **[!UICONTROL Filter]** enthält einige Standardfacetten, wie z. B. **[!UICONTROL Pfadbrowser]**, **[!UICONTROL Dateityp]**, **[!UICONTROL Dateigröße]**, **[!UICONTROL Status]** und **[!UICONTROL Ausrichtung]**. Sie können jedoch [benutzerdefinierte Suchfacetten hinzufügen](../using/brand-portal-search-facets.md) oder spezifische Suchfacetten aus dem Bereich **[!UICONTROL Filter]** entfernen, indem Sie im zugrunde liegenden Suchformular Prädikate hinzufügen oder entfernen. Siehe die Liste aller verfügbaren und verwendbaren [Suchprädikate in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

So können Sie mit den verfügbaren [Suchfacetten](../using/brand-portal-search-facets.md) die Filter auf Ihre Suche anwenden:

1. Klicken Sie auf das Symbol „Überlagerung“ und wählen Sie **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

1. Wählen Sie im Bereich **[!UICONTROL Filter]** auf der linken Seite die entsprechenden Optionen aus, um die relevanten Filter anzuwenden.
Verwenden Sie beispielsweise die folgenden Standardfilter:

   * Nutzen Sie den **[!UICONTROL Pfadbrowser]** um Assets in einem bestimmten Verzeichnis zu suchen. Der Standardsuchpfad der Sucheigenschaft für den Pfadbrowser lautet `/content/dam/mac/<tenant-id>/`. Dieser kann durch Bearbeiten des Standardsuchformulars konfiguriert werden.

   >[!NOTE]
   >
   >Für Benutzer ohne Administratorrechte zeigt der [!UICONTROL Pfadbrowser] im Bereich [!UICONTROL Filter] nur die Inhaltsstruktur der Ordner (und der Vorgängerordner) an, die für sie freigegeben sind.\
   >Administratoren können über den Pfadbrowser zu einem beliebigen Ordner in Brand Portal navigieren.

   * **[!UICONTROL Dateityp]**, um den Typ (Bild, Dokument, Multimedia, Archiv) der gesuchten Asset-Datei anzugeben. Darüber hinaus können Sie den Umfang Ihrer Suche einschränken. Geben Sie zum Beispiel den MIME-Typ (TIFF, Bitmap, GIMP-Bilder) für Bilder oder das Format (PDF oder MS® Word) für die Dokumente an.
   * **[!UICONTROL Dateigröße]**, um nach Assets basierend auf ihrer Größe zu suchen. Sie können die untere und obere Grenze für den Größenbereich ausgeben, um Ihre Suche einzuschränken und die Maßeinheit für die Suche anzugeben.
   * **[!UICONTROL Status]**, um basierend auf dem Asset-Status, z. B. Genehmigung (Genehmigt, Änderung angefordert, Abgelehnt, Ausstehend) und Ablauf, nach Assets zu suchen.
   * **[!UICONTROL Durchschnittliche Bewertung]**, um nach Assets, basierend auf ihrer Bewertung, zu suchen.
   * **[!UICONTROL Ausrichtung]**, um nach Assets, basierend auf ihrer Ausrichtung (horizontal, vertikal, quadratisch), zu suchen.
   * **[!UICONTROL Stil]**, um basierend auf dem Stil (farbig, einfarbig) der Assets nach Assets zu suchen.
   * **[!UICONTROL Videoformat]**, um basierend auf dem Format von Video-Assets (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM) nach Video-Assets zu suchen.

   Sie können im Bedienfeld „Filter“ [benutzerdefinierte Suchfacetten](../using/brand-portal-search-facets.md) verwenden, indem Sie das zugrunde liegende Suchformular bearbeiten.

   * Wenn im Suchformular verwendet, können Sie mithilfe von **[!UICONTROL Eigenschaftsprädikat]** nach Assets suchen, die mit einer Metadateneigenschaft übereinstimmen, der das Prädikat zugeordnet ist.\
     Wenn beispielsweise das Eigenschaftsprädikat [!UICONTROL `jcr:content /metadata/dc:title`] zugeordnet ist, können Sie Assets auf Grundlage ihres Titels suchen.\
     Das [!UICONTROL Eigenschaftsprädikat] unterstützt die Textsuche nach Folgendem:

     **Teilsätze**
Wenn Sie die Asset-Suche mithilfe teilweiser Sätze im Eigenschaftsprädikat ermöglichen möchten, aktivieren Sie im Suchformular das Kontrollkästchen **[!UICONTROL Teilsuche]**. Dadurch können Sie nach den gewünschten Assets suchen, auch wenn Sie nicht die genauen Wörter/Sätze angeben, die in den Asset-Metadaten verwendet werden.

     >[!NOTE]
     >
     > Brand Portal unterstützt die folgenden Felder für die Teilsuche:
     >* jcr:content/metadata/dc:title
     >* jcr:content/jcr:title
     >* jcr:content/metadata/dam:search_promote
     >* jcr:content/metadata/dc:format

     Sie haben folgende Möglichkeiten:
      * Geben Sie im Bedienfeld „Filter“ in der Facette ein Wort an, das im gesuchten Satz vorhanden ist. Suchen Sie beispielsweise nach dem Begriff **klettern** (und das Eigenschaftsprädikat ist der Eigenschaft [!UICONTROL `dc:title`] zugeordnet), dann werden alle Assets mit dem Wort **klettern** in der Titelphrase zurückgegeben.
      * Geben Sie einen Teil des Wortes ein, das im Suchbegriff vorkommt, und füllen Sie die Lücken mit dem Platzhalterzeichen (&#42;).
Zum Beispiel gibt die Suche nach:
         * **klettern&#42;** alle Elemente zurück, deren Titelphrase Wörter enthält, die mit der Zeichenfolge „klettern“ beginnen.
         * **&#42;klettern** gibt alle Elemente zurück, deren Titelphrase Wörter enthält, die mit den Zeichen „klettern“ enden.
         * **&#42;klettern&#42;** gibt alle Elemente zurück, deren Titelphrase Wörter enthält, die die Zeichenfolge „klettern“ enthalten.

     **Text ohne Berücksichtigung der Groß- und Kleinschreibung**
Um die Suche im Eigenschaftsprädikat ohne Berücksichtigung der Groß-/Kleinschreibung zuzulassen, aktivieren Sie das Kontrollkästchen **[!UICONTROL Groß- und Kleinschreibung ignorieren]** im Suchformular. Bei der Textsuche im Eigenschaftsprädikat wird standardmäßig zwischen Groß- und Kleinschreibung unterschieden.

   >[!NOTE]
   >
   >Nach Aktivierung des Kontrollkästchens **[!UICONTROL Teilsuche]** wird **[!UICONTROL Groß-/Kleinschreibung ignorieren]** standardmäßig aktiviert.

   ![](assets/wildcard-prop-1.png)

   Die Suchergebnisse werden entsprechend den angewendeten Filtern zusammen mit der Anzahl der Suchergebnisse angezeigt.

   ![](assets/omnisearch-with-filters.png)

   Asset-Suchergebnis mit Zählung der Suchergebnisse.

1. Sie können einfach zu einem Element in den Suchergebnissen navigieren und mit der Schaltfläche „Zurück“ in Ihrem Browser zum selben Suchergebnis zurückkehren, ohne die Suchabfrage erneut starten zu müssen.

## Suchen als Smart-Sammlung speichern {#save-your-searches-as-smart-collection}

Sie können die Sucheinstellungen als Smart-Sammlung speichern, damit Sie dieselbe Suche zu einem späteren Zeitpunkt wiederholen können, ohne die Einstellungen erneut vornehmen zu müssen. Sie können jedoch keine Suchfilter in einer Sammlung anwenden.

So speichern Sie die Sucheinstellungen als Smart-Sammlung:

1. Tippen/klicken Sie auf **[!UICONTROL Smart-Sammlung speichern]** und geben Sie einen Namen für die Smart-Sammlung ein.

   Damit die Smart-Sammlung von allen Benutzern verwendet werden kann, aktivieren Sie die Option **[!UICONTROL Öffentlich]**. Eine Meldung bestätigt, dass die Smart-Sammlung erstellt und zur Liste der gespeicherten Suchen hinzugefügt wurde.

   >[!NOTE]
   >
   >Benutzer ohne Administratorrechte können daran gehindert werden, Smart-Sammlungen öffentlich zu machen. So kann verhindert werden, dass Benutzer ohne Administratorrechte eine große Anzahl öffentlicher Smart-Sammlungen im Brand Portal der Organisation erstellen. Unternehmen können die Konfiguration **[!UICONTROL Erstellung öffentlicher Smart-Sammlungen zulassen]** im Admin-Tools-Bereich unter den Einstellungen **[!UICONTROL Allgemein]** deaktivieren.

   ![](assets/save_smartcollectionui.png)

1. Um die Smart-Sammlung unter einem anderen Namen zu speichern, aktivieren oder deaktivieren Sie das Kontrollkästchen **[!UICONTROL Öffentlich]** und klicken Sie auf **[!UICONTROL Smart-Sammlung bearbeiten]**.

   ![](assets/edit_smartcollection.png)

1. Wählen Sie im Dialogfeld **[!UICONTROL Smart-Sammlung bearbeiten]** die Option **[!UICONTROL Speichern unter]** aus und geben Sie einen Namen für die Smart-Sammlung ein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/saveas_smartsearch.png)


## Suchsammlung {#search-collection}

Omnisearch wird für Sammlungen nicht unterstützt. Sie können jedoch Suchfilter anwenden, um die relevanten Sammlungen aus der Oberfläche [!UICONTROL Sammlungen] aufzulisten.

Klicken Sie in der Oberfläche [!UICONTROL Sammlungen] auf das Überlagerungssymbol, um den Filterbereich in der linken Leiste zu öffnen. Wenden Sie einzelne oder mehrere Suchfilter aus den verfügbaren Filtern an (`modified date`, `access type` und `tags`). Es wird der relevanteste Satz von Sammlungen basierend auf den angewendeten Filtern aufgelistet.

![](assets/collection-search.png)
