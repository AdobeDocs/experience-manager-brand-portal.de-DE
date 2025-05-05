---
title: Veröffentlichen von Vorgaben, Schemata und Facetten in Brand Portal
description: Erfahren Sie, wie Sie Vorgaben, Schemata und Facetten in Brand Portal veröffentlichen.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4d9d7afa2cd45ea68c2e15338c92aa29ecf09f91
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 43%

---

# Veröffentlichen von Vorgaben, Schemata und Facetten in Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

In diesem Artikel wird beschrieben, wie Vorgaben, Metadatenschemata und benutzerdefinierte Suchfacetten aus der AEM-Autoreninstanz in Brand Portal veröffentlicht werden. Mit der Veröffentlichungsfunktion können Unternehmen die in einer AEM-Autoreninstanz erstellten oder bearbeiteten Bildvorgaben, Metadatenschemata und Suchfacetten wiederverwenden. Dieser Ansatz reduziert doppelten Aufwand.

>[!NOTE]
>
>Die Funktion zum Veröffentlichen von Bildvorgaben, Metadatenschemata und Suchfacetten aus der AEM-Autoreninstanz in Brand Portal ist ab AEM 6.2 SP1-CFP7 und AEM 6.3 SP 1-CFP 1 (6.3.1.1) verfügbar.

## Veröffentlichen von Bildvorgaben in Brand Portal {#publish-image-presets-to-brand-portal}

Bildvorgaben sind eine Gruppe von Größenangaben und Formatierungsbefehlen, die zum Zeitpunkt der Bildbereitstellung angewendet werden. Bildvorgaben können in Brand Portal erstellt und geändert werden. Wenn eine AEM-Autoreninstanz im Dynamic Media-Modus ausgeführt wird, können Benutzerinnen und Benutzer alternativ Voreinstellungen in der AEM-Autoreninstanz erstellen und in AEM Assets Brand Portal veröffentlichen. Dadurch wird vermieden, dass dieselben Vorgaben in Brand Portal neu erstellt werden.
Nachdem die Vorgabe erstellt wurde, wird sie in der Leiste „Asset-Detail-Ausgabedarstellungen“ und im Dialogfeld „Herunterladen“ als dynamische Ausgabedarstellung aufgeführt.

>[!NOTE]
>
>Wenn die AEM-Autoreninstanz nicht im **[!UICONTROL Dynamic Media-Modus]** ausgeführt wird (der Kunde hat Dynamic Media nicht erworben), wird die Ausgabedarstellung **[!UICONTROL Pyramid TIFF]** der Assets zum Zeitpunkt des Uploads nicht erstellt. Bildvorgaben oder dynamische Ausgabedarstellungen funktionieren auf **[!UICONTROL Pyramid-TIFF]** eines Assets. Wenn daher **[!UICONTROL Pyramid TIFF]** in der AEM-Autoreninstanz nicht verfügbar ist, ist sie auch in Brand Portal nicht verfügbar. Daher sind auf der Seite mit den Asset-Details und im Dialogfeld Herunterladen in der Leiste „Ausgabedarstellungen“ keine dynamischen Ausgabedarstellungen vorhanden.

Gehen Sie wie folgt vor, um Bildvorgaben in Brand Portal zu veröffentlichen:

1. Klicken Sie in der AEM-Autoreninstanz auf das AEM-Logo, um auf die globale Navigationskonsole zuzugreifen. Klicken Sie dann auf das Werkzeugsymbol und navigieren Sie zu **[!UICONTROL Assets > Bildvorgaben]**.
1. Wählen Sie die Bildvorgabe oder mehrere Bildvorgaben aus der Liste von Bildvorgaben aus und klicken Sie auf **[!UICONTROL Publish zu Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Wenn Benutzer auf **[!UICONTROL Publish in Brand Portal]** klicken, werden die Bildvorgaben zur Veröffentlichung in die Warteschlange gestellt. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

Gehen Sie wie folgt vor, um die Veröffentlichung von Bildvorgaben in Brand Portal rückgängig zu machen:

1. Klicken Sie in der AEM-Autoreninstanz auf das AEM-Logo, um auf die globale Navigationskonsole zuzugreifen. Klicken Sie dann auf **[!UICONTROL Tools]** und navigieren Sie zu **[!UICONTROL Assets > Bildvorgaben]**.
1. Wählen Sie eine Bildvorgabe aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]** aus.

## Veröffentlichen des Metadatenschemas in Brand Portal {#publish-metadata-schema-to-brand-portal}

Im Metadatenschema sind das Layout und die Eigenschaften beschrieben, die auf der Eigenschaftenseite von Assets/Sammlungen angezeigt werden.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Wenn Benutzerinnen und Benutzer das Standardschema in einer AEM-Autoreninstanz bearbeitet haben und sie dasselbe Schema verwenden möchten wie das Standardschema in der Brand Portal, veröffentlichen Sie die Metadatenschema-Formulare in Brand Portal. In einem solchen Fall überschreiben die Standardschemata, die von der AEM-Autoreninstanz veröffentlicht wurden, das Standardschema bei Brand Portal.

Wenn Benutzer ein benutzerdefiniertes Schema in der AEM-Autoreninstanz erstellt haben, können sie das benutzerdefinierte Schema in Brand Portal veröffentlichen, anstatt dort dasselbe Schema noch einmal zu erstellen. Benutzer können dieses benutzerdefinierte Schema auf jeden Ordner und jede Sammlung in Brand Portal anwenden.

