---
title: Versionshinweise
description: Hier erhalten Sie nützliche Informationen zu Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal Version 2024.10.0.
content-type: reference
contentOwner: Kirandeep Kour
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 3f3065de994f5c38e604b52848b0a538c9efd7d1
workflow-type: tm+mt
source-wordcount: '1533'
ht-degree: 76%

---

# Versionshinweise {#release-notes}

Hier erhalten Sie nützliche Informationen zu neuen Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal Version 2024.10.0.

## Versionshinweise {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2024.10.0 |
| Datum | Oktober 2024 |

## Übersicht {#overview}

Mit Adobe Experience Manager (AEM) Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzende auf allen Geräten verteilen. Es hilft, die Effizienz der gemeinsamen Nutzung von Assets zu verbessern, die Markteinführung von Assets zu beschleunigen und das Risiko der Nichteinhaltung von Vorschriften und des unbefugten Zugriffs zu verringern. Mit Brand Portal können Benutzer jederzeit und überall Assets durchsuchen, suchen, in der Vorschau anzeigen, herunterladen und in Formate exportieren, die vom Unternehmen genehmigt wurden.

## Neue Funktionen in Version 2024.10.0 {#whats-new-in-2024.10.0}

### Behobene kritische Probleme {#critical-issues-fixed}

#### Fehlerbehebungen {#bug-fixes}

Diese Version enthält die folgenden Fehlerbehebungen:

* Die E-Mail-Benachrichtigungen für die Beschaffung von Importereignissen werden nicht gesendet.
* Bei Verwendung des Suchfilters zeigt [!DNL Brand Portal] doppelte Ordner im Suchfilterfenster an.
* Der Download von Sammlungen mit nicht lizenzierten Assets mit Sonderzeichen in ihren Namen funktioniert nicht.
* Beim Navigieren zum [!UICONTROL Suchformular-Editor] werden Kennzeichnungen nicht lokalisiert.
* Kennzeichnungen werden im Fenster „Link-Freigabe“ nicht lokalisiert.
* Video mit Sonderzeichen im Namen kann nicht heruntergeladen werden.
* Das Veröffentlichen und Rückgängigmachen der Veröffentlichung von Assets aus [!DNL Adobe Experience Manager Assets] in Brand Portal funktioniert nicht ordnungsgemäß.
* Aus der Brand Portal heruntergeladene Videos können nicht wiedergegeben werden.

## Frühere Versionen

### Version Februar 2024 {#feb-2024}

**Fehlerbehebungen und Verbesserungen**

Diese Version enthält die folgenden Fehlerbehebungen:

* Mit DRM geschützte digitale Assets im türkischen Gebietsschema können nicht heruntergeladen werden.
* Die vorhandenen Berichte mit Assets mit mehrzeiligem Titel können nicht geöffnet und heruntergeladen werden.
* Wenn Sie Assets über die Schaltfläche [!UICONTROL Herunterladen] in der Aktionsleiste herunterladen, werden maximal 1.000 Assets heruntergeladen.
* Falscher Name von Assets vom Typ PSD bei der Anzeige in der Inhaltsstruktur.
* Die Option [!UICONTROL Ausgabedarstellung löschen] auf der Asset-Detailseite funktioniert nicht.
* Titel und Größe der Assets sind im Download-Popup-Fenster falsch ausgerichtet.
* Beim Erstellen eines Berichts sind Beschriftungen nicht lokalisiert.
* Support-Admins wurden in Brand Portal als Admins benannt.

### Version Oktober 2023 {#oct-2023}

**Fehlerbehebungen und Verbesserungen**
Diese Version umfasst die folgenden Verbesserungen:

* Leistungsverbesserungen beim Durchsuchen von [!UICONTROL Sammlungen].

* Verbesserungen bei den Suchergebnissen bei der Durchführung einer partiellen Suche mithilfe des OmniSearch-Felds.

Diese Version enthält die folgenden Fehlerbehebungen:

* Speicherung der Eigeschaften von [!UICONTROL Datum] und [!UICONTROL Optionen] in der [!UICONTROL Smart-Sammlung] nicht möglich.

* Das Format für [!UICONTROL Datum und Uhrzeit] ist bei der Arbeit mit einem anderen Gebietsschema als Englisch inkonsistent.

* Bei der Suche nach Assets [!UICONTROL  die Schaltfläche ]Löschen“.

