---
title: Konfigurieren und Veröffentlichen des Beitragsordners aus Experience Manager Assets in Brand Portal
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration und Veröffentlichung eines Beitragsordners aus Experience Manager Assets in Brand Portal.
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 3845d9fa17e75d59493383303ca0978349ca0401
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 100%

---

# Konfigurieren des Beitragsordners in Experience Manager Assets {#configure-contribution-folder}

Bei der gemeinsamen Asset-Beschaffung können Experience Manager Assets-Benutzer (Administratoren und Benutzer ohne Administratorrechte) neue Ordner des Typs **Asset-Beitrag** erstellen, um sicherzustellen, dass die neu erstellten Ordner von Brand Portal-Benutzern für die Übermittlung von Assets nutzbar sind.  Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens **FREIGEGEBEN** und **NEU** im neu erstellten **Beitragsordner** erstellt werden.

Der Experience Manager Assets-Benutzer definiert dann die Asset-Anforderungen, indem er eine Zusammenfassung der Asset-Typen, die zum Beitragsordner hinzugefügt werden sollen, sowie eine Reihe von Grundlinien-Assets in den Ordner **FREIGEGEBEN** hochlädt, um sicherzustellen, dass Brand Portal-Benutzer über die benötigten Informationen verfügen. Der Administrator kann aktiven Brand Portal-Benutzern anschließend Zugriff auf den Beitragsordner gewähren, bevor der neu erstellte Beitragsordner in Brand Portal veröffentlicht wird.

Das folgende Video zeigt, wie Sie einen Beitragsordner in Experience Manager Assets konfigurieren:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Der Experience Manager Assets-Benutzer führt beim Konfigurieren eines Beitragsordners die folgenden Aktivitäten aus:

