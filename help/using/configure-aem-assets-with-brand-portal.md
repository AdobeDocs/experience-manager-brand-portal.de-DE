---
title: Konfigurieren von Experience Manager Assets mit Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von Experience Manager Assets mit Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: f4add370fd3242f5506e5cc4d921362e2b14141a
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 60%

---

# Konfigurieren von Experience Manager Assets mit Brand Portal {#configure-integration}

Die Konfiguration von Adobe Experience Manager Assets mit Brand Portal bietet Benutzern von Brand Portal Funktionen zur Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets. Dadurch können Experience Manager Assets-Benutzende Assets veröffentlichen und mit den Brand Portal-Benutzenden verteilen. Brand Portal-Benutzer können auf die freigegebenen Assets zugreifen und ihren Beitrag leisten, indem sie neue Assets in die Asset-Beitragsordner hochladen und sie wieder in Experience Manager Assets veröffentlichen.

Die Konfiguration von Experience Manager Assetss mit Brand Portal wird unterstützt in:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (On-Premise und Managed Service) 6.5 und höher

Experience Manager Assets as a Cloud Service wird automatisch mit Brand Portal konfiguriert, indem Brand Portal über Cloud Manager aktiviert wird. Der Aktivierungs-Workflow erstellt die erforderlichen Konfigurationen im Backend und aktiviert Brand Portal in derselben IMS-Org wie die Experience Manager Assets as a Cloud Service-Instanz.

Experience Manager Assets (On-Premise und Managed Service) wird hingegen manuell mit Brand Portal mithilfe von Adobe Developer Console konfiguriert, wodurch ein Adobe Identity Management Services (IMS)-Token zur Autorisierung des Brand Portal-Mandanten abgerufen wird.

>[!NOTE]
>
>***Für Experience Manager Assets 6.5 und höher***
>
>Zuvor wurde Brand Portal auf der klassischen Benutzeroberfläche mit dem alten OAuth-Gateway konfiguriert. Das Gateway ruft mithilfe des JSON Web Token (JWT)-Austauschs ein IMS-Token zur Autorisierung ab.
>
>Die Konfiguration über das alte OAuth wird ab dem 6. April 2020 nicht mehr unterstützt, sondern über Adobe Developer Console auf die Konfiguration umgestellt.


>[!TIP]
>
>***Nur für Bestandskunden (On-Premise und Managed Service)***
>
>Die Konfiguration des alten OAuth-Gateways funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth-Gateway-Konfiguration auftreten, löschen Sie die bestehende Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.

Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und abhängig davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal aktivieren](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal) | – |
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal) | [Upgrade der Konfiguration](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) |
