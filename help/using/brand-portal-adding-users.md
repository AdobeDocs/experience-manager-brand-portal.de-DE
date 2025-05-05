---
title: Verwalten von Benutzern, Gruppen und Benutzerrollen
description: Erfahren Sie, wie Administratoren die Adobe Admin Console verwenden können, um Brand Portal-Benutzende und -Produktprofile zu erstellen und ihre Rollen mithilfe der Benutzeroberfläche von Brand Portal zu verwalten. Diese Berechtigung ist für Betrachter und Bearbeiter nicht verfügbar.
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 35b1fd75-f9e4-4145-80bd-84de091f8b2b
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '2166'
ht-degree: 57%

---

# Verwalten von Benutzern, Gruppen und Benutzerrollen {#manage-users-groups-and-user-roles}

Administratoren können Adobe Admin Console verwenden, um Benutzende und Produktprofile für Experience Manager Assets Brand Portal zu erstellen und ihre Rollen mithilfe der Benutzeroberfläche von Brand Portal zu verwalten. Diese Berechtigung ist für Betrachter und Bearbeiter nicht verfügbar.

In der [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) können Sie alle Produkte anzeigen, die mit Ihrem Unternehmen verbunden sind. Bei diesen Produkten kann es sich um beliebige Experience Cloud-Lösungen handeln, z. B. Adobe Analytics, Adobe Target oder Experience Manager Assets Brand Portal. Wählen Sie das AEM Brand Portal-Produkt aus und erstellen Sie Produktprofile.

<!--
Comment Type: draft

<note type="note">
<p>Product profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to Product Profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Diese Produktprofile werden alle 8 Stunden mit der Benutzeroberfläche von Brand Portal synchronisiert und in Brand Portal als Gruppen angezeigt. Nachdem Sie Benutzende hinzugefügt, Produktprofile erstellt und diesen Produktprofilen Benutzende hinzugefügt haben, können Sie in Brand Portal Benutzenden und Gruppen Rollen zuweisen.

>[!NOTE]
>
>Um in Brand Portal Gruppen zu erstellen, wählen Sie in der [!UICONTROL Adobe Admin Console] die Seite **[!UICONTROL Produkte > Produktprofile]** (nicht **[!UICONTROL Benutzer > Benutzergruppen]**) aus. Die Funktion „Produktprofile“ in der [!UICONTROL Adobe Admin Console] wird zum Erstellen von Gruppen in Brand Portal verwendet.

## Hinzufügen von Benutzern {#add-a-user}