* Wenn das Feld [!UICONTROL Titel] mehrere Multibyte-Symbole in der [!UICONTROL Link-Freigabe] enthält, kann der Bericht nicht heruntergeladen werden.

* Beim Anzeigen eines PDF-Dokuments sind die Beschriftungen und QuickInfos nicht lokalisiert.

### Version August 2023 {#aug-2023}

**Fehlerbehebungen und Verbesserungen**
Diese Version umfasst die folgenden Verbesserungen:

* Leistungsverbesserungen beim Laden von Assets über das Popup [!UICONTROL Herunterladen].
* Wenn Sie ein Asset oder eine Ausgabedarstellung eines Assets herunterladen, wird es jetzt in seinem ursprünglichen Dateiformat und nicht mehr als Zip-Datei heruntergeladen.

Diese Version enthält die folgenden Fehlerbehebungen:

* Bei Suchfiltern werden lange Beschriftungen oder Tags nicht richtig angezeigt.
* Lange Ausgabedarstellungsnamen können nicht im Dialogfeld „Herunterladen“ angezeigt werden.
* Die Vorschau von Video-Assets in der Kartenansicht ist nicht möglich.

### Version Mai 2023 {#may-2023}

**Fehlerbehebungen**
Diese Version enthält Fehlerbehebungen für die folgenden kritischen Probleme:

* Wenn beim Herunterladen eines Assets von einem freigegebenen Link ein Fehler auftritt, werden die Kennzeichnungen `Notice` und `Close` in der Fehlermeldung nicht lokalisiert.
* Brand Portal zeigt beim Zugriff auf Suchfilter mit dem `Filter`-Bereich den Fehler **Anfragekopfzeilenfelder zu groß** an.

**Bekannte Probleme**
Diese Version enthält die folgenden bekannten Probleme:

* Teilweise Lokalisierung des Inhalts eines Asset-Beschaffungs-Berichts.
* Nur wenige Felder des Benutzerprofils können im Benutzerprofil nicht bearbeitet werden.

### Version Februar 2023 {#feb-2023}

**Fehlerbehebungen**

Diese Version umfasst Fehlerbehebungen für die folgenden kritischen Probleme:

* Profilbild kann nicht im Brand Portal aktualisiert werden.
* Die Größe des Inhaltsstrukturbereichs kann nicht geändert werden. Wenn der Dateiname länger als die Standardbreite der Inhaltsstruktur ist, können Sie die Inhaltsstruktur nicht sowohl horizontal als auch vertikal ziehen. Daher sind längere Dateinamen nicht lesbar.
* Die Suchergebnisse sind für dasselbe Eigenschaftsprädikat inkonsistent, das zweimal in den Suchformularen verwendet wird.
* Der Text auf den zwischengeschalteten Anmeldeseiten ist nicht in allen Sprachen lokalisiert.

**Verbesserungen**

Diese Version umfasst die folgenden Verbesserungen:

* Für eine verbesserte Vorschau der PDF-Assets ist jetzt ein neuer, moderner PDF-Viewer verfügbar.
* Jetzt können Sie Benachrichtigungen zur Asset-Beschaffung für Admins aktivieren oder deaktivieren. Navigieren Sie zu [!UICONTROL Allgemeine Einstellungen] und aktivieren oder deaktivieren Sie [!UICONTROL `Notify Administrator of asset contribution`].

  ![Admin über den Asset-Beitrag benachrichtigen](assets/notify-admin.png)

* Nicht autorisierte Benutzende können keinen Zugriff auf das Brand Portal anfordern, wenn der Anforderungszugriff deaktiviert ist.
* Nur die Organisationen, die für das Brand Portal bereitgestellt wurden, werden in der Profilauswahlliste angezeigt.

**Bekannte Probleme**

Diese Version weist die folgenden bekannten Probleme auf:

* Teilweise Lokalisierung des Inhalts eines Asset-Beschaffungs-Berichts.
* Nur wenige Felder des Benutzerprofils können im Benutzerprofil nicht bearbeitet werden.

### Version Oktober 2022 {#oct-2022}

**Behobene kritische Probleme**

Diese Version umfasst Fehlerbehebungen für die folgenden kritischen Probleme:

