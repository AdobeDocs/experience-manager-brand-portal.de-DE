---
title: Hochladen von Assets und Veröffentlichen des Beitragsordners von Brand Portal aus in Experience Manager Assets
description: Hier erhalten Sie einen Einblick in das Hochladen neuer Assets und das Veröffentlichen des Beitragsordners von Brand Portal aus in Experience Manager Assets.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 10f89ded6febb1a024cbe181fa48a290d90223f0
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 73%

---

# Veröffentlichen des Beitragsordners in Experience Manager Assets {#using-asset-souring-in-bp}

Brand Portal-Benutzer mit entsprechender Berechtigung können mehrere Assets oder Ordner mit mehreren Assets in den Beitragsordner hochladen. Brand Portal-Benutzer können jedoch nur Assets in den Ordner **NEU** hochladen. Der **FREIGEGEBEN**-Ordner ist für die Verteilung von Grundlinien-Assets (Referenzinhalten) vorgesehen, die von den Brand Portal-Benutzern beim Erstellen neuer Assets für den Beitrag verwendet werden.

Brand Portal-Benutzer mit Zugriffsberechtigung auf den Beitragsordner können die folgenden Aktivitäten ausführen:

* [Herunterladen von Asset-Anforderungen](#download-asset-requirements)
* [Hochladen von neuen Assets in den Beitragsordner](#uplad-new-assets-to-contribution-folder)
* [Veröffentlichen des Beitragsordners in Experience Manager Assets](#publish-contribution-folder-to-aem)

## Herunterladen von Asset-Anforderungen {#download-asset-requirements}

Brand Portal-Benutzer erhalten automatisch E-Mail- und Push-Benachrichtigungen, wenn ein Experience Manager Assets-Benutzer einen Beitragsordner freigibt. Dieser Workflow ermöglicht das Herunterladen der Zusammenfassung (Asset-Anforderungsdokument) und der Grundlinien-Assets (Referenzinhalte) aus dem Ordner **FREIGEGEBEN**, um die Asset-Anforderungen zu verstehen.

Der Brand Portal-Benutzer führt die folgenden Aktivitäten aus, um Asset-Anforderungen herunterzuladen:

* **Zusammenfassung herunterladen** - Zum Herunterladen der Zusammenfassung (Dokument mit den Asset-Anforderungen), die dem Beitragsordner angehängt ist. Es enthält Asset-bezogene Informationen wie den Typ der Assets, den Zweck, unterstützte Formate, die maximale Asset-Größe und mehr.
* **Herunterladen von Grundlinien-Assets** - Laden Sie die Grundlinien-Assets herunter, die zum Verständnis der erforderlichen Asset-Typen verwendet werden können. Brand Portal-Benutzer können diese Assets als Referenz verwenden, um neue Assets für Beiträge zu erstellen.

Das Brand Portal-Dashboard enthält alle vorhandenen Ordner, die dem Brand Portal-Benutzer zur Verfügung stehen, sowie den neu freigegebenen Beitragsordner. In diesem Beispiel hat der Brand Portal-Benutzer nur Zugriff auf den neu erstellten Beitragsordner. Es wird kein anderer vorhandener Ordner für den Benutzer freigegeben.

**Herunterladen von Asset-Anforderungen:**

1. Melden Sie sich bei Ihrer Brand Portal-Instanz an.
1. Wählen Sie im Brand Portal-Dashboard einen Beitragsordner aus.
1. Klicken Sie auf **[!UICONTROL Eigenschaften]**. Das Fenster „Eigenschaften“ mit den Details zum Beitragsordner wird geöffnet.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. Klicken Sie auf die Option **[!UICONTROL Mandat herunterladen]**, um das Asset-Anforderungsdokument auf Ihren lokalen Computer herunterzuladen.

   ![](assets/download.png)

1. Gehen Sie zurück zum Brand Portal-Dashboard.
1. Klicken Sie auf den Beitragsordner, um ihn zu öffnen. Sie können zwei Unterordner sehen: **[!UICONTROL FREIGEGEBEN]** und **[!UICONTROL NEU]** im Beitragsordner. Der Ordner „FREIGEGEBEN“ enthält alle Grundlinien-Assets (Referenzinhalte), die von den Administratoren freigegeben werden.
1. Sie können den Ordner **[!UICONTROL FREIGEGEBEN]** mit allen Grundlinien-Assets auf Ihren lokalen Computer herunterladen.
Alternativ können Sie den Ordner **[!UICONTROL FREIGEGEBEN]** öffnen und auf das Symbol **Herunterladen** klicken, um einzelne Dateien/Ordner herunterzuladen.

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

Sehen sie sich die Zusammenfassung (Asset-Anforderungsdokument) und die Grundlinien-Assets an, um die Asset-Anforderungen zu verstehen. Jetzt können Sie neue Assets für den Beitrag erstellen und sie in den Beitragsordner hochladen.

## Hochladen von Assets in den Beitragsordner {#upload-new-assets-to-contribution-folder}

Nachdem Sie die Asset-Anforderungen durchlaufen haben, können die Brand Portal-Benutzer neue Assets erstellen und sie in den Ordner „NEU“ im Beitragsordner hochladen. Ein Benutzer kann mehrere Assets in einen Asset-Beitragsordner hochladen. Es kann jedoch jeweils nur ein Ordner erstellt werden.

>[!NOTE]
>
>Brand Portal-Benutzer können Assets (maximal zwei Gigabyte pro Dateigröße) in den Ordner „NEU“ hochladen.
>
>Der Upload-Grenzwert für jeden Brand Portal-Mandanten beträgt 10 Gigabyte. Dies ist der kumulative Wert für alle Beitragsordner.
>
>Die in Brand Portal hochgeladenen Assets werden nicht für Ausgabedarstellungen verarbeitet und enthalten keine Vorschauen.

>[!NOTE]
>
>Adobe empfiehlt, den Upload-Bereich nach der Veröffentlichung des Beitragsordners in Experience Manager Assets freizugeben, damit er für die anderen Brand Portal-Benutzer verfügbar ist.
>
>Wenn Sie die Upload-Grenze für Ihren Brand Portal-Mandanten über **10** GB hinaus erweitern müssen, wenden Sie sich an den Adobe-Support und geben Sie die Anforderung an.


**Hochladen neuer Assets:**

1. Melden Sie sich bei Ihrer Brand Portal-Instanz an.
Das Brand Portal-Dashboard enthält alle vorhandenen Ordner, die dem Brand Portal-Benutzer zur Verfügung stehen, sowie den neu freigegebenen Beitragsordner.

1. Wählen Sie den Beitragsordner aus und klicken Sie darauf, um ihn zu öffnen. Der Beitragsordner enthält zwei Unterordner - **[!UICONTROL FREIGEGEBEN]** und **[!UICONTROL NEU]**.

1. Klicken Sie auf den **[!UICONTROL Ordner NEU]**.

   ![](assets/upload-new-assets4.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]** > **[!UICONTROL Dateien]**, um einzelne Dateien oder Ordner (.zip) mit mehreren Assets hochzuladen.

   ![](assets/upload-new-assets5.png)

1. Suchen Sie nach Assets (Dateien/Ordner) und laden Sie sie in den Ordner **[!UICONTROL NEU]** hoch.

   ![](assets/upload-asset4.png)

Nachdem Sie alle Assets oder Ordner in den Ordner „NEU“ hochgeladen haben, veröffentlichen Sie den Beitragsordner in Experience Manager Assets.


## Veröffentlichen des Beitragsordners in Experience Manager Assets {#publish-contribution-folder-to-aem}

Brand Portal-Benutzer können den Beitragsordner in Experience Manager Assets veröffentlichen, ohne Zugriff auf die Experience Manager Assets-Autoreninstanz zu benötigen.

Stellen Sie sicher, dass Sie die Asset-Anforderungen durchlaufen haben und die neu erstellten Assets in den Ordner **NEU** im Beitragsordner hochladen.

**So veröffentlichen Sie einen Beitragsordner:**

1. Melden Sie sich bei Ihrer Brand Portal-Instanz an.

1. Wählen Sie im Brand Portal-Dashboard einen Beitragsordner aus.
1. Klicken Sie auf **[!UICONTROL In AEM veröffentlichen]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

In verschiedenen Phasen des Veröffentlichungs-Workflows wird eine E-Mail-/Pulsbenachrichtigung an den Brand Portal-Benutzer und an Brand Portal-Administratoren gesendet:

1. **In Warteschlange** – Eine Benachrichtigung wird an den Brand Portal-Benutzer und Brand Portal-Administratoren gesendet, wenn ein Publishing-Workflow in Brand Portal ausgelöst wird.

1. **Abgeschlossen** – Eine Benachrichtigung wird an den Brand Portal-Benutzer und Brand Portal-Administratoren gesendet, wenn der Beitragsordner erfolgreich in Experience Manager Assets veröffentlicht wurde.

Nachdem die neu erstellten Assets in Experience Manager Assets veröffentlicht wurden, können Brand Portal-Benutzer sie aus dem Ordner „NEU“ löschen. Der Brand Portal-Administrator kann die Assets jedoch sowohl aus dem Ordner „NEU“ als auch aus dem Ordner „FREIGEGEBEN“ löschen.

Sobald die Erstellung eines Beitragsordners erreicht ist, kann der Brand Portal-Administrator den Beitragsordner löschen, um den Upload-Speicherplatz für andere Benutzer freizugeben.

## Status des Veröffentlichungsauftrags {#publishing-job-status}

Administratoren können zwei Berichte verwenden, um den Status von Asset-Beitragsordnern anzuzeigen, die aus Brand Portal in Experience Manager Assets veröffentlicht wurden.

* Navigieren Sie in Brand Portal zu **[!UICONTROL Tools]** > **[!UICONTROL Asset-Beitragsstatus]**. Dieser Bericht spiegelt den Status aller Veröffentlichungsaufträge in den verschiedenen Phasen des Veröffentlichungs-Workflows wider.

  ![](assets/contribution-folder-status-v2.png)

* Gehen Sie in Experience Manager Assets (On-Premise oder Managed Service) zu **[!UICONTROL Assets]** > **[!UICONTROL Aufträge]**. Dieser Bericht spiegelt den endgültigen Status (Erfolg oder Fehler) aller Veröffentlichungsaufträge wider.

  ![](assets/publishing-status.png)

* Gehen Sie in Experience Manager Assets as a Cloud Service zu **[!UICONTROL Assets]** > **[!UICONTROL Aufträge]**.

  Sie können auch direkt über die globale Navigation zu **[!UICONTROL Aufträge]** gehen.

  Dieser Bericht spiegelt den endgültigen Status (Erfolg oder Fehler) aller Veröffentlichungsaufträge wider, einschließlich des Imports von Assets aus Brand Portal in Experience Manager Assets as a Cloud Service.

  ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->

## Automatisches Löschen von in Experience Manager Assets veröffentlichten Assets aus dem Beitragsordner {#automatically-delete-published-assets-from-contribution-folder}

Brand Portal führt jetzt alle zwölf Stunden automatische Aufträge aus, um alle Beitragsordner zu überprüfen und alle Assets zu löschen, die in AEM veröffentlicht wurden. Daher müssen Sie die Assets im Beitragsordner nicht manuell löschen, um die Ordnergröße unter dem [Schwellenwert](#upload-new-assets-to-contribution-folder) zu halten. Sie können auch den Status der Löschvorgänge überwachen, die in den letzten sieben Tagen automatisch ausgeführt wurden. Der Bericht für einen Auftrag enthält die folgenden Details:

* Startzeit des Auftrags
* Endzeit des Auftrags
* Auftragsstatus
* Gesamtzahl der in einem Auftrag enthaltenen Assets
* Gesamtzahl der Assets, die erfolgreich in einem Auftrag gelöscht wurden
* Gesamtspeicher, der infolge der Auftragsausführung verfügbar gemacht wurde

  ![Löschbericht](assets/deletion-reports.png)

Sie können die Details der einzelnen Assets, die in einem Löschauftrag enthalten sind, auch weiter aufschlüsseln. Details wie der Asset-Titel, die Größe, der Autor, der Löschstatus und die Löschzeit sind im Bericht enthalten.

![Löschbericht detailliert](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * Kunden können sich an die Adobe-Kundenunterstützung wenden, um die automatische Löschfunktion zu deaktivieren und wieder zu aktivieren oder die Häufigkeit der Ausführung zu ändern.
> * Diese Funktion ist in Experience Manager 6.5.13.0 und höheren Versionen verfügbar.

### Anzeigen und Herunterladen von Löschberichten {#view-delete-jobs}

So zeigen Sie Berichte für einen Löschauftrag an und laden diese herunter:

1. Navigieren Sie in Brand Portal zur Option **[!UICONTROL Tools]** > **[!UICONTROL Asset-Beitragsstatus]** > **[!UICONTROL Löschberichte]**.

1. Wählen Sie einen Auftrag aus und klicken Sie auf **[!UICONTROL Anzeigen]**, um den Bericht anzuzeigen.

   Sehen Sie sich die Details der einzelnen Assets an, die in einem Löschauftrag enthalten sind. Details wie der Asset-Titel, die Größe, der Autor, der Löschstatus und die Löschzeit sind im Bericht enthalten. Klicken Sie auf **[!UICONTROL Herunterladen]**, um den Bericht für den Auftrag im CSV-Format herunterzuladen.

   Der Löschstatus für ein Asset kann im Bericht die folgenden möglichen Werte aufweisen:

   * **Gelöscht**: Das Asset wurde erfolgreich aus dem Beitragsordner gelöscht.

   * **Nicht gefunden**: Brand Portal konnte das Asset nicht im Beitragsordner finden. Das Asset wurde bereits manuell aus dem Ordner gelöscht.

   * **Übersprungen**: Brand Portal hat den Asset-Löschvorgang übersprungen, da eine neue Version für das Asset im Beitragsordner verfügbar ist, die noch nicht in Experience Manager veröffentlicht wurde.

   * **Fehlgeschlagen**: Brand Portal konnte das Asset nicht löschen. Es gibt drei Wiederholungsversuche, um ein Asset mit einem Löschstatus `Failed` zu löschen. Wenn der dritte Versuch, das Asset zu löschen, fehlschlägt, müssen Sie das Asset manuell löschen.

### Löschen eines Berichts

In Brand Portal können Sie auch einen oder mehrere Berichte auswählen und manuell löschen.

So löschen Sie einen Bericht:

1. Navigieren Sie zur Option **[!UICONTROL Tools]** > **[!UICONTROL Asset-Beitragsstatus]** > **[!UICONTROL Löschberichte]**.

1. Wählen Sie einen oder mehrere Berichte aus und klicken Sie auf **[!UICONTROL Löschen]**.


