---
title: Verwalten des Benutzerzugriffs auf Brand Portal
description: Konfigurieren Sie den Gastzugriff und den Neubenutzerzugriff auf die Brand Portal.
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 27a9cd26-9bb3-473b-b1ac-37f77975c912
TQID: https://experienceleague.adobe.com/SGJ5f5BOFd4Yiu2OiR9wyRU3wk-YlnGrX5Zm5JmPHuY
product_v2: id: d09181b5-a36a-43de-ba01-36641440bc43id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2: id: cda65036-5305-4f01-89da-9b3506ae8c50id: da0dfbce-df02-4f8b-b32d-a4e3b1d05085
subfeature_v2: id: e00c7c12-7035-41fe-ad76-1ec82c8c3f01
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e48edcb1ed5d76686794f7a7ed6389c7f4ab1ed3
workflow-type: tm+mt
source-wordcount: 293
ht-degree: 32%

---

# Verwalten des Benutzerzugriffs auf Brand Portal {#administer-user-access-on-brand-portal}

Ab Adobe Experience Manager Assets Brand Portal 6.4.2 können Administratoren den Gastzugriff konfigurieren und es Benutzern ermöglichen, Zugriff auf die Brand Portal ihres Unternehmens anzufordern. Diese Konfigurationen sind über die Konfigurationen **[!UICONTROL Zugriffseinstellungen]** im Verwaltungsbereich möglich. Beide Einstellungen sind standardmäßig deaktiviert.

![](assets/access-configs.png)

**A** - Konfiguration, über die Gäste über den **[!UICONTROL `Guest Access?`]** auf dem Brand Portal-Willkommensbildschirm auf Brand Portal zugreifen können. (Die Option ist standardmäßig deaktiviert.)

**B** - Konfiguration, damit Benutzende über den **[!UICONTROL `Need access?`]** Link auf dem Brand Portal-Willkommensbildschirm Zugriff auf Brand Portal anfordern können. (Die Option ist standardmäßig deaktiviert.)

## Zulassen des Gastzugangs {#allow-guest-access}

Durch die Gewährung von Gastzugriff können Benutzer auf die öffentlichen Assets zugreifen, ohne sich bei Brand Portal anmelden zu müssen.
Um den Gastzugang zuzulassen, muss der Administrator die folgenden Schritte ausführen:

1. Wählen Sie oben in der Symbolleiste das AEM-Logo aus, um die Admin-Tools aufzurufen.
1. Wählen Sie im Admin-Tools-Bereich die Option **[!UICONTROL Zugriff]** aus, um die Seite **[!UICONTROL Zugriffseinstellungen]** zu öffnen.
1. Aktivieren Sie die Konfiguration **[!UICONTROL Gastzugang erlauben]**.
1. **[!UICONTROL Speichern]** Sie die Änderungen.
1. Melden Sie sich ab, damit die Änderungen wirksam werden.

![](assets/bp-welcome-screen.png)

## Erlauben der Zugriffsanfrage durch Benutzer {#allow-users-to-request-access}

Administratoren können Benutzern von Organisationen erlauben, auf dem Willkommensbildschirm den Zugriff auf Brand Portal anzufordern. Admins müssen jedoch die Konfiguration **[!UICONTROL Benutzern Zugriff erteilen]** aktivieren, damit der Link Zugriff anfordern auf dem Willkommensbildschirm angezeigt wird.

Damit Organisationsbenutzer Zugriff auf Brand Portal anfordern können, müssen Administratoren folgende Schritte durchführen:

1. Wählen Sie oben in der Symbolleiste das AEM-Logo aus, um die Admin-Tools aufzurufen.
1. Wählen Sie im Admin-Tools-Bereich die Option **[!UICONTROL Zugriff]** aus, um die Seite **[!UICONTROL Zugriffseinstellungen]** zu öffnen.
1. Aktivieren Sie die Konfiguration **[!UICONTROL Zugriffsanfrage durch Benutzer zulassen]**.
1. **[!UICONTROL Speichern]** Sie die Änderungen.
1. Melden Sie sich ab, damit die Änderungen wirksam werden.
