---
title: Freigeben von Ordnern
seo-title: Share folders
description: Brand Portal unterstützt keine Asset-Aufnahme, sodass Assets aus einer vorkonfigurierten Experience Manager Assets-Autoreninstanz in Brand Portal veröffentlicht werden müssen. Brand Portal-Benutzer ohne Administratorrechte können nicht auf veröffentlichte Assets zugreifen, sofern sie nicht bei der Konfiguration der Replikation mit der Experience Manager-Instanz konfiguriert wurden. Stattdessen müssen sie für diese Benutzer freigegeben werden.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 80%

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

Die Zugriffsrechte für die Assets eines Ordners hängen von den Zugriffsrechten für den jeweiligen übergeordneten Ordner ab, unabhängig von den Einstellungen der untergeordneten Ordner. Dieses Verhalten wird in AEM durch [ACLs](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html?lang=de) gesteuert, da untergeordnete Ordner die ACLs von den jeweiligen übergeordneten Ordnern erben. Wenn beispielsweise Ordner A den Ordner B enthält und dieser wiederum den Ordner C, haben Benutzergruppen (oder Benutzer), die Zugriffsrechte für Ordner A haben, auch dieselben Zugriffsrechte für Ordner B und Ordner C. Da Ordner B dem Ordner A untergeordnet ist, erbt er die ACLs von Ordner A. Und da Ordner C dem Ordner B untergeordnet ist, erbt er die ACLs von Ordner B.

Entsprechend haben Benutzergruppen (oder Benutzer), die nur Zugriffsberechtigungen für den Ordner B haben, dieselben Berechtigungen für den Ordner C, aber nicht für Ordner A. Daher wird empfohlen, dass Unternehmen ihre Inhalte so anordnen, dass die am meisten exponierten Assets in die untergeordneten Ordner eingefügt werden. Der Zugriff vom untergeordneten Ordner auf den Stammordner kann eingeschränkt werden.

### Veröffentlichen von öffentlichen Ordnern {#public-folder-publish}

Sofern die Option **[!UICONTROL Öffentlichen Ordner veröffentlichen]** bei der Konfiguration der Brand Portal-Replikation nicht aktiviert wurde, haben Benutzer ohne Administratorrechte (z. B. Bearbeiter und Betrachter) keinen Zugriff auf Assets, die aus AEM Assets in Brand Portal veröffentlicht wurden.

![](assets/assetbpreplication.png)

Wenn die Option **[!UICONTROL Öffentlichen Ordner veröffentlichen]** deaktiviert ist, müssen Administratoren diese Assets mithilfe der Freigabefunktion speziell für Benutzer ohne Administratorrechte freigeben.

>[!NOTE]
>
>Die Option **[!UICONTROL Veröffentlichung eines öffentlichen Ordners]** ist ab AEM-Version 6.3.2.1 verfügbar.

## Zugriff auf freigegebene Ordner {#access-to-shared-folders}

In der folgenden Matrix werden die Zugriffsberechtigungen und die Berechtigungen für Freigabe/Aufheben der Freigabe für verschiedene Benutzerrollen dargestellt:

|               | Zugriff auf alle Ordner, die aus AEM Assets in Brand Portal veröffentlicht wurden | Zugriff auf freigegebene Ordner | Freigeben/Aufheben der Freigabe von Ordnerberechtigungen |
|---------------|-----------|-----------|------------|
| Administrator | Ja | Ja | Ja |
| Bearbeiter | Nein* | Ja nur, wenn es für sie oder die Gruppe freigegeben wurde, zu der sie gehören | Ja, nur für die Ordner, die für die Benutzer oder deren Gruppe freigegeben wurden |
| Betrachter | Nein* | Ja nur, wenn es für sie oder die Gruppe freigegeben wurde, zu der sie gehören | Nein |
| Gastbenutzer | Nein* | Ja nur, wenn es für sie oder die Gruppe freigegeben wurde, zu der sie gehören | Nein |

>[!NOTE]
>
>Standardmäßig ist die Option **[!UICONTROL Öffentlichen Ordner veröffentlichen]** bei der Konfiguration der Replikation von Brand Portal mit der AEM-Autoreninstanz deaktiviert. Wenn die Option aktiviert ist, können standardmäßig alle Benutzer (auch Benutzer ohne Administratorrechte) auf die in Brand Portal veröffentlichten Ordner zugreifen.

### Zugriff von Benutzern ohne Administratorrechte auf freigegebene Ordner {#non-admin-user-access-to-shared-folders}

Benutzer ohne Administratorrechte können nur auf die Ordner zugreifen, die in Brand Portal für sie freigegeben sind. Wie diese Ordner jedoch im Portal angezeigt werden, wenn sich die Benutzer anmelden, hängt von den Einstellungen der Konfiguration **[!UICONTROL Ordnerhierarchie aktivieren]**.

**Wenn die Konfiguration deaktiviert ist**

Benutzer ohne Administratorrechte sehen bei der Anmeldung bei der Brand Portal alle Ordner, die für sie auf der Landingpage freigegeben wurden.

![](assets/disabled-folder-hierarchy1-1.png)

**Wenn die Konfiguration aktiviert ist**

Benutzer ohne Administratorrechte sehen bei der Anmeldung bei Brand Portal die Ordnerstruktur (angefangen beim Stammordner) und die freigegebenen Ordner, die in den jeweiligen übergeordneten Ordnern angeordnet sind.

Diese übergeordneten Ordner sind virtuelle Ordner und für sie können keine Aktionen durchgeführt werden. Sie können diese virtuellen Ordner an einem Sperrsymbol erkennen.

Im Gegensatz zu freigegebenen Ordnern sind keine Aktionsaufgaben zu sehen, wenn Sie den Mauszeiger auf die Ordner bewegen oder sie in der **[!UICONTROL Kartenansicht]** auswählen. Die Schaltfläche **[!UICONTROL Überblick]** wird angezeigt, wenn Sie einen virtuellen Ordner in der **[!UICONTROL Spaltenansicht]** und **[!UICONTROL Listenansicht]** auswählen.

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
