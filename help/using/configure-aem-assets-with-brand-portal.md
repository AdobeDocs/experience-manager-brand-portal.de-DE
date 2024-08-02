---
title: Konfigurieren von Experience Manager Assets mit Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von Experience Manager Assets mit Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 60%

---

# Konfigurieren von Experience Manager Assets mit Brand Portal {#configure-integration}

Die Konfiguration von Adobe Experience Manager Assets mit Brand Portal bietet Benutzern von Brand Portal Funktionen zur Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets. Damit können Experience Manager Assets-Benutzer Assets veröffentlichen und an die Brand Portal-Benutzer verteilen. Brand Portal-Benutzer können auf die freigegebenen Assets zugreifen und ihren Beitrag leisten, indem sie neue Assets in die Asset-Beitragsordner hochladen und sie wieder in Experience Manager Assets veröffentlichen.

Die Konfiguration von Experience Manager Assetss mit Brand Portal wird unterstützt in:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (On-Premise und Managed Service) 6.5 und höher

Experience Manager Assets as a Cloud Service wird automatisch mit Brand Portal konfiguriert, indem Brand Portal über Cloud Manager aktiviert wird. Der Aktivierungs-Workflow erstellt die erforderlichen Konfigurationen im Backend und aktiviert Brand Portal in derselben IMS-Org wie die Experience Manager Assets as a Cloud Service-Instanz.

Im Gegensatz dazu wird Experience Manager Assets (On-Premise und verwalteter Dienst) mithilfe von Adobe Developer Console manuell mit Brand Portal konfiguriert. Dadurch wird ein Adobe Identity Management Services (IMS)-Token zur Autorisierung des Brand Portal-Mandanten abgerufen.

>[!NOTE]
>
>***Für Experience Manager Assets, 6.5 und höher***
>
>Zuvor konfigurierte die klassische Benutzeroberfläche Brand Portal mit dem Legacy OAuth Gateway, das den JSON Web Token (JWT)-Austausch nutzt, um ein IMS-Token zur Autorisierung zu erhalten.
>
>Die Konfiguration über die alte OAuth-Version wird ab dem 6. April 2020 nicht mehr unterstützt und wird durch Adobe Developer Console in die Konfiguration geändert.


>[!TIP]
>
>***Nur für Bestandskunden (On-Premise und Managed Service)***
>
>Die alte OAuth Gateway-Konfiguration funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.

Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und abhängig davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal aktivieren](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal) | - |
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal) | [Upgrade der Konfiguration](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) |