>[!NOTE]
>
>Standardschemata können nicht in der Brand Portal veröffentlicht werden, wenn sie in der AEM-Instanz gesperrt waren. Das heißt, sie werden nicht bearbeitet.

![](assets/default-schema-form.png)

>[!NOTE]
>
>Wenn auf eine AEM-Autoreninstanz ein Schema auf einen Ordner angewendet wird, muss dasselbe Schema auch auf der Brand Portal vorhanden sein. Dies hilft, die Konsistenz auf der Seite mit den Asset-Eigenschaften in AEM Author und Brand Portal aufrechtzuerhalten.

Gehen Sie wie folgt vor, um ein Metadatenschema aus der AEM-Autoreninstanz in Brand Portal zu veröffentlichen:

1. Klicken Sie in der AEM-Autoreninstanz auf das AEM-Logo, um auf die globale Navigationskonsole zuzugreifen. Klicken Sie dann auf das Werkzeugsymbol und navigieren Sie zu **[!UICONTROL Assets > Metadatenschemata]**.
1. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL In Brand Portal veröffentlichen]** aus.

>[!NOTE]
>
>Wenn Benutzer auf **[!UICONTROL In Brand Portal veröffentlichen]** klicken, werden die Metadatenschemata zur Veröffentlichung in die Warteschlange gestellt. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

So heben Sie die Veröffentlichung eines Metadatenschemas in Brand Portal auf:

1. Klicken Sie in der AEM-Autoreninstanz auf das AEM-Logo, um auf die globale Navigationskonsole zuzugreifen. Klicken Sie dann auf das Werkzeugsymbol und navigieren Sie zu **[!UICONTROL Assets > Metadatenschemata]**.
1. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]** aus.

## Veröffentlichen von Suchfacetten in Brand Portal {#publish-search-facets-to-brand-portal}

Suchformulare stellen Benutzern in Brand Portal die Funktion [Facettensuche](../using/brand-portal-search-facets.md) bereit. Die Suchfacetten ermöglichen detailliertere Suchen in Brand Portal. Alle dem Suchformular [hinzugefügten Eigenschaften](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/administer/search-facets) sind für Benutzer als Suchfacetten in Suchfiltern verfügbar.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Um ein benutzerdefiniertes Suchformular in der **[!UICONTROL Assets-Admin-Suchleiste]** von der AEM-Autoreninstanz aus zu verwenden, veröffentlichen Sie es direkt in Brand Portal, anstatt es erneut zu erstellen.

>[!NOTE]
>
>Um ein gesperrtes Suchformular auf der **[!UICONTROL Assets Admin Search Rail]** von AEM Assets in Brand Portal zu veröffentlichen, müssen Sie es zunächst bearbeiten. Nach der Bearbeitung und Veröffentlichung überschreibt dieses Suchformular das vorhandene Suchformular in Brand Portal.

Gehen Sie wie folgt vor, um die bearbeitete Suchfacette aus der AEM-Autoreninstanz in Brand Portal zu veröffentlichen:

1. Klicken Sie auf das AEM-Logo und navigieren Sie **[!UICONTROL Tools > Allgemein > Forms durchsuchen]**.
1. Wählen Sie das bearbeitete Suchformular und **[!UICONTROL In Brand Portal veröffentlichen]** aus.

   >[!NOTE]
   >
   >Wenn Benutzer auf **[!UICONTROL In Brand Portal veröffentlichen]** klicken, werden Suchfacetten zur Veröffentlichung in die Warteschlange gestellt. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

So heben Sie die Veröffentlichung von Suchformularen in Brand Portal auf:

1. Klicken Sie in der AEM-Autoreninstanz auf das AEM-Logo, um auf die globale Navigationskonsole zuzugreifen. Klicken Sie dann auf das Werkzeugsymbol und navigieren Sie zu **[!UICONTROL Allgemein > Forms durchsuchen]**.
1. Wählen Sie das Suchformular und oben die Option **[!UICONTROL Aus Brand Portal löschen]** aus.

>[!NOTE]
>
>Die **[!UICONTROL Veröffentlichung in Brand Portal rückgängig machen]**-Aktion verlässt das standardmäßige Suchformular in Brand Portal und stellt nicht das letzte Suchformular wieder her, das vor der Veröffentlichung verwendet wurde.

### Beschränkungen {#limitations}

1. Nur wenige Sucheigenschaften können nicht für Suchfilter in Brand Portal verwendet werden. Wenn diese Sucheigenschaften als Teil des Suchformulars aus der AEM-Autoreninstanz in Brand Portal veröffentlicht werden, werden sie herausgefiltert. Benutzer sehen daher eine geringere Anzahl von Eigenschaften in dem Formular, das in Brand Portal veröffentlicht wurde. Weitere Informationen finden Sie in der [Liste aller verwendbaren Sucheigenschaften in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Wenn [!UICONTROL Optionsprädikat] einen benutzerdefinierten Pfad zum Lesen von Optionen in einer AEM-Autoreninstanz verwendet, funktioniert dies in Brand Portal nicht. Diese zusätzlichen Pfade und Optionen werden nicht mit dem Suchformular in Brand Portal veröffentlicht. In diesem Fall können Benutzer die Option **[!UICONTROL Manuell]** unter **[!UICONTROL Optionen hinzufügen]** in der **[!UICONTROL Options-Eigenschaft]** auswählen, um diese Optionen manuell zu Brand Portal hinzuzufügen.

![](assets/options-predicate-manual.png)
