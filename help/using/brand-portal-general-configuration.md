---
title: Verwalten allgemeiner Mandantenkonfigurationen
seo-title: Administer general tenant configurations
description: Konfigurieren Sie die Download-Beschleunigung, die Erstellung öffentlicher Smart-Sammlungen sowie die Erstellung öffentlicher Sammlungen und gestatten Sie Admin-Benutzern, Assets auf Mandanten zu löschen.
seo-description: Configure download acceleration, public smart collection creation, public collection creation, and enable admin users to delete assets on tenants.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 92%

---

# Verwalten allgemeiner Mandantenkonfigurationen {#administer-general-tenant-configurations}

Mit Experience Manager Assets Brand Portal können Unternehmen die folgenden Funktionen für bestimmte Mandanten konfigurieren:

* das Löschen von Assets durch Administratoren
* die Erstellung öffentlicher Sammlungen von Benutzern ohne Administratorrechte
* die Erstellung öffentlicher Smart-Sammlungen von Benutzern ohne Administratorrechte
* Sichtbarkeit der übergeordneten Hierarchie von freigegebenen Ordnern für Benutzer ohne Administratorrechte

Diese Konfigurationen sind über die Konfigurationen **[!UICONTROL Allgemeine Einstellungen]** im Admin Tools-Bereich möglich.

![](assets/general-config.png)

**A** Konfiguration, die es Administratoren gestattet, Assets aus Brand Portal zu löschen. (Die Option ist standardmäßig aktiviert.)

**B** Konfiguration, die es Benutzern ohne Administratorrechte gestattet, öffentliche Sammlungen zu erstellen. (Die Option ist standardmäßig aktiviert.)

**C** Konfiguration, die es Benutzern ohne Administratorrechte gestattet, öffentliche Smart-Sammlungen zu erstellen. (Die Option ist standardmäßig aktiviert.)

**D** Konfiguration, die Benutzern ohne Administratorrechte (Bearbeitern, Betrachtern und Gastbenutzern) gestattet, die Ordnerhierarchie (vom Stamm) der freigegebenen Ordner anzuzeigen. (Die Option ist standardmäßig deaktiviert.)

## Aktivieren/Deaktivieren der allgemeinen Konfigurationen {#enable-disable-general-configurations}

So aktivieren/deaktivieren Sie jede dieser Konfigurationen:

1. Melden Sie sich mit Administratorrechten an.
1. Wählen Sie in der Symbolleiste am oberen Rand das Experience Manager-Logo aus, um auf die Admin Tools zuzugreifen.
1. Wählen Sie im Admin Tools-Bereich die Option **[!UICONTROL Allgemein]** aus, um die Seite **[!UICONTROL Allgemeine Einstellungen]** zu öffnen.
1. Verwenden Sie den entsprechenden Umschalter, um allgemeine Konfigurationen zu aktivieren/deaktivieren.
1. **[!UICONTROL Speichern]** Sie die Änderungen.
1. Melden Sie sich ab, um die Änderungen zu übernehmen.

## Löschen von Assets in Brand Portal durch Administratoren zulassen {#allow-admin-users-to-delete-assets-from-brand-portal}

Mit der Konfiguration **[!UICONTROL Löschen von Assets in Brand Portal durch Administratoren zulassen]** können Unternehmen Administratoren erlauben, Assets und Ordner aus Brand Portal zu löschen.

## Zulassen der Erstellung öffentlicher Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-collections-creation-by-non-admins}

Mit der Konfiguration [[!UICONTROL Zulassen der Erstellung öffentlicher Sammlungen durch Benutzer ohne Administratorrechte]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) wird gesteuert, ob Benutzer ohne Administratorrechte öffentliche Sammlungen in Brand Portal erstellen können. Die Konfiguration ist standardmäßig aktiviert. Unternehmen können die Konfiguration deaktivieren, um zu verhindern, dass sich in ihrem Portal zahlreiche öffentliche Sammlungen befinden. Auf diese Weise wird Systemspeicherplatz eingespart.

## Zulassen der Erstellung öffentlicher Smart-Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-smart-collections-creation-by-non-admins}

Mit der Konfiguration [[!UICONTROL Zulassen der Erstellung öffentlicher Smart-Sammlungen durch Benutzer ohne Administratorrechte]](../using/brand-portal-searching.md#main-pars-header-500620467) wird gesteuert, ob Benutzer ohne Administratorrechte Suchen als Smart-Sammlungen speichern und sie für diesen Mandanten öffentlich machen können. Die Konfiguration ist standardmäßig aktiviert. Unternehmen können die Konfiguration deaktivieren, um zu verhindern, dass Benutzer ohne Administratorrechte eine große Anzahl öffentlicher Smart-Sammlungen im Brand Portal der Organisation erstellen.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Aktivieren der Ordnerhierarchie {#enable-folder-hierarchy}

Mit der Konfiguration [[!UICONTROL Ordnerhierarchie aktivieren]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) können Administratoren steuern, wie Benutzer ohne Administratorrechte (Bearbeiter, Betrachter und Gastbenutzer) die freigegebenen Ordner nach der Anmeldung sehen.