Verwenden Sie als Produkt-Administrator die Adobe [[!UICONTROL Admin Console &#x200B;]](https://adminconsole.adobe.com/enterprise/overview), um Benutzende zu erstellen und diese Produktprofilen (*ehemals „Produktkonfigurationen„) zuzuweisen,* in Brand Portal als Gruppen angezeigt werden. Sie können über Gruppen Massenvorgänge wie Rollenverwaltung und Asset-Freigabe durchführen.

>[!NOTE]
>
>Neue Benutzende, die keinen Zugriff auf Brand Portal haben, können den Zugriff über den Anmeldebildschirm von Brand Portal anfordern. Weitere Informationen finden Sie unter [Zugriff auf Brand Portal anfordern](../using/brand-portal.md#request-access-to-brand-portal). Wenn Sie im Benachrichtigungsbereich eine Benachrichtigung über eine Zugriffsanforderung erhalten, klicken Sie auf die entsprechende Benachrichtigung und dann auf **[!UICONTROL Zugriff erlauben]**. Alternativ können Sie auch auf den Link in der eingegangenen E-Mail mit der Zugriffsanforderung klicken. Anschließend wird der Benutzer über die [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) hinzugefügt. Befolgen Sie dazu die unten beschriebenen Schritte 4 bis 7.

>[!NOTE]
>
>Sie können sich direkt oder von Brand Portal aus bei der [Adobe](https://adminconsole.adobe.com/enterprise/overview)Admin Console  anmelden. Wenn Sie sich direkt anmelden, befolgen Sie die unten stehenden Schritte 4 bis 7, um einen Benutzer hinzuzufügen.

1. Klicken Sie oben in der AEM-Symbolleiste auf das Adobe-Logo, um auf die Admin-Tools zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin-Tools-Bereich](assets/admin-tools-panel-5.png)

1. Klicken Sie auf der Seite [!UICONTROL Benutzerrollen] auf die Registerkarte **[!UICONTROL Verwaltung]** und klicken Sie dann auf **[!UICONTROL Admin Console starten]**.

   ![Benutzerrollen zum Starten der Admin Console](assets/launch_admin_console.png)

1. Führen Sie in der Admin Console einen der folgenden Schritte aus, um einen neuen Benutzer zu erstellen:

   * Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Überblick]**. Klicken Sie auf der Seite [!UICONTROL Überblick] auf der Produktkarte „Brand Portal“ auf **[!UICONTROL Benutzer zuweisen]**.

   ![Überblick über die Admin Console](assets/admin_console_overviewadduser.png)

   * Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Benutzer]**. Auf der [!UICONTROL Benutzer]-Seite [!UICONTROL Benutzer] in der linken Leiste standardmäßig ausgewählt. Klicken Sie auf **[!UICONTROL Benutzer hinzufügen]**.

   ![Admin Console – Benutzer hinzufügen](assets/admin_console_adduseruserpage.png)

1. Geben Sie im Dialogfeld Benutzer hinzufügen die E-Mail-ID des Benutzers ein, den Sie hinzufügen möchten, oder wählen Sie den Benutzer aus der Liste der Vorschläge aus, die beim Tippen angezeigt werden.

   ![Benutzer zu Brand Portal hinzufügen](assets/add_user_to_aem_bp.png)

1. Weisen Sie den Benutzer mindestens einem Produktprofil (ehemals „Produktkonfiguration“) zu, damit der Benutzer auf Brand Portal zugreifen kann. Wählen Sie im Feld **[!UICONTROL Profil für dieses Produkt auswählen]** das entsprechende Produktprofil aus.
1. Klicken Sie auf **[!UICONTROL Speichern]**. Eine Begrüßungs-E-Mail wird an den neu hinzugefügten Benutzer gesendet. Der eingeladene Benutzer kann auf den Link in der Begrüßungs-E-Mail klicken, um auf Brand Portal zuzugreifen. Die Benutzerin bzw. der Benutzer kann sich mit der in der Admin Console konfigurierten E-MailID ([!UICONTROL Adobe ID], Enterprise ID oder [!UICONTROL Federated ID]) anmelden. Weitere Informationen finden Sie unter [Schritte bei der ersten Anmeldung](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >Wenn sich ein(e) Benutzende(r) nicht bei Brand Portal anmelden kann, sollte der Administrator des Unternehmens die Adobe-[!UICONTROL Admin Console aufrufen]. Überprüfen Sie, ob der Benutzer vorhanden ist und zu mindestens einem Produktprofil hinzugefügt wurde.

   Informationen zum Gewähren von Administratorrechten für Benutzer finden Sie unter [Bereitstellen von Administratorrechten für Benutzer](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Hinzufügen von Produktprofilen {#add-a-product-profile}

Produktprofile (ehemals „Produktkonfigurationen“) in der [!UICONTROL Admin Console] werden zum Erstellen von Gruppen in Brand Portal verwendet, mit deren Hilfe Sie Massenvorgänge wie Rollenverwaltung und Asset-Freigabe durchführen können. **Brand Portal** ist das standardmäßig verfügbare Produktprofil. Sie können weitere Produktprofile erstellen und Benutzer zu den neuen Produktprofilen hinzufügen.

>[!NOTE]
>
>Sie können sich direkt oder über Brand Portal bei [&#128279;](https://adminconsole.adobe.com/enterprise/overview) [!UICONTROL Admin Console anmelden. Wenn Sie sich direkt bei der Admin Console {]} anmelden, befolgen Sie die unten beschriebenen Schritte 4 bis 7, um ein Produktprofil hinzuzufügen.

1. Klicken Sie oben in der AEM-Symbolleiste auf das Adobe-Logo, um auf die Admin-Tools zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin-Tools-Bereich](assets/admin-tools-panel-6.png)

1. Klicken Sie auf der Seite [!UICONTROL Benutzerrollen] auf die Registerkarte **[!UICONTROL Verwaltung]** und klicken Sie dann auf **[!UICONTROL Admin Console starten]**.

   ![Admin Console starten](assets/launch_admin_console.png)

1. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Produkte]**.
1. Auf der [!UICONTROL Produkte]Seite [!UICONTROL Produktprofile] standardmäßig ausgewählt. Klicken Sie auf **[!UICONTROL Neues Profil]**.

   ![Neues Produktprofil hinzufügen](assets/admin_console_addproductprofile.png)

1. Geben [!UICONTROL &#x200B; auf der Seite &#x200B;]Neues Profil erstellen“ den Profilnamen, den Anzeigenamen und die Profilbeschreibung an. Entscheiden Sie sich dafür, Benutzer per E-Mail benachrichtigen zu lassen, wenn sie zum Profil hinzugefügt oder daraus entfernt werden.

   ![Produktprofil erstellen](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Klicken Sie auf **[!UICONTROL Fertig]**. Die Produktkonfigurationsgruppe. Beispielsweise wird die **[!UICONTROL Vertriebsgruppe]** zu Brand Portal hinzugefügt.

   ![Produktprofile](assets/admin_console_productprofileadded.png)

## Hinzufügen von Benutzern zu Produktprofilen {#add-users-to-a-product-profile}

Um Benutzer zu einer Brand Portal-Gruppe hinzuzufügen, fügen Sie sie dem entsprechenden Produktprofil (ehemals „Produktkonfigurationen„) in der [!UICONTROL Admin Console hinzu]. Sie können Benutzer einzeln oder mehrere Benutzer auf einmal hinzufügen.

>[!NOTE]
>
>Sie können sich direkt oder über Brand Portal bei [&#128279;](https://adminconsole.adobe.com/enterprise/overview) Admin Console anmelden. Wenn Sie sich direkt bei der Admin Console anmelden, befolgen Sie die unten beschriebenen Schritte 4 bis 7, um Benutzer zu einem Produktprofil hinzuzufügen.

1. Klicken Sie in der Symbolleiste oben auf das Experience Manager-Logo, um auf die Admin-Tools zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin-Tools-Bereich](assets/admin-tools-panel-7.png)

1. Klicken Sie auf der Seite [!UICONTROL Benutzerrollen] auf die Registerkarte **[!UICONTROL Verwaltung]** und klicken Sie dann auf **[!UICONTROL Admin Console starten]**.

   ![Starten [!DNL Admin Console]](assets/launch_admin_console.png)

1. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Produkte]**.
1. Auf der [!UICONTROL Produkte]Seite [!UICONTROL Produktprofile] standardmäßig ausgewählt. Öffnen Sie das Produktprofil, zu dem ein Benutzer hinzugefügt werden soll, zum Beispiel [!UICONTROL Vertriebsgruppe].

   ![Produktprofile](assets/admin_console_productprofileadded.png)

1. Gehen Sie wie folgt vor, um einzelne Benutzer zum Produktprofil hinzuzufügen:

   * Klicken Sie auf **[!UICONTROL Benutzer hinzufügen]**.

   ![Gruppe zum Zuordnen des Produktprofils in Brand Portal](assets/admin_console_productprofilesalesgroup.png)

   * Geben Sie auf der Seite [!UICONTROL Benutzer zu Vertriebsgruppe hinzufügen] die E-Mail-Adresse des Benutzers ein, den Sie hinzufügen möchten, oder wählen Sie den Benutzer aus der Liste mit Vorschlägen aus, die eingeblendet wird, wenn Sie mit der Eingabe beginnen.

   ![Hinzufügen eines Benutzers zu einer Gruppe](assets/admin_console_addusertosalesgroup.png)

   * Klicken Sie auf **[!UICONTROL Speichern]**.

1. Gehen Sie wie folgt vor, um mehrere Benutzer zum Produktprofil hinzuzufügen:

   * Wählen Sie **[!UICONTROL die Auslassungszeichen (...) > Benutzer über CSV hinzufügen]** aus.

   ![Stapelweises Hinzufügen von Benutzern](assets/admin_console_addbulkusers.png)

   * Laden Sie auf der Seite **[!UICONTROL Benutzer über CSV hinzufügen]** eine CSV-Vorlage herunter oder fügen Sie eine CSV-Datei per Drag-and-Drop hinzu.

   ![Benutzer über CSV hinzufügen](assets/admin_console_addbulkuserscsv.png)

   * Klicken Sie auf **[!UICONTROL Hochladen]**.

   Wenn Sie Benutzende zum Standardproduktprofil Brand Portal hinzufügen, sendet das System eine Begrüßungs-E-Mail an die entsprechenden E-Mail-IDs. Die eingeladenen Benutzer können dann auf Brand Portal zugreifen, indem sie auf den Link in der Begrüßungs-E-Mail klicken und sich mit ihrer [!UICONTROL Adobe ID anmelden]. Siehe [Erstes Anmeldeerlebnis](../using/brand-portal-onboarding.md).

   Benutzende, die einem benutzerdefinierten oder einem neuen Produktprofil hinzugefügt wurden, erhalten keine E-Mail-Benachrichtigungen.

## Bereitstellen von Administratorrechten für Benutzer {#provide-administrator-privileges-to-users}

Sie können einem Brand Portal-Benutzer entweder Systemadministrator- oder Produktadministratorrechte gewähren. Vermeiden Sie es jedoch, andere in der Admin Console [!UICONTROL &#x200B; verfügbare Administratorrollen zuzuweisen]. Zum Beispiel Produktprofil-Administrator, Benutzergruppen-Administrator und Support-Administrator. Siehe [Administratorrollen](https://helpx.adobe.com/de/enterprise/using/admin-roles.html).

>[!NOTE]
>
>Sie können sich direkt oder über Brand Portal bei [&#128279;](https://adminconsole.adobe.com/enterprise/overview) Admin Console anmelden. Wenn Sie sich direkt bei der [!UICONTROL Admin Console &#x200B;], befolgen Sie die unten beschriebenen Schritte 4 bis 8, um einen Benutzer zu einem Produktprofil hinzuzufügen.

1. Klicken Sie oben in der AEM-Symbolleiste auf das Adobe-Logo, um auf die Admin-Tools zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin-Tools-Bereich](assets/admin-tools-panel-8.png)

1. Klicken Sie auf der Seite [!UICONTROL Benutzerrollen] auf die Registerkarte **[!UICONTROL Verwaltung]** und klicken Sie dann auf **[!UICONTROL Admin Console starten]**.

   ![Admin Console starten](assets/launch_admin_console.png)

1. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Benutzer]**.
1. Auf der Seite [!UICONTROL Benutzer] in der linken Leiste [!UICONTROL Benutzer] standardmäßig ausgewählt. Klicken Sie auf den Benutzernamen des Benutzers, dem Sie Administratorrechte gewähren möchten.

   ![Benutzer in der Admin Console hinzufügen](assets/admin_console_adduseruserpage.png)

1. Klicken Sie auf der Benutzerprofilseite unten im Bereich **[!UICONTROL Administratorrechte]** auf **[!UICONTROL die Auslassungszeichen (...) > Administratorrechte bearbeiten]**.
   ![Administratorrechte in der Admin Console](assets/admin_console_editadminrights.png)

1. Wählen Sie auf der Seite [!UICONTROL Administratorrechte bearbeiten] die Option „Systemadministrator“ bzw. „Produkt-Administrator“ aus.

   ![Administratorrechte in der Admin Console bearbeiten](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal unterstützt nur die Rollen „Systemadministrator“ und „Produkt-Administrator“.
   >
   >Adobe empfiehlt, die Rolle „Systemadministrator“ zu vermeiden, da sie für alle Produkte des jeweiligen Unternehmens unternehmensweite Administratorrechte gewährt. Beispielsweise verfügt ein Systemadministrator einer Organisation, die drei Cloud-Produkte für das Marketing enthält, über den gesamten Satz von Berechtigungen für alle drei Produkte. Nur ein Systemadministrator kann Experience Manager Assets so konfigurieren, dass Assets aus Experience Manager Assets in Brand Portal veröffentlicht werden können. Weitere Informationen finden Sie unter [Konfigurieren von Experience Manager Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >Im Gegensatz dazu gewährt die Rolle „Produkt-Administrator“ ausschließlich Administratorrechte für ein bestimmtes Produkt. Wenn Sie detaillierte Zugriffssteuerungen innerhalb von Brand Portal umsetzen möchten, verwenden Sie die Rolle „Produkt-Administrator“ und wählen Sie als Produkt Brand Portal aus.

   >[!NOTE]
   >
   >Brand Portal unterstützt keine Produktprofil-Administratorrechte (ehemals „Konfigurationsadministrator„). Vermeiden Sie es, Benutzern die Administratorrolle „Produktprofil-Administrator“ zuzuweisen.

1. Überprüfen Sie die Auswahl des Administratortyps und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!NOTE]
   >
   >Um die Administratorrechte für einen Benutzer zu widerrufen, nehmen Sie auf der Seite **[!UICONTROL Administrator bearbeiten]** die entsprechenden Änderungen vor und klicken Sie auf **[!UICONTROL Speichern]**.


## Verwalten von Benutzerrollen {#manage-user-roles}

Ein Administrator kann die Rollen von Benutzenden in Brand Portal ändern.

Zusätzlich zur Administratorrolle unterstützt Brand Portal die folgenden Rollen:

* [!UICONTROL Betrachter:] Benutzer mit dieser Rolle können Dateien und Ordner anzeigen, die ein Administrator für sie freigegeben hat. Betrachter können zudem nach Assets suchen und diese herunterladen. Sie können jedoch keine Inhalte (Dateien, Ordner, [!UICONTROL Sammlungen]) für andere Benutzer freigeben.
* [!UICONTROL Editor]: Benutzer mit dieser Rolle haben alle Berechtigungen eines Viewers. Zusätzlich können Bearbeiter Inhalte (Ordner, [!UICONTROL Sammlungen], Links) für andere Benutzer freigeben.

1. Klicken Sie oben in der AEM-Symbolleiste auf das Adobe-Logo, um auf die Admin-Tools zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

1. Klicken Sie im Admin-Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin-Tools-Bereich](assets/admin-tools-panel-9.png)

1. Auf der Seite [!UICONTROL Benutzerrollen] ist die Registerkarte [!UICONTROL Benutzer] standardmäßig ausgewählt. Für den Benutzer, dessen Rolle Sie ändern möchten, wählen Sie **[!UICONTROL Bearbeiter]** oder **[!UICONTROL Betrachter]** aus der Dropdown-Liste **[!UICONTROL Rolle]**.

   ![Benutzerrollen ändern](assets/modify_user_role.png)

   Wenn Sie gleichzeitig die Rollen mehrerer Benutzer ändern möchten, wählen Sie die entsprechenden Benutzer aus und wählen Sie die gewünschte Rolle in der Dropdown-Liste **[!UICONTROL Rolle]** aus.

   >[!NOTE]
   >
   >Die [!UICONTROL Rollen]-Liste für Admin-Benutzer ist deaktiviert. Sie können diese Benutzer nicht auswählen, um ihre Rollen zu ändern.


   >[!NOTE]
   >
   >Die Benutzerrolle ist auch deaktiviert, wenn der Benutzer Mitglied der Gruppe „Editor“ ist. Um dem Benutzer die Bearbeitungsberechtigungen zu entziehen, entfernen Sie entweder den Benutzer aus der Gruppe Editor oder ändern Sie die Rolle der gesamten Gruppe in Viewer.


1. Klicken Sie auf **[!UICONTROL Speichern]**. Die Rolle wird für den entsprechenden Benutzer geändert. Wenn Sie mehrere Benutzer ausgewählt haben, werden die Rollen für alle ausgewählten Benutzer gleichzeitig geändert.

   >[!NOTE]
   >
   >Änderungen in den Benutzerberechtigungen werden auf der Seite **[!UICONTROL Benutzerrollen]** erst dann angezeigt, wenn sich die Benutzer erneut bei Brand Portal anmelden.

## Verwalten von Gruppenrollen und -berechtigungen {#manage-group-roles-and-privileges}

Ein Administrator kann einer [Gruppe](../using/brand-portal-adding-users.md#main-pars-title-278567577) von Benutzern in Brand Portal bestimmte Berechtigungen zuweisen. Auf der Registerkarte **[!UICONTROL Gruppen]** der Seite **[!UICONTROL Benutzerrollen]** können Administratoren Folgendes tun:

* Sie können Benutzergruppen Rollen zuweisen.
* Schränken Sie Benutzergruppen ein, die Original-Ausgabedarstellungen von Bilddateien (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) aus Brand Portal herunterladen können.

>[!NOTE]
>
>Für die als Link freigegebenen Assets gilt die Berechtigung zum Zugriff auf die Original-Ausgabedarstellungen von Bilddateien basierend auf den Berechtigungen des Benutzers, der die Assets freigibt.

Führen Sie die folgenden Schritte aus, um die Rolle und die Berechtigung für den Zugriff auf die Originalwiedergaben für bestimmte Gruppenmitglieder zu ändern:

1. Navigieren Sie auf der Seite **[!UICONTROL Benutzerrollen]** zur Registerkarte **[!UICONTROL Gruppen]**.
1. Wählen Sie die Gruppen aus, deren Rollen geändert werden sollen.
1. Wählen Sie die entsprechende Rolle in der Dropdown-Liste **[!UICONTROL Rolle]** aus.

   Damit Gruppenmitglieder auf Original-Ausgabedarstellungen von Bilddateien zugreifen können, die sie über das Portal oder den freigegebenen Link herunterladen, lassen Sie die Option **[!UICONTROL Zugriff auf Original]** für diese Gruppe ausgewählt. Dieser Ansatz umfasst Dateitypen wie die folgenden:

   * .jpeg
   * .tiff
   * .png
   * .bmp
   * .gif
   * .pjpeg
   * .psd
   * x-portable-anymap
   * x-portable-bitmap
   * X-portable-graymap
   * X-portable-pixmap
   * x-rgb
   * x-xbitmap
   * x-xpixmap
   * x-icon
   * image/photoshop
   * image/x-photoshop
   * image/vnd.adobe.photoshop

   Standardmäßig ist die Option **[!UICONTROL Zugriff auf Original]** für alle Benutzer aktiviert. Möchten Sie verhindern, dass eine Benutzergruppe auf Original-Ausgabedarstellungen zugreifen kann, heben Sie die Auswahl der Option für diese Gruppe auf.

   ![Benutzergruppenrollen](assets/access-original-rend.png)

   >[!NOTE]
   >
   >Wenn ein Benutzer mehreren Gruppen hinzugefügt wird und eine dieser Gruppen über Einschränkungen verfügt, gelten die Einschränkungen für diesen Benutzer.
   >
   >Außerdem gelten die Einschränkungen für den Zugriff auf die Original-Ausgabedarstellungen von Bilddateien nicht für Admins, auch wenn sie Mitglieder von eingeschränkten Gruppen sind.


1. Klicken Sie auf **[!UICONTROL Speichern]**. Die Rolle wird für die entsprechenden Gruppen geändert.

   >[!NOTE]
   >
   >Die Verknüpfung von Benutzer zu Gruppe bzw. die Gruppenmitgliedschaft eines Benutzers wird alle 8 Stunden mit Brand Portal synchronisiert. Änderungen bei Benutzer- oder Gruppenrollen treten nach Abschluss der nächsten Synchronisierung in Kraft.
