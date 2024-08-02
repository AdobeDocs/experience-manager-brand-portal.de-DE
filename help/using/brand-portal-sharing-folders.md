---
title: Freigeben von Ordnern
description: Brand Portal erfordert, dass Assets von einer vorkonfigurierten Experience Manager Assets-Autoreninstanz veröffentlicht werden. Benutzer ohne Administratorrechte können nur dann auf veröffentlichte Assets zugreifen, wenn sie während der Replikationseinrichtung mit Experience Manager konfiguriert wurden. Assets müssen dann für sie freigegeben werden.
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 50%

---

# Freigeben von Ordnern in Brand Portal {#share-folders}

Assets müssen in Brand Portal aus einer vorkonfigurierten Experience Manager-Autoreninstanz veröffentlicht werden, da Brand Portal die Asset-Erfassung nicht unterstützt.

## Workflow zur Ordnerfreigabe in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Nachfolgend werden der Ordnerfreigabe-Workflow und der Benutzerzugriff beschrieben:

* Standardmäßig werden alle aus Experience Manager Assets in Brand Portal veröffentlichten Ordner nur für den Brand Portal-Administrator angezeigt, wenn sie bei der Konfiguration der Replikation nicht als „Öffentlich“ gekennzeichnet sind.
* Der Administrator nutzt die Konsole **[!UICONTROL Ordnereigenschaften]**, um einen Ordner für ausgewählte Benutzer oder Gruppen freizugeben. Nur die Benutzer oder Gruppen, für die der Ordner freigegeben ist, können den Ordner nach der Anmeldung bei Brand Portal sehen. Der Ordner ist für andere Benutzer nicht sichtbar.
* Der Administrator kann auch festlegen, dass ein Ordner öffentlich zugänglich gemacht wird, und zwar durch das Kontrollkästchen **[!UICONTROL Öffentlicher Ordner]** in den **[!UICONTROL Ordnereigenschaften]**. Ein öffentlicher Ordner ist für alle Benutzer sichtbar.

* Unabhängig von den Benutzerrollen und Berechtigungen sehen Benutzer bei der Anmeldung bei Brand Portal alle öffentlichen Ordner sowie die Ordner, die direkt für sie oder eine Gruppe freigegeben sind, zu der sie gehören. Private Ordner oder Ordner, die für andere Benutzer freigegeben wurden, sind nicht für alle Benutzer sichtbar.

### Freigeben von Ordnern für Benutzergruppen in Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Die Zugriffsrechte für die Assets eines Ordners hängen von den Zugriffsrechten für den jeweiligen übergeordneten Ordner ab, unabhängig von den Einstellungen der untergeordneten Ordner. Dieses Verhalten wird von [ACLs](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/security/security) in AEM gesteuert, wobei untergeordnete Ordner ACLs von ihren übergeordneten Ordnern übernehmen. Angenommen, Ordner A enthält Ordner B, der den Ordner C enthält. Dann haben auch eine Benutzergruppe (oder Benutzer) mit Zugriffsrechten für Ordner A dieselben Zugriffsrechte für Ordner B und Ordner C. Da Ordner B der untergeordnete Ordner von A ist, erbt er seine ACLs, und der Ordner C, der dem Ordner B untergeordnet ist, erbt seine ACLs.

Ebenso haben Benutzergruppen (oder Benutzer), die nur Zugriff auf Ordner B haben, dieselben Zugriffsberechtigungen für Ordner C, jedoch nicht für Ordner A. Adobe empfiehlt, Inhalte so zu organisieren, dass die am häufigsten angezeigten Assets in untergeordneten Ordnern platziert werden, sodass der Zugriff von den untergeordneten Ordnern bis zum Stammordner beschränkt werden kann.

### Veröffentlichen von öffentlichen Ordnern {#public-folder-publish}

Benutzer ohne Administratorrechte (z. B. Bearbeiter und Betrachter) können nur dann auf Assets zugreifen, die aus AEM Assets in Brand Portal veröffentlicht wurden, wenn während der Brand Portal-Replikationskonfiguration die Option **[!UICONTROL Öffentlicher Ordner - Publish]** ausgewählt wurde.

![](assets/assetbpreplication.png)

Wenn die Option **[!UICONTROL Öffentlicher Ordner - Publish]** deaktiviert ist, müssen Administratoren diese Assets mithilfe der Freigabefunktion speziell für Benutzer ohne Administratorrechte freigeben.

>[!NOTE]
>
>Die Option **[!UICONTROL Veröffentlichung eines öffentlichen Ordners]** ist ab AEM-Version 6.3.2.1 verfügbar.

## Zugriff auf freigegebene Ordner {#access-to-shared-folders}

In der folgenden Matrix werden die Zugriffsberechtigungen und Berechtigungen zum Freigeben oder Aufheben der Freigabe von Assets für verschiedene Benutzerrollen dargestellt:

|               | Zugriff auf alle Ordner, die aus AEM Assets in Brand Portal veröffentlicht wurden | Zugriff auf freigegebene Ordner | Freigeben oder Aufheben der Freigabe von Ordnerberechtigungen |
|---------------|-----------|-----------|------------|
| Administrator | Ja | Ja | Ja |
| Bearbeiter | Nein* | Ja nur, wenn es für sie oder die Gruppe freigegeben wurde, zu der sie gehören | Ja, nur für die Ordner, die für die Benutzer oder deren Gruppe freigegeben wurden |
| Betrachter | Nein* | Ja nur, wenn es für sie oder die Gruppe freigegeben wurde, zu der sie gehören | Nein |
| Gastbenutzer | Nein* | Ja nur, wenn es für sie oder die Gruppe freigegeben wurde, zu der sie gehören | Nein |