* Langsame Reaktionszeiten beim Kopieren großer Dateien aus Brand Portal in ein Tool eines Drittanbieters.
* Wenn Sie das Kontrollkästchen „Zählung der Ausgabedarstellungen“ aktivieren, werden die Kontrollkästchen zur Auswahl einzelner Ausgabedarstellungen deaktiviert.
* Langsame Reaktionszeit für die Suche.

>[!IMPORTANT]
>
>Pulse-Benachrichtigungen in der AEM Assets Brand Portal werden ab dem 1. Dezember 2022 eingestellt. Anstelle von Pulse-Benachrichtigungen erhalten Sie weiterhin E-Mail-Benachrichtigungen für die folgenden Ereignisse:
>
>* Freigeben von Assets über einen Link
>* Workflow zum Anfordern von Zugriff
>* Freigeben von Beitragsordnern
>* Export nach AEM starten
>* Abgeschlossener Export nach AEM
>

### Version August 2022 {#aug-2022}

**Behobene kritische Probleme**

Diese Version umfasst Fehlerbehebungen für die folgenden kritischen Probleme:

* Wenn NUI ein Asset in Experience Manager nicht verarbeiten kann, zeigt Brand Portal einen ungenauen Asset-Importstatus an.
* Wenn die Vorschauaktion fehlschlägt, gibt es keine Benachrichtigung, um den Fehler zu melden.
* Der ungenaue Wert für die `totalUploadedSize`-Eigenschaft für jedes Asset wird behoben.
* Wenn Sie auf **Alle Elemente herunterladen** klicken und eine große Anzahl von Ausgabedarstellungen für ein Asset verfügbar ist, lädt Brand Portal eine ungültige ZIP-Datei herunter.
* Die Übersetzung einiger Zeichenfolgen wird auf der Benutzeroberfläche von Brand Portal abgeschnitten.

### Version Mai 2022 {#may-2022}

**Neue Funktionen**

Brand Portal führt nun alle zwölf Stunden automatische Aufträge aus, um alle in AEM veröffentlichten Brand Portal-Assets zu löschen. Daher müssen Sie die Assets im Beitragsordner nicht manuell löschen, um die Ordnergröße unter dem Schwellenwert zu halten.

**Behobene kritische Probleme**

Diese Version umfasst Fehlerbehebungen für die folgenden kritischen Probleme:

* Wenn Sie einen Ordner oder eine Sammlung herunterladen, der bzw. die Assets mit farbigen Tags enthält, wird auch eine XML-Datei heruntergeladen.
* Wenn Sie ein Video mit Ausgabeformaten herunterladen, erstellt Brand Portal eine ungültige ZIP-Datei.
* Wenn Sie Vorgaben und Assets in der AEM-Autoreninstanz erstellen und dann in Brand Portal veröffentlichen, können Sie beim Herunterladen der Assets dynamische Ausgabedarstellungen auswählen. Sie können die heruntergeladene ZIP-Datei jedoch nicht extrahieren. Dieses Problem verhindert den Zugriff auf den heruntergeladenen Inhalt.
* Probleme beim Herunterladen von Video-Assets aus bestimmten in Brand Portal verfügbaren Ordnern.
* Wenn Sie die URL des Beitragsordners per E-Mail versenden, haben die Rollen „Betrachter“ und „Bearbeiter“ Probleme, über den Breadcrumb auf den übergeordneten Ordner zuzugreifen.
* Bei der Beschaffung eines veröffentlichten Berichts wird eine falsche Auftragsstartzeit angezeigt.

### Version Februar 2022 {#feb-2022}

**Neue Funktionen**

