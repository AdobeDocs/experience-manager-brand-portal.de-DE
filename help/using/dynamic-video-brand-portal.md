---
title: Unterstützung für Dynamic Video in Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Unterstützung für Dynamic Video in Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: beabaa4e5cca4c2554111861b15902cac54ccd4c
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 100%

---

# Unterstützung für Dynamic Video in Brand Portal {#dynamic-video-support-on-brand-portal}

Profitieren Sie von einer Vorschau und adaptiven Wiedergabe von Videos in Brand Portal mit Dynamic Media-Unterstützung. Laden Sie auch die dynamischen Ausgabedarstellungen aus dem Portal und von freigegebenen Links herunter.
Brand Portal-Benutzer haben folgende Möglichkeiten:

* Sehen Sie sich die Vorschau von Videos auf der Seite „Asset-Details“, in der Kartenansicht und auf der Vorschauseite der Link-Freigabe an.
* Videokodierungen auf der Seite „Asset-Details“ abspielen.
* Anzeigen dynamischer Ausgabedarstellungen auf der Registerkarte „Asset-Details“ der Seite „Asset-Details“
* Laden Sie Videokodierungen und Ordner mit Videos herunter.

>[!NOTE]
>
>Um mit Videos zu arbeiten und sie in Brand Portal zu veröffentlichen, stellen Sie sicher, dass die Experience Manager-Autoreninstanz entweder im Dynamic Media Hybrid-Modus oder im Dynamic Media **[!DNL Scene7]**-Modus.

Um Videos in einer Vorschau anzeigen, diese wiederzugeben und herunterzuladen, stellt Brand Portal die beiden folgenden Konfigurationen für Administratoren bereit:

* [Dynamic Media Hybrid-Konfiguration](#configure-dm-hybrid-settings)
Wenn die Experience Manager-Autoreninstanz im Dynamic Media Hybrid-Modus ausgeführt wird.
* [Dynamic Media  [!DNL Scene7] -Konfiguration](#configure-dm-scene7-settings)
Wenn die Experience Manager-Autoreninstanz im Dynamic Media **[!DNL Scene7]**-Modus ausgeführt wird.
Legen Sie eine dieser Konfigurationen basierend auf den Konfigurationen fest, die Sie in Ihrer Experience Manager-Autoreninstanz festgelegt haben, mit der der Brand Portal-Mandant repliziert wird.

>[!NOTE]
>
>Dynamische Videos werden nicht für Brand Portal-Mandanten unterstützt, die in der Experience Manager-Autoreninstanz mit dem **[!UICONTROL Scene7Connect]**-Ausführungsmodus konfiguriert sind.

## Wie wird Dynamic Video abgespielt? {#how-are-dynamic-videos-played}

![Videokodierungen werden aus der Cloud abgerufen.](assets/VideoEncodes.png)

Wenn Dynamic Media-Konfigurationen ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)- oder [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)-Konfigurationen) in Brand Portal eingerichtet werden, werden die dynamischen Ausgabedarstellungen vom **[!DNL Scene7]**-Server abgerufen. Videokodierungen werden daher in einer Vorschau angezeigt und ohne Verzögerung und Qualitätsverluste wiedergegeben.

Da Videokodierungen nicht im Brand Portal-Repository gespeichert und vom **[!DNL Scene7]**-Server abgerufen werden, müssen Sie sicherstellen, dass die Dynamic Media-Konfigurationen in der Adobe Experience Manager-Autoreninstanz und in Brand Portal identisch sind.

>[!NOTE]
>
>Video-Viewer und Viewer-Vorgaben werden in Brand Portal nicht unterstützt. Videos werden in den Standard-Viewern in Brand Portal als Vorschau angezeigt und abgespielt.

## Voraussetzungen {#prerequisites}

Um mit Dynamic Video in Brand Portal zu arbeiten, müssen Sie Folgendes sicherstellen:

* **Starten Sie die Experience Manager-Autoreninstanz im Dynamic Media-Modus**
Starten Sie die Experience Manager-Autoreninstanz (mit der Brand Portal konfiguriert wird) entweder im Modus [Dynamic Media - [!DNL Scene7] ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=de#enabling-dynamic-media-in-scene-mode) oder im Modus [Dynamic Media - Hybrid](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=de) oder
* **Konfigurieren Sie Dynamic Media Cloud Services in der Experience Manager-Autoreninstanz**
Abhängig vom Dynamic Media-Modus (Scene7-Modus oder Hybrid-Modus), auf dem die Experience Manager-Autoreninstanz ausgeführt wird, legen Sie entweder [Dynamic Media Cloud Services ([!DNL Scene7]-Modus)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=de#configuring-dynamic-media-cloud-services) oder [Dynamic Media Cloud Services (Hybrid-Modus)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=de#configuring-dynamic-media-cloud-services) für die Experience Manager-Autoreninstanz unter **Tools**   **Cloud Services**   **Dynamic Media** fest.
* **Konfigurieren Sie Dynamic Media in Brand Portal**
Konfigurieren Sie basierend auf den Dynamic Media-Cloud-Konfigurationen in der Experience Manager-Autoreninstanz die [Dynamic Media-Einstellungen](#configure-dm-hybrid-settings) oder die [[!DNL Scene7] -Einstellungen](#configure-dm-scene7-settings) über die Admin Tools von Brand Portal.
Stellen Sie sicher, dass [separate Brand Portal-Mandanten](#separate-tenants) für Experience Manager-Autoreninstanzen verwendet werden, die in Dynamic Media konfiguriert sind - **[!UICONTROL Scene7]**-Modus und Dynamic Media-Hybrid-Modus. Insbesondere bei der Verwendung der Dynamic Media-Funktionen **[!UICONTROL S7]** und „Dynamic Media Hybrid“.
* **Veröffentlichen Sie Ordner mit Videokodierungen, die in Brand Portal angewendet werden**
Wenden Sie [Videokodierungen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html?lang=de) an und veröffentlichen Sie den Ordner mit Rich-Media-Assets der Experience Manager-Autoreninstanz in Brand Portal.
* **Setzen Sie Egress-IPs in SPS auf die Allowlist, wenn die sichere Vorschau aktiviert ist**
Bei der Nutzung von Dynamic Media-**[!DNL Scene7]** (mit [aktivierter sicherer Vorschau](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de) für ein Unternehmen) wird empfohlen, dass der **[!DNL Scene7]** -Unternehmens-Administrator [die öffentlichen Egress-IPs auf die Zulassungsliste setzt](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de#testing-the-secure-testing-service). Dies erfolgt für die betreffenden Regionen mittels der SPS (**[!UICONTROL Scene7]** Publishing System)-Flash-Benutzeroberfläche.
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| nicht vorhanden | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

Informationen zum Hinzufügen einer dieser Egress-IPs zur Zulassungsliste finden Sie unter [Vorbereiten Ihres Kontos für sicheres Testen](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de#testing-the-secure-testing-service).

## Best Practices

Um sicherzustellen, dass Ihre Dynamic Video-Assets erfolgreich in einer Vorschau angezeigt, wiedergegeben und aus Brand Portal (und den freigegebenen Links) heruntergeladen werden, gehen Sie wie folgt vor:

### Separate Mandanten für den Modus „Dynamic Media - Scene7“ und den Modus „Dynamic Media - Hybrid“ {#separate-tenants}

Wenn Sie sowohl Funktionen des Modus „Dynamic Media – **[!DNL Scene7]**“ als auch des Modus „Dynamic Media – Hybrid“ verwenden, nutzen Sie verschiedene Brand Portal-Mandanten für Experience Manager-Autoreninstanzen, die mit dem Modus „Dynamic Media – **[!DNL Scene7]**“ und dem Modus „Dynamic Media – Hybrid“ konfiguriert wurden.


![Autoreninstanz und BP – 1:1-Zuordnung](assets/BPDynamicMedia.png)

### Gleiche Konfigurationsdetails in der Experience Manager-Autoreninstanz und in Brand Portal

Stellen Sie sicher, dass die Konfigurationsdetails in Brand Portal und der **[!UICONTROL Experience Manager Cloud-Konfiguration]** identisch sind. Dieselben Konfigurationsdetails umfassen Folgendes:

* **[!UICONTROL Titel]**
* **[!UICONTROL Registrierungs-ID]**
* **[!UICONTROL Video-Service-URL]** im Modus **[!UICONTROL Dynamic Media – Hybrid]**
* **[!UICONTROL Titel]**
* Anmeldeinformationen (**[!UICONTROL E-Mail]** und Passwort)
* **[!UICONTROL Region]**
* **[!UICONTROL Firma]** im Modus „Dynamic Media – **[!DNL Scene7]**“

### Öffentliche Ausgangs-IPs für den Dynamic Media Scene7-Modus auf die Zulassungsliste setzen

Wenn Dynamic Media **[!UICONTROL Scene7]** mit aktivierter [sicherer Vorschau](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de) genutzt wird, um Video-Assets für Brand Portal bereitzustellen, richtet **[!UICONTROL Scene7]** einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen ein. Mit einer beliebigen Anforderung an diesen Server wird die IP-Ursprungsadresse geprüft. Wenn die eingehende Anforderung nicht in der Liste genehmigter IP-Adressen enthalten ist, wird eine Fehlerantwort zurückgegeben.
Der **[!UICONTROL Scene7]**-Unternehmensadministrator konfiguriert daher eine Liste genehmigter IP-Adressen für die **[!UICONTROL sichere Testumgebung]** seines Unternehmens. Dies erfolgt über die Flash-Benutzeroberfläche von **[!UICONTROL SPS]** (Scene7 Publishing System). Stellen Sie sicher, dass die Egress-IP für Ihre jeweilige Region (siehe unten) in diese genehmigte Liste aufgenommen wird.
Informationen zum Hinzufügen einer dieser Egress-IPs zur Zulassungsliste finden Sie unter [Vorbereiten Ihres Kontos für sicheres Testen](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de#testing-the-secure-testing-service).
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| nicht vorhanden | 130.248.160.68, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| APAC | 63.140.44.54 |

## Konfigurieren von Dynamic Media (Hybrid)-Einstellungen {#configure-dm-hybrid-settings}

Wenn die Experience Manager-Autoreninstanz im Dynamic Media-Hybrid-Modus ausgeführt wird, konfigurieren Sie die Dynamic Media-Gateway-Einstellungen über die Kachel **[!UICONTROL Video]** im Bereich „Admin Tools“.

>[!NOTE]
>
>Die [Videokodierungsprofile](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html?lang=de) werden nicht in Brand Portal veröffentlicht, sondern vom **[!UICONTROL Scene7]**-Server abgerufen. Stellen Sie daher sicher, dass die Konfigurationsdetails in Ihrer Experience Manager-Autoreninstanz mit denen von [Dynamic Media Cloud Services ([!DNL Scene7]-Modus)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=de#configuring-dynamic-media-cloud-services) identisch sind, damit Videokodierungen erfolgreich in Brand Portal wiedergegeben werden können.

So richten Sie Dynamic Media-Konfigurationen für Brand Portal-Mandanten ein:

1. Wählen Sie in Brand Portal in der Symbolleiste am oberen Rand das Experience Manager-Logo aus, um die Admin Tools aufzurufen.
1. Wählen Sie im Admin-Tools-Bereich die Kachel **[!UICONTROL Video]** aus.

   ![Dynamic Media-Hybrid-Konfiguration in Brand Portal](assets/DMHybrid-Video.png)

   Die Seite **[!UICONTROL Konfiguration für Dynamic Media bearbeiten]** wird geöffnet.

   ![Dynamic Media-Hybrid-Konfiguration in Brand Portal](assets/edit-dynamic-media-config.png)

1. Geben Sie die **[!UICONTROL Registrations-ID]** und **[!UICONTROL die Video Service-URL]** (DM-Gateway URL) an. Stellen Sie sicher, dass diese Details mit denen unter **[!UICONTROL Tools > Cloud Services]** in Ihrer Experience Manager-Autoreninstanz übereinstimmen.
1. Wählen Sie **Speichern** aus, um die Konfiguration zu speichern.

## Konfigurieren von Dynamic Media Scene7-Einstellungen {#configure-dm-scene7-settings}

Wenn die Experience Manager-Autoreninstanz im Modus „Dynamic Media – **[!UICONTROL Scene7]**“ ausgeführt wird, legen Sie über die Kachel **[!UICONTROL Dynamic Media-Konfiguration]** im Bereich „Admin Tools“ die Server-Einstellungen für **[!UICONTROL Scene7]** fest.

Gehen Sie wie folgt vor, um Dynamic Media **[!UICONTROL Scene7]**-Konfigurationen für Brand Portal-Mandanten einzurichten:

1. Wählen Sie in Brand Portal in der Symbolleiste am oberen Rand das Experience Manager-Logo aus, um die Admin Tools aufzurufen.

2. Wählen Sie im Admin-Tools-Bereich die Kachel **[!UICONTROL Dynamic Media-Konfiguration]** aus.

   ![DM [!UICONTROL Scene7]-Konfiguration in Brand Portal](assets/DMS7-Tile.png)

   Die Seite **[!UICONTROL Konfiguration für Dynamic Media bearbeiten]** wird geöffnet.

   ![Scene7-Konfiguration in Brand Portal](assets/S7Config.png)

3. Geben Sie Folgendes an:

   * **[!UICONTROL Titel]**
   * Anmeldedaten (**[!UICONTROL E-Mail-ID]** und **[!UICONTROL Passwort]**) für den Zugriff auf den Scene7-Server
   * **[!UICONTROL Region]**

   Stellen Sie sicher, dass diese Werte mit den Werten in Ihrer Experience Manager-Autoreninstanz übereinstimmen.

4. Wählen Sie **[!UICONTROL Mit Dynamic Media verbinden]** aus.

5. Geben Sie den **[!UICONTROL Unternehmensnamen]** an und **[!UICONTROL speichern]** Sie die Konfiguration.
