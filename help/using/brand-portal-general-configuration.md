---
title: Verwalten allgemeiner Mandantenkonfigurationen
description: Konfigurieren Sie die Download-Beschleunigung, die Erstellung öffentlicher Smart-Sammlungen sowie die Erstellung öffentlicher Sammlungen und gestatten Sie Admin-Benutzern, Assets auf Mandanten zu löschen.
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 53%

---

# Verwalten allgemeiner Mandantenkonfigurationen {#administer-general-tenant-configurations}

In Experience Manager Assetss Brand Portal können Unternehmen die folgenden Funktionen für bestimmte Mandanten konfigurieren:

* das Löschen von Assets durch Administratoren
* die Erstellung öffentlicher Sammlungen von Benutzern ohne Administratorrechte
* die Erstellung öffentlicher Smart-Sammlungen von Benutzern ohne Administratorrechte
* Die übergeordnete Hierarchie freigegebener Ordner ist für Benutzer ohne Administratorrechte sichtbar.

Diese Konfigurationen wurden als Konfigurationen für **[!UICONTROL Allgemeine Einstellungen]** im Admin Tools-Bereich bereitgestellt.

![](assets/general-config.png)

**A** - Konfiguration, die es Administratoren gestattet, Assets aus Brand Portal zu löschen. (Die Option ist standardmäßig aktiviert.)

**B** - Konfiguration, die es Benutzern ohne Administratorrechte gestattet, öffentliche Sammlungen zu erstellen. (Die Option ist standardmäßig aktiviert.)

**C** - Konfiguration, die es Benutzern ohne Administratorrechte gestattet, öffentliche Smart-Sammlungen zu erstellen. (Die Option ist standardmäßig aktiviert.)

**D** - Konfiguration zum Anzeigen der Ordnerhierarchie (vom Stamm) freigegebener Ordner für Benutzer ohne Administratorrechte (Bearbeiter, Betrachter, Gastbenutzer). (Die Option ist standardmäßig deaktiviert.)

## Aktivieren oder Deaktivieren der allgemeinen Konfigurationen {#enable-disable-general-configurations}

So aktivieren oder deaktivieren Sie jede dieser Konfigurationen:

1. Melden Sie sich mit Administratorrechten an.
1. Wählen Sie das Experience Manager-Logo aus, um in der Symbolleiste am oberen Rand auf die Admin Tools zuzugreifen.
1. Wählen Sie im Admin-Tools-Bereich die Option **[!UICONTROL Allgemein]** aus, um die Seite **[!UICONTROL Allgemeine Einstellungen]** zu öffnen.
1. Verwenden Sie den entsprechenden Umschalter, um eine der allgemeinen Konfigurationen zu aktivieren oder zu deaktivieren.
1. **[!UICONTROL Speichern]** Sie die Änderungen.
1. Melden Sie sich ab, damit die Änderungen wirksam werden können.

## Löschen von Assets in Brand Portal durch Administratoren zulassen {#allow-admin-users-to-delete-assets-from-brand-portal}

Mit der Konfiguration **[!UICONTROL Löschen von Assets in Brand Portal durch Administratoren zulassen]** können Unternehmen Administratoren erlauben, Assets und Ordner aus Brand Portal zu löschen.

## Zulassen der Erstellung öffentlicher Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-collections-creation-by-non-admins}

Mit der Konfiguration [[!UICONTROL Zulassen der Erstellung öffentlicher Sammlungen durch Benutzer ohne Administratorrechte]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) wird gesteuert, ob Benutzer ohne Administratorrechte öffentliche Sammlungen in Brand Portal erstellen können. Die Konfiguration ist standardmäßig aktiviert. Unternehmen können die Konfiguration deaktivieren, um zu verhindern, dass sich in ihrem Portal zahlreiche öffentliche Sammlungen befinden, sodass Systemspeicherplatz eingespart werden kann.

## Zulassen der Erstellung öffentlicher Smart-Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-smart-collections-creation-by-non-admins}

Mit der Konfiguration [[!UICONTROL Zulassen der Erstellung öffentlicher Smart-Sammlungen durch Benutzer ohne Administratorrechte]](../using/brand-portal-searching.md#main-pars-header-500620467) wird gesteuert, ob Benutzer ohne Administratorrechte Suchen als Smart-Sammlungen speichern und sie für diesen Mandanten öffentlich machen können. Die Konfiguration ist standardmäßig aktiviert. Unternehmen können die Konfiguration deaktivieren, um zu verhindern, dass Benutzer ohne Administratorrechte eine große Anzahl öffentlicher Smart-Sammlungen im Brand Portal des Unternehmens erstellen.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Aktivieren der Ordnerhierarchie {#enable-folder-hierarchy}

Mit der Konfiguration [[!UICONTROL Ordnerhierarchie aktivieren]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) können Administratoren steuern, wie Benutzer ohne Administratorrechte (Bearbeiter, Betrachter und Gastbenutzer) die freigegebenen Ordner nach der Anmeldung sehen.