* Der Schwellenwert für den Sitzungs-Timeout für Gastbenutzer wurde von 2 Stunden auf 15 Minuten verringert.
* Die zusätzliche Option **[!UICONTROL Seiten anzeigen]** wurde für mehrseitige PDF-Dateien entfernt, da der Benutzer die PDF-Seiten jetzt über Adobe Document Cloud Viewer anzeigen kann.
* Benutzer können keine Ordner suchen, in ihnen navigieren oder sie öffnen. Die Benutzeroberfläche zeigt die Fehlermeldung: `Failed to load data`.
* Im Bedienfeld **[!UICONTROL Ausgabedarstellungen]** werden nicht alle statischen Ausgabedarstellungen der Assets aufgelistet, die in Brand Portal veröffentlicht wurden.
* Im Bedienfeld **[!UICONTROL Ausgabedarstellungen]** werden zwar die Ausgabedarstellungen für den intelligenten Zuschnitt des Assets aufgelistet, der Benutzer kann jedoch die Ausgabedarstellungen für den intelligenten Zuschnitt nicht in der Vorschau anzeigen oder herunterladen.
* Im Dialogfeld „Herunterladen“ werden die Ausgabedarstellungen für den intelligenten Zuschnitt des ausgewählten Assets aufgelistet. Der Benutzer kann die Ausgabedarstellungen für den intelligenten Zuschnitt jedoch nicht herunterladen.
* Ein Benutzer ohne Administratorrechte erhält beim Herunterladen eines Assets nur die ursprüngliche Ausgabedarstellung des Assets. Die System- und benutzerdefinierten Ausgabedarstellungen werden nicht heruntergeladen.
* Wenn ein Suchfilter zum Herunterladen eines Assets angewendet wird, ist die Schaltfläche „`Download`“ im Download-Dialogfeld deaktiviert, sodass der Benutzer das Asset nicht herunterladen kann.
* Wenn „`Smart Tags`“ und (oder) „`Color Tags`“ aktiviert sind, listet der Download-Dialog die `json`-Dateien als Wiedergabeversionen auf und lädt diese `json`-Dateien in den archivierten Zip-Ordner herunter.
* Die anonymen Benutzer können Assets nicht über einen freigegebenen Link herunterladen, da der Link zur Brand Portal-Anmeldeseite weiterleitet.
* Das System spiegelt nicht den korrekten Wert für die Anzahl der aktiven gleichzeitigen Benutzer wider.

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.

* The users are unable to search, navigate, or open folders. The user interface reflects the error message: `Failed to load data`. 
* The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal.
* The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
* The download dialog lists the smart crop renditions of the selected asset, however, the user cannot download the smart crop renditions. 
* A non-admin user is getting only the original asset rendition when downloading an asset. The system and custom renditions are not downloaded.  
* When applying search filter to download an asset, the `Download` button is disabled in the download dialog and does not allows the user to download the asset.
* If `Smart Tags` and (or) `Color Tags` are enabled, the download dialog lists the `json` files as renditions and downloads these `json` files in the archived zip folder.
* The anonymous users are unable to download assets using a shared link because the link redirects to the Brand Portal login page. 
* The system is not reflecting the correct value for the number of active concurrent users.
-->

<!--
### New features {#new-features}

Brand Portal now executes automatic jobs every twelve hours to delete all Brand Portal assets that are published to AEM. As a result, you do not need to delete the assets in the Contribution folder manually to keep the folder size below the threshold limit. See [What's new in Experience Manager Assets Brand Portal](whats-new.md).
-->

<!--
This release includes fixes to the following critical issues:

* When you download a folder or a collection that includes assets with color tags, an XML file gets downloaded as well.

* When you download a video that includes renditions, Brand Portal creates an invalid .ZIP file.

* When you create presets and assets on AEM author and publish them to Brand Portal and then select dynamic renditions while downloading the assets, you cannot extract the downloaded .ZIP file.

* Issues while downloading video assets from certain folders available on Brand Portal.

* When you share the Contribution folder's URL using an email, Viewer and Editor roles face issues while accessing its parent folder using the breadcrumb.

* Sourcing published report displays an incorrect job start time.
>
 
<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Sprachen {#languages}

Die Benutzeroberfläche von Brand Portal ist in den folgenden Sprachen verfügbar:

* Englisch
* Deutsch
* Französisch
* Spanisch
* Italienisch
* Brasilianisches Portugiesisch
* Japanisch
* Vereinfachtes Chinesisch
* Koreanisch

## Zertifizierte Plattformen {#certified-platforms}

Informationen dazu, welche Plattformen für diese Brand Portal-Version zertifiziert sind, finden Sie in der Spalte **Unterstützung für Touch** optimierte Benutzeroberfläche) im Abschnitt **Unterstützte Browser für die Authoring-** von [Technische Anforderungen](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/implementing/deploying/introduction/technical-requirements).

## Links {#links}

* [Adobe Experience Manager-Produktseite unter adobe.com](https://business.adobe.com/de/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal-Dokumentation](https://experienceleague.adobe.com/en/docs/experience-manager-brand-portal/using/home)

## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kundinnen und Kunden verfügbar. Wenn Sie eine Kundin oder ein Kunde sind und Zugriff benötigen, wenden Sie sich an die Adobe-Kundenbetreuung.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
