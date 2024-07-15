---
title: Konfigurieren von Experience Manager Assets mit Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von Experience Manager Assets mit Brand Portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 454b05c05359a2068cc29124f826d5bd25a1bad1
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 100%

---

# Konfigurieren von Experience Manager Assets mit Brand Portal {#configure-integration}

Die Konfiguration von Adobe Experience Manager Assets mit Brand Portal bietet Benutzern von Brand Portal Funktionen zur Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets. Sie ermöglicht Experience Manager Assets-Benutzern das Veröffentlichen und Verteilen von Assets an Brand Portal-Benutzer. Brand Portal-Benutzer können auf die freigegebenen Assets zugreifen und ihren Beitrag leisten, indem sie neue Assets in die Asset-Beitragsordner hochladen und sie wieder in Experience Manager Assets veröffentlichen.

Die Konfiguration von Experience Manager Assetss mit Brand Portal wird unterstützt in:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (On-Premise und Managed Service) 6.5 und höher

Experience Manager Assets as a Cloud Service wird automatisch mit Brand Portal konfiguriert, indem Brand Portal über Cloud Manager aktiviert wird. Der Aktivierungs-Workflow erstellt die erforderlichen Konfigurationen im Backend und aktiviert Brand Portal in derselben IMS-Org wie die Experience Manager Assets as a Cloud Service-Instanz.

Experience Manager Assets (On-Premise und Managed Service) wird hingegen manuell mit Brand Portal über Adobe Developer Console konfiguriert, die ein Adobe Identity Management Services (IMS)-Token für die Autorisierung des Brand Portal-Mandanten abruft.

>[!NOTE]
>
>***Für Experience Manager Assets 6.5 und höher***
>
>Zuvor wurde Brand Portal über das alte OAuth-Gateway in der klassischen Benutzeroberfläche konfiguriert. Das Gateway ruft mithilfe des JSON Web Token (JWT)-Austauschs ein IMS-Token zur Autorisierung ab.
>
>Die Konfiguration über das alte OAuth-Protokoll wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe Developer Console.


>[!TIP]
>
>***Nur für Bestandskunden (On-Premise und Managed Service)***
>
>Die alte OAuth Gateway-Konfiguration funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth-Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.

Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und abhängig davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal aktivieren](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html?lang=de) | - |
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=de) | [Upgrade der Konfiguration](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=de#upgrade-integration-65) |