>[!NOTE]
>
>Standardmäßig ist die Option **[!UICONTROL Öffentlichen Ordner veröffentlichen]** bei der Konfiguration der Replikation von Brand Portal mit der AEM-Autoreninstanz deaktiviert. Wenn die Option aktiviert ist, können standardmäßig alle Benutzer (auch Benutzer ohne Administratorrechte) auf die in Brand Portal veröffentlichten Ordner zugreifen.

### Zugriff von Benutzern ohne Administratorrechte auf freigegebene Ordner {#non-admin-user-access-to-shared-folders}

Benutzer ohne Administratorrechte können nur auf die Ordner zugreifen, die in Brand Portal für sie freigegeben sind. Wie diese Ordner jedoch beim Anmelden im Portal angezeigt werden, hängt von den Einstellungen der Konfiguration **[!UICONTROL Ordnerhierarchie aktivieren]** ab.

**Wenn die Konfiguration deaktiviert ist**

Benutzer ohne Administratorrechte können bei der Anmeldung bei der Brand Portal alle Ordner sehen, die für sie auf der Landingpage freigegeben wurden.

![](assets/disabled-folder-hierarchy1-1.png)

**Wenn die Konfiguration aktiviert ist**

Benutzer ohne Administratorrechte sehen bei der Anmeldung bei Brand Portal die Ordnerstruktur (angefangen beim Stammordner) und die freigegebenen Ordner, die in den jeweiligen übergeordneten Ordnern angeordnet sind.

Bei diesen übergeordneten Ordnern handelt es sich um virtuelle Ordner, für die keine Aktionen ausgeführt werden können. Sie können diese virtuellen Ordner an einem Sperrsymbol erkennen.

Im Gegensatz zu freigegebenen Ordnern sind keine Aktionsaufgaben zu sehen, wenn Sie den Mauszeiger auf die Ordner bewegen oder sie in der **[!UICONTROL Kartenansicht]** auswählen. Die Schaltfläche **[!UICONTROL Überblick]** wird angezeigt, wenn Sie einen virtuellen Ordner in der **[!UICONTROL Spaltenansicht]** und in der **[!UICONTROL Listenansicht]** auswählen.

>[!NOTE]
>
>Beachten Sie, dass das Standardminiaturbild der virtuellen Ordner das Miniaturbild des ersten freigegebenen Ordners ist.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Freigeben von Ordnern {#how-to-share-folders}

Führen Sie folgende Schritte aus, um einen Ordner in Brand Portal für Benutzer freizugeben:

1. Klicken Sie links auf das Überlagerungssymbol und wählen Sie dann **[!UICONTROL Navigation]**.

   ![](assets/selectorrail.png)

1. Wählen Sie links in der Seitenleiste **[!UICONTROL Dateien]** aus.

   ![](assets/access_files.png)

1. Wählen Sie in der Brand Portal-Benutzeroberfläche den Ordner aus, den Sie freigeben möchten.

   ![](assets/share-folders.png)

1. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Freigeben]**.

   ![](assets/share_icon.png)

   Die Konsole [!UICONTROL Ordnereigenschaften] wird angezeigt.

   ![](assets/folder_properties.png)

1. Geben Sie in der Konsole **[!UICONTROL Ordnereigenschaften]** den Ordnertitel im Feld **[!UICONTROL Ordnertitel]** an, wenn den Benutzern der Standardname nicht angezeigt werden soll.
1. Wählen Sie aus der Liste **[!UICONTROL Benutzer hinzufügen]** den Benutzer oder die Gruppe aus, für den/die Sie den Ordner freigeben möchten, und klicken Sie auf **[!UICONTROL Hinzufügen]**.
Um den Ordner nur für Gastbenutzer und keine anderen Benutzer freizugeben, wählen Sie **[!UICONTROL Anonyme Benutzer]** aus dem Dropdown-Menü **[!UICONTROL Mitglieder]**.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Um den Ordner allen Benutzern unabhängig von ihrer Gruppenzugehörigkeit und -rolle zur Verfügung zu stellen, machen Sie ihn öffentlich, indem Sie das Kontrollkästchen **[!UICONTROL Öffentlicher Ordner]** aktivieren.

1. Klicken Sie, falls nötig, auf **[!UICONTROL Miniatur ändern]**, um das Miniaturbild für den Ordner zu ändern.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

1. Um auf den freigegebenen Ordner zuzugreifen, melden Sie sich bei Brand Portal mit den Anmeldeinformationen des Benutzers an, für den Sie den Ordner freigegeben haben. Überprüfen Sie den freigegebenen Ordner in der Benutzeroberfläche.

## Aufheben der Freigabe von Ordnern {#unshare-the-folders}

Gehen Sie wie folgt vor, um die vormalige Freigabe eines Ordners aufzuheben:

1. Wählen Sie in der Brand Portal-Benutzeroberfläche den Ordner aus, dessen Freigabe Sie aufheben möchten.

   ![](assets/share-folders-1.png)

1. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Freigeben]**.
1. Klicken Sie in der Konsole **[!UICONTROL Ordnereigenschaften]** unter **[!UICONTROL Mitglieder]** auf das **[!UICONTROL x]**-Symbol neben einem Benutzer um diesen aus der Liste der Benutzer zu entfernen, für die Sie den Ordner freigegeben haben.

   ![](assets/folder_propertiesunshare.png)

1. Klicken Sie in der Warnmeldung auf **[!UICONTROL Bestätigen]**, um das Aufheben der Freigabe zu bestätigen.
Klicken Sie auf **[!UICONTROL Speichern]**.

1. Melden Sie sich bei Brand Portal mit den Anmeldeinformationen des Benutzers an, den Sie aus der freigegebenen Liste entfernt haben. Der Ordner ist in der Brand Portal-Oberfläche für den Benutzer nicht mehr verfügbar.
