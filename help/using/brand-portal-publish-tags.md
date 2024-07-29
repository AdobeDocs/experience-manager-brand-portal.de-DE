---
title: Veröffentlichen von Tags in Brand Portal
description: Erfahren Sie, wie Sie Tags aus Experience Manager Assets in Brand Portal veröffentlichen.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: ff51a49a958d43c98443d816a92276faae5e9569
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 44%

---

# Veröffentlichen von Tags in Brand Portal {#publish-tags-to-brand-portal}

Erfahren Sie, wie Sie Tags aus Experience Manager Assets in Brand Portal veröffentlichen.

Tags sind nützlich für die Organisation von Assets und die Verbesserung der Suchbarkeit von Assets, mit denen sie verknüpft sind. Tags können als Keywords oder Beschriftungen (Metadaten) betrachtet werden, die mit Assets angehängt sind und es ermöglichen, Assets schnell als Ergebnis einer Suche zu finden. Informationen dazu, wie Tags den Assets in Experience Manager Assets zugewiesen werden, finden Sie im Artikel [Verwenden von Tags zum Organisieren von Assets](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/managing/organize-assets).

Tags (die mit Assets und Sammlungen in AEM verknüpft sind) werden automatisch in Brand Portal veröffentlicht, wenn die Assets (und Sammlungen) mit verknüpften Tags in Brand Portal veröffentlicht werden. Die veröffentlichten Tags sind hilfreich bei der Suche nach verknüpften Assets.

>[!NOTE]
>
>Adobe empfiehlt, Tags ausschließlich in Brand Portal zu veröffentlichen, bevor die Assets (und Sammlungen) veröffentlicht werden, mit denen die Tags verknüpft sind. Dieser Ansatz ermöglicht eine schnellere Veröffentlichung der Assets (und Sammlungen) in Brand Portal.

## Verwalten von Tags {#manage-tags}

Sie können bereits vorhandene Tags über die AEM-Tags-Konsole (**[!UICONTROL Tools ) an ein Asset anhängen oder neue Tags erstellen | Tagging | AEM Tags]**). In beiden Fällen müssen Sie die Tags zuerst in Brand Portal veröffentlichen und sie dann mit den entsprechenden Assets verknüpfen.

Führen Sie die folgenden Schritte aus, um Tags in AEM zu erstellen, in Brand Portal zu veröffentlichen und mit den entsprechenden Assets (oder Sammlungen) zu verknüpfen:

1. **Erstellen von Tags**
Melden Sie sich bei einer AEM-Autoreninstanz mit Administratorrechten an und greifen Sie über die globale Navigation auf die Konsole **[!UICONTROL AEM Tags]** zu:

   1. Wählen Sie **[!UICONTROL Tools]**

   1. Wählen Sie **[!UICONTROL Allgemein]**

   1. Wählen Sie **[!UICONTROL Tagging]**

1. Wählen Sie **[!UICONTROL Erstellen]** und dann die Option **[!UICONTROL Tag erstellen]** aus.
1. Geben Sie Folgendes an:

   * **[!UICONTROL Titel]**
     *(erforderlich)* Ein Anzeigetitel für das Tag.
   * **[!UICONTROL Name]**
     *(erforderlich)* Ein Name für das Tag. Wenn Sie keinen festlegen, wird ein gültiger Knotenname aus dem Titel erstellt. Siehe [TagID](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/implementing/developing/platform/tagging/framework).
   * **Beschreibung**
     *(optional)* Eine Beschreibung des Tags.
   * **Tag-Pfad** JCR-Pfad des Tags.

1. Wählen Sie **[!UICONTROL Übermitteln]** aus, um das Tag zu erstellen.

   Nachdem Sie ein Tag in einer AEM-Instanz erstellt haben, ist das Tag für die Anlage an ein Asset verfügbar (im Abschnitt Eigenschaften oder im Abschnitt Tags verwalten dieses Assets).

1. **Veröffentlichen Sie das Tag in Brand Portal**.

   Navigieren Sie zur Konsole **[!UICONTROL AEM Tags]** ([!UICONTROL Tools | Tagging | AEM Tags]), wählen Sie das gewünschte Tag und Publish zu Brand Portal aus.

1. **Hängen Sie das Tag an ein Asset (oder eine Sammlung) an.**

   Wählen Sie ein Asset (oder eine Sammlung) aus und fügen Sie das gewünschte Tag über den Abschnitt Eigenschaften oder den Abschnitt Tags verwalten dieses Assets an. Weitere Informationen zum Zuweisen von Tags zu Assets in AEM Assets finden Sie unter [Tags zum Organisieren von Assets verwenden](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/managing/organize-assets).

1. **Veröffentlichen Sie die Assets (oder Sammlungen) in Brand Portal**.\
   Wenn Sie ein Asset (oder eine Sammlung) in Brand Portal veröffentlichen, ist das beigefügte Tag auch in Brand Portal verfügbar.

   Um das angehängte Tag im entsprechenden Asset (oder in der Sammlung) in Brand Portal anzuzeigen, melden Sie sich bei Brand Portal an und wählen Sie dann das Asset aus. Im Abschnitt Eigenschaften wird das angehängte Tag angezeigt.

## Priorisieren der Suche {#search-promote}

In AEM Assets Brand Portal können Sie bestimmte Assets priorisieren, damit sie in den Suchanfragen, die auf einem Suchbegriff-Tag basieren, ganz oben in den Suchergebnissen erscheinen.

Gehen Sie wie folgt vor, um ein Asset für einen Suchbegriff zu priorisieren:

1. Öffnen Sie die Seite **[!UICONTROL Eigenschaften]** eines Assets in der AEM-Autoreninstanz.
1. Gehen Sie zur Registerkarte **[!UICONTROL Erweitert]** .
1. Wählen Sie im Abschnitt **[!UICONTROL Suche priorisieren]** im Abschnitt **[!UICONTROL Für Suchbegriffe erhöhen]** die Option **[!UICONTROL Hinzufügen]** aus, um die Suchbegriffe oder Tags hinzuzufügen.

   ![](assets/search-promote.png)

1. Speichern Sie die Änderungen.
1. Publish des Assets in Brand Portal.
1. Melden Sie sich bei Brand Portal an. Zeigen Sie die Registerkarte **[!UICONTROL Erweitert]** im Abschnitt **[!UICONTROL Eigenschaften]** des Assets an.
Beachten Sie, dass der Suchbegriff aus **[!UICONTROL Suche priorisieren]** auch in den Eigenschaften dieses Assets sichtbar ist.