* [Erstellen von Beitragsordnern](#create-contribution-folder)
* [Hochladen von Asset-Anforderungen und Zuweisen von Beitragenden](#configure-contribution-folder-properties)
* [Hochladen von Grundlinien-Assets](#uplad-new-assets-to-contribution-folder)
* [Veröffentlichen des Beitragsordners aus Experience Manager Assets in Brand Portal](#publish-contribution-folder-to-brand-portal)

## Erstellen von Beitragsordnern {#create-contribution-folder}


Experience Manager Assets-Administratoren und Benutzer ohne Administratorrechte, die zum Erstellen eines neuen Ordners berechtigt sind, können in Experience Manager Assets einen Beitragsordner erstellen.
Um einen Beitragsordner zu erstellen, erstellen Sie einen neuen Ordner des Typs Asset-Beitrag und stellen Sie sicher, dass der neu erstellte Ordner von Brand Portal-Benutzern für die Übermittlung von Assets nutzbar ist.  Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens SHARED und NEW im Beitragsordner erstellt werden.


>[!NOTE]
>
>Administratoren können mehrere Asset-Beitragsordner in einem Ordner erstellen.
>
>Ein Asset-Beitragsordner enthält die Ordner NEU und FREIGEGEBEN für Verteilung und Beitrag von Assets. Erstellen Sie keinen Assets, Ordner oder Beitragsordner in einem Beitragsordner.


Sie können die Eigenschaften des Beitragsordners sowohl separat als auch beim Erstellen des Beitragsordners konfigurieren. In diesem Beispiel konfigurieren wir die Eigenschaften separat.

**Erstellen eines Beitragsordners:**

1. Melden Sie sich bei Ihrer Experience Manager Assets-Instanz an.

1. Gehen Sie zu **[!UICONTROL Assets]** > **[!UICONTROL Dateien]**. Es werden alle vorhandenen Ordner im Experience Manager Assets-Repository aufgelistet.

1. Klicken Sie auf **[!UICONTROL Erstellen]**, um einen neuen Ordner zu erstellen. Das Dialogfeld **[!UICONTROL Ordner erstellen]** wird geöffnet.

1. Geben Sie **[!UICONTROL Titel]** und **[!UICONTROL Name]** des Ordners ein und aktivieren Sie das Kontrollkästchen **[!UICONTROL Asset-Beiträge]**.
Wir empfehlen, Kleinbuchstaben ohne Leerzeichen zu verwenden, um den Ordner zu benennen.

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Der Beitragsordner wird im Experience Manager Assets-Repository aufgelistet.

   >[!NOTE]
   >
   >Ein Benutzer ohne Administratorrechte kann einen Asset-Beitragsordner erstellen und freigeben, ihn jedoch nicht ändern oder löschen.


   ![](assets/create-contribution-folder.png)

1. Klicken Sie, um den Beitragsordner zu öffnen. Es werden zwei Unterordner angezeigt: **[!UICONTROL FREIGEGEBEN]** und **[!UICONTROL NEU]**. Diese werden automatisch im Beitragsordner erstellt.

   ![](assets/contribution-folder.png)


## Konfigurieren von Eigenschaften von Beitragsordnern {#configure-contribution-folder-properties}

Der Experience Manager Assets-Administrator führt beim Konfigurieren der Eigenschaften eines Beitragsordners die folgenden Aktivitäten aus.

* **Beschreibung hinzufügen**: Geben Sie eine allgemeine Beschreibung des Beitragsordners ein.
* **Zusammenfassung hochladen**: Laden Sie das Asset-Anforderungsdokument hoch, das Asset-bezogene Informationen enthält.
* **Beitragende hinzufügen**: Fügen Sie Brand Portal-Benutzer hinzu, um ihnen Zugriff auf den Beitragsordner zu gewähren.

Die Asset-Anforderung bezieht sich auf die Details, die von Administratoren bereitgestellt werden, um Beitragende (Brand Portal-Benutzer) dabei zu unterstützen, die Notwendigkeit und Anforderungen des Beitragsordners zu verstehen. Der Administrator lädt ein Asset-Anforderungsdokument hoch, das eine Zusammenfassung des Asset-Typs enthält, der dem Beitragsordner hinzugefügt werden soll, sowie Asset-bezogene Informationen, wie z. B. Zweck, Typ der Bilder, maximale Größe usw.

**Konfigurieren von Eigenschaften von Beitragsordnern:**

1. Melden Sie sich bei Ihrer Experience Manager Assets-Instanz an.

1. Navigieren Sie zu **[!UICONTROL Assets > Dateien]** und suchen Sie nach dem Beitragsordner.
1. Wählen Sie den Beitragsordner aus und klicken Sie auf **[!UICONTROL Eigenschaften]**, um das Fenster „Ordnereigenschaften“ zu öffnen.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Navigieren Sie zur Registerkarte **[!UICONTROL Asset-Beitrag]**.
1. Geben Sie eine allgemeine **[!UICONTROL Beschreibung]** des Beitragsordners ein.
1. Klicken Sie auf **[!UICONTROL Zusammenfassung hochladen]**, um von Ihrem lokalen Computer aus zu navigieren und ein **Asset-Anforderungsdokument** hochzuladen.

   ![](assets/upload.png)

1. Geben Sie im Feld **[!UICONTROL Benutzer hinzufügen]** Brand Portal-Benutzer an, für die Sie den Beitragsordner freigeben möchten. Diese Benutzer können über die Brand Portal-Oberfläche Inhalte in diesem Beitragsordner abrufen oder in ihn hochladen.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Die Suchergebnisse basieren auf der in Experience Manager Assets konfigurierten Brand Portal-Benutzerliste. Stellen Sie sicher, dass Sie über die aktualisierte Brand Portal-Benutzerliste verfügen.

Administratoren können die Datei `user.csv` aus der [!DNL Admin Console] nutzen und als Basisvorlage zum Hinzufügen von Brand Portal-Benutzern verwenden. Navigieren Sie zu [!UICONTROL Benutzer] und klicken Sie auf die Option [!UICONTROL Benutzerliste in CSV exportieren], um die Datei `users.csv` herunterzuladen. Die folgende Beispiel-Benutzerliste enthält die Attribute, die zum Hinzufügen der Benutzer erforderlich sind. Das einzige obligatorische Attribut für einen Benutzereintrag ist die `Email`. Alle anderen Attribute sind optional.

[Datei laden](assets/users.csv)

## Hochladen von Assets in den Beitragsordner {#uplad-new-assets-to-contribution-folder}

Ein Benutzer von Experience Manager Assets lädt eine Reihe von Grundlinien-Assets in den Ordner **FREIGEGEBEN**, um sicherzustellen, dass die Benutzer von Brand Portal über die benötigten Informationen verfügen.

**Hochladen von Grundlinien-Assets:**

1. Melden Sie sich bei Ihrer Experience Manager Assets-Instanz an.

1. Navigieren Sie zu **[!UICONTROL Assets > Dateien]** und suchen Sie nach dem Beitragsordner.

1. Wählen Sie den Beitragsordner aus und klicken Sie darauf, um ihn zu öffnen.

1. Klicken Sie auf den **[!UICONTROL Ordner NEU]**.

   ![](assets/upload-new-assets1.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]** > **[!UICONTROL Dateien]**, um einzelne Dateien oder Ordner (.zip) mit mehreren Assets hochzuladen.

   ![](assets/upload-new-assets2.png)

1. Suchen Sie nach Assets (Dateien/Ordner) und laden Sie sie in den Ordner **[!UICONTROL NEU]** hoch.

   ![](assets/upload-asset4.png)

Nachdem Sie alle Assets oder Ordner in den Ordner „NEU“ hochgeladen haben, veröffentlichen Sie den Beitragsordner in Experience Manager Assets.


## Veröffentlichen von Beitragsordnern in Brand Portal {#publish-contribution-folder-to-brand-portal}

Sobald der Beitragsordner konfiguriert ist, kann der Experience Manager Assets-Benutzer (Administratoren/Benutzer ohne Administratorrechte) den Beitragsordner aus Experience Manager Assets in Brand Portal veröffentlichen. Brand Portal-Benutzer, die Zugriff auf den Beitragsordner haben, erhalten nach Abschluss der Veröffentlichungsaktion eine E-Mail-/Pulsbenachrichtigung.


**Veröffentlichen des Beitragsordners:**

1. Melden Sie sich bei Ihrer Experience Manager Assets-Instanz an.

1. Navigieren Sie zu **[!UICONTROL Assets > Dateien]** und suchen Sie nach dem Beitragsordner, in dem Sie in Brand Portal veröffentlichen möchten.
1. Wählen Sie den Beitragsordner aus und klicken Sie auf **[!UICONTROL Quick Publish]** > **[!UICONTROL In Brand Portal veröffentlichen]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   Sie erhalten eine Erfolgsmeldung, sobald der Beitragsordner in Brand Portal veröffentlicht wurde.

Eine E-Mail-/Pulsbenachrichtigung wird an die Brand Portal-Benutzer gesendet, die dem Beitragsordner zugewiesen sind. Die Brand Portal-Benutzer können auf den Beitragsordner zugreifen und mit dem Beitrag beginnen. Weitere Informationen finden Sie unter [Hochladen von Assets in den Beitragsordner und Veröffentlichen in Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
