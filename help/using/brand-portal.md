---
title: Überblick über Experience Manager Assets Brand Portal
description: Erfahren Sie, wie Sie mit Experience Manager Assets Brand Portal problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen können.
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 60%

---

# Überblick über Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als Marketing-Experte müssen Sie manchmal mit Vertriebspartnern und internen Geschäftsbenutzern zusammenarbeiten, um relevante digitale Inhalte zu erstellen, zu verwalten und schnell für Kunden bereitzustellen. Die zeitnahe Bereitstellung relevanter Inhalte für die gesamte Customer Journey ist ein wichtiger Faktor für Nachfragegenerierung, Konversionen, Interaktionen und Kundenloyalität.

Die Entwicklung von Lösungen, die die effiziente und sichere Freigabe von Elementen wie genehmigten Marken-Logos, Kampagnen-Assets oder Produktfotos für Teams, Partner und Wiederverkäufer unterstützen, ist jedoch eine Herausforderung. Die Sicherstellung von Effizienz und Sicherheit in diesem Prozess erfordert eine sorgfältige Planung und Ausführung.

**Adobe Experience Manager (AEM) Assets Brand Portal** konzentriert sich auf das Bedürfnis des Marketingexperten, effektiv mit den global verteilten Brand Portal-Benutzern zusammenzuarbeiten, indem es Asset-Verteilungs- und Asset-Beitragsfunktionen bereitstellt.

Mit der Asset-Verteilung können Sie genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen. Der Asset-Beitrag ermöglicht es Brand Portal-Benutzern jedoch, Assets in Brand Portal hochzuladen und in Experience Manager Assets zu veröffentlichen, ohne Zugriff auf die Autorenumgebung zu benötigen. Die Beitragsfunktion wird als **Asset-Beschaffung in Brand Portal** bezeichnet. Zusammengenommen verbessert sie die gesamte Brand Portal-Erfahrung bei der Verteilung von Assets und den Beiträgen der Brand Portal-Benutzer (externen Agenturen/Teams), beschleunigt die Markteinführung von Assets und verringert das Risiko von Nichteinhaltung und unbefugtem Zugriff.
Siehe [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).

Die browserbasierte Portalumgebung ermöglicht es Ihnen, Assets einfach in genehmigten Formaten hochzuladen, zu durchsuchen, zu suchen, in der Vorschau anzuzeigen und zu exportieren.

## Konfigurieren von Experience Manager Assets mit Brand Portal {#configure-brand-portal}

Die Konfiguration von Adobe Experience Manager Assets mit Brand Portal bietet Benutzern von Brand Portal Funktionen zur Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets.

>[!NOTE]
>
>Die Konfiguration von Experience Manager Assets mit Brand Portal wird von Experience Manager Assets as a Cloud Service sowie Experience Manager Assets 6.3 und höher unterstützt.

Experience Manager Assets as a Cloud Service wird automatisch mit Brand Portal konfiguriert, indem Brand Portal über Cloud Manager aktiviert wird. Der Aktivierungs-Workflow erstellt die erforderlichen Konfigurationen im Backend und aktiviert Brand Portal in derselben IMS-Org wie die Experience Manager Assets as a Cloud Service-Instanz.

Experience Manager Assets (On-Premise und verwalteter Dienst) wird jedoch mithilfe von Adobe Developer Console manuell mit Brand Portal konfiguriert, das ein Adobe Identity Management Services (IMS)-Token zur Autorisierung des Brand Portal-Mandanten abruft.

Weitere Informationen finden Sie unter [Konfigurieren von Experience Manager Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Benutzerrollen in Brand Portal {#Personas}

Brand Portal unterstützt die folgenden Benutzerrollen:

* Gastbenutzer
* Betrachter
* Bearbeiter
* Administrator

Die folgende Tabelle enthält die Aufgaben, die Benutzer mit diesen Rollen ausführen können:

|  | **Durchsuchen** | **Suchen** | **Download** | **Freigeben von Ordnern** | **Freigeben von Sammlungen** | **Freigeben von Assets als Link** | **Zugriff auf Admin-Tools** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Gastbenutzer** | ✓* | ✓* | ✓* | x | x | x | x |
| **Betrachter** | ✓ | ✓ | ✓ | x | x | x | x |
| **Bearbeiter** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrator** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>Gastbenutzer können nur Assets durchsuchen, auf Assets zugreifen oder nach Assets suchen, die sich in öffentlichen Ordnern und Sammlungen befinden.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Gastbenutzer {#guest-user}

Experience Manager Assets Brand Portal ermöglicht den [Gastzugang](#request-access-to-brand-portal) zu Brand Portal. Ein Gastbenutzer benötigt keine Anmeldeinformationen, um das Portal aufzurufen, und hat Zugriff auf die öffentlichen Ordner (und Sammlungen). Als Gastbenutzer können Sie Asset-Details durchsuchen und eine vollständige Asset-Ansicht der Mitglieder öffentlicher Ordner und Sammlungen erhalten. Sie können öffentliche Assets suchen, herunterladen und zur Sammlung [!UICONTROL Lightbox] hinzufügen.

Die Gastsitzung verhindert jedoch, dass Sie Sammlungen und gespeicherte Suchen erstellen und diese weiter freigeben. Benutzer in einer Gastsitzung können nicht auf Einstellungen für Ordner und Sammlungen zugreifen und Assets nicht als Link freigeben. Diese Aufgaben kann ein Gastbenutzer ausführen:

* [Öffentliche Assets durchsuchen und darauf zugreifen](browse-assets-brand-portal.md)

* [Nach öffentlichen Assets suchen](brand-portal-searching.md)

* [Öffentliche Assets herunterladen](brand-portal-download-assets.md)

* [Assets zu [!UICONTROL Lightbox] hinzufügen](brand-portal-light-box.md#add-assets-to-lightbox)

Weitere Informationen finden Sie unter [Gastzugang für Brand Portal](../using/guest-access.md).

### Betrachter {#viewer}

Brand Portal-Benutzer definiert in der [!DNL Admin Console] , der Zugriff auf Brand Portal mit der Rolle &quot;Betrachter&quot;hat. Ein Benutzer mit dieser Rolle kann sich bei Brand Portal anmelden und auf zulässige Ordner, Sammlungen und Assets zugreifen. Der Benutzer kann außerdem Assets durchsuchen, als Vorschau anzeigen, herunterladen und exportieren (ursprüngliche oder bestimmte Ausgabedarstellungen), Kontoeinstellungen konfigurieren sowie Assets suchen. Diese Aufgaben kann eine Person mit der Rolle „Betrachter“ ausführen:

* [Durchsuchen von Assets](browse-assets-brand-portal.md)

* [Suchen nach Assets](brand-portal-searching.md)

* [Herunterladen von Assets](brand-portal-download-assets.md)

### Bearbeiter {#editor}

Benutzende mit der Rolle „Bearbeiter“ können alle Aufgaben ausführen, die der Rolle „Betrachter“ zur Verfügung stehen. Zusätzlich kann eine Person mit der Rolle „Bearbeiter“ die Dateien und Ordner anzeigen, die von der oder dem Admin freigegeben wurden. Benutzende mit der Rolle „Bearbeiter“ können außerdem Inhalte (Dateien, Ordner und Sammlungen) für andere Benutzende freigeben.

Neben den Aufgaben, die ein Betrachter ausführen kann, stehen dem Bearbeiter folgende Aufgaben zur Verfügung:

* [Freigeben von Ordnern](brand-portal-sharing-folders.md)

* [Freigeben von Sammlungen](brand-portal-share-collection.md)

* [Freigeben von Assets als Link](brand-portal-link-share.md)

### Administrator {#administrator}

Zu den Administratoren gehören Benutzer, die in der [!UICONTROL Admin Console] als Systemadministrator oder Brand Portal-Produktadministrator gekennzeichnet sind. Administratoren können Systemadministratoren und Benutzer hinzufügen und entfernen, Vorgaben definieren, E-Mails an Benutzer senden sowie Portalnutzung und Speicherberichte anzeigen.

>[!NOTE]
>
>In Brand Portal hat ein Benutzer, der in der [!UICONTROL Admin Console] als Support-Administrator gekennzeichnet ist, dieselben Berechtigungen wie ein Systemadministrator.

Ein Administrator kann alle Aufgaben ausführen, die ein Bearbeiter ausführen kann. Im Folgenden finden Sie die zusätzlichen Aufgaben, die ein Administrator ausführen kann:

* [Verwalten von Benutzern, Gruppen und Benutzerrollen](brand-portal-adding-users.md)
* [Anpassen von Hintergrund, Seitenkopfzeilen und E-Mails](brand-portal-branding.md)
* [Verwenden benutzerdefinierter Suchfacetten](brand-portal-search-facets.md)
* [Verwenden des Metadatenschemas](brand-portal-metadata-schemas.md)
* [Anwenden von Bildvorgaben oder dynamischen Ausgabedarstellungen](brand-portal-image-presets.md)
* [Arbeiten mit Berichten](brand-portal-reports.md)

Zusätzlich zu den oben genannten Aufgaben stehen AEM Assets-Autoren folgende Aufgaben zur Verfügung:

* [Konfigurieren von AEM Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md)
* [Veröffentlichen von Ordnern in Brand Portal](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-folder)
* [Veröffentlichen von Sammlungen in Brand Portal](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-collection)

## Alternativer Alias für Brand Portal-URL {#tenant-alias-for-portal-url}

Ab Brand Portal 6.4.3 können Unternehmen für jede vorhandene URL ihres Brand Portal-Mandanten über eine alternative URL (Alias) verfügen. Die Alias-URL kann erstellt werden, indem ein alternatives Präfix in die URL eingefügt wird.\
Wenn der Mandantenname länger als 32 Zeichen ist, muss ein Mandantenalias erstellt werden.
Beachten Sie, dass nur das Präfix der Brand Portal-URL angepasst werden kann und nicht die gesamte URL. Für eine Organisation mit der vorhandenen Domain `geomettrix.brand-portal.adobe.com` kann beispielsweise auf Anfrage die Domain `geomettrixinc.brand-portal.adobe.com` erstellt werden.

Die AEM-Autoreninstanz kann jedoch nur mit der Mandanten-ID-URL und nicht mit der (alternativen) Mandanten-Alias-URL [konfiguriert](../using/configure-aem-assets-with-brand-portal.md) werden.

>[!NOTE]
>
>Um einen Alias für den Mandantennamen in einer vorhandenen Portal-URL zu erhalten, müssen sich Unternehmen an den Kundensupport wenden und eine Anfrage zur Erstellung eines neuen Mandantenalias stellen. Überprüfen Sie zunächst, ob der Alias verfügbar ist, und erstellen Sie dann den Alias für die Verarbeitung dieser Anfrage.
>
>Um den alten Alias zu ersetzen oder zu löschen, muss der gleiche Prozess befolgt werden.

## Anfordern von Zugriff auf Brand Portal {#request-access-to-brand-portal}

Benutzer können über den Anmeldebildschirm Zugriff auf Brand Portal anfragen. Diese Anfragen werden an Brand Portal-Administratoren gesendet, die über die [!UICONTROL Adobe Admin Console] den Zugriff für Benutzer gewähren. Sobald der Zugriff gewährt wurde, erhalten die Benutzenden eine Benachrichtigungs-E-Mail.

Gehen Sie wie folgt vor, um Zugriff anzufragen:

1. Wählen Sie auf der Anmeldeseite von Brand Portal **[!UICONTROL Hier klicken]** neben **[!UICONTROL Benötigen Sie Zugriff?]**. Um jedoch einer Gastsitzung beizutreten, wählen Sie **[!UICONTROL Hier klicken]** neben **[!UICONTROL Gastzugang?]**.

   ![Brand Portal-Anmeldebildschirm](assets/bp-login-requestaccess.png)

   Die Seite [!UICONTROL Zugriff anfragen] wird geöffnet.

1. Um Zugriff auf das Brand Portal eines Unternehmens anzufragen, benötigen Sie eine gültige [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] oder [!UICONTROL Federated ID].

   Melden Sie sich auf der Seite [!UICONTROL Zugriff anfordern] mit Ihrer ID an (Szenario 1) oder erstellen Sie eine [!UICONTROL Adobe ID] (Szenario 2):

   ![[!UICONTROL Zugriff anfordern]](assets/bplogin_request_access_2.png)

   **Szenario 1**

   1. Wenn Sie bereits eine [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] oder [!UICONTROL Federated ID] haben, klicken Sie auf **[!UICONTROL Anmelden]**.
Die Seite [!UICONTROL Anmelden] wird geöffnet.

   1. Geben Sie Ihre [!UICONTROL Adobe ID]-Anmeldedaten ein und klicken Sie auf **[!UICONTROL Anmelden]**.

      ![Adobe-Anmeldung](assets/bplogin_request_access_3.png)

   Sie werden zur Seite [!UICONTROL Zugriff anfordern] weitergeleitet.

   **Szenario 2**

   1. Wenn Sie noch keine [!UICONTROL Adobe ID] haben, erstellen Sie die ID, indem Sie auf der Seite **[!UICONTROL Zugriff anfordern]** auf [!UICONTROL Adobe ID anfordern] klicken.
Die Seite [!UICONTROL Anmelden] wird geöffnet.
   1. Klicken Sie auf **[!UICONTROL Adobe ID anfordern]**.
Die Seite [!UICONTROL Anmelden] wird geöffnet.
   1. Geben Sie Ihren Vornamen und Nachnamen, E-Mail-Adresse und Passwort ein.
   1. Wählen Sie **[!UICONTROL Anmelden]** aus.

      ![](assets/bplogin_request_access_5.png)

   Sie werden zur Seite [!UICONTROL Zugriff anfordern] weitergeleitet.

1. Auf der nächsten Seite werden der Name des aktuellen Benutzers und die E-Mail-Adresse angezeigt, die zum Anfordern des Zugriffs genutzt werden. Geben Sie einen Kommentar für den Administrator ein und klicken Sie dann auf **[!UICONTROL Übermitteln]**.

   ![](assets/bplogin-request-access.png)

## Produkt-Administratoren gewähren Zugriff {#grant-access-to-brand-portal}

Brand Portal-Produkt-Administratoren erhalten die Zugriffsanforderungen im Brand Portal-Benachrichtigungsbereich und per E-Mail ins Postfach.

![Benachrichtigung zu Zugriffsanforderungen](assets/bplogin_request_access_7.png)

Um Zugriff zu gewähren, müssen Produktadministratoren auf die entsprechende Benachrichtigung im Brand Portal-Benachrichtigungsbereich klicken und dann auf **[!UICONTROL Zugriff gewähren]** klicken.
Alternativ können Produktadministratoren dem in der E-Mail mit der Zugriffsanfrage angegebenen Link folgen, um die Adobe [!UICONTROL Admin Console] aufzurufen und den Benutzer zur entsprechenden Produktkonfiguration hinzuzufügen.

Sie werden zur Homepage der [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) weitergeleitet. Verwenden Sie die Adobe [!UICONTROL Admin Console] , um Benutzer zu erstellen und diese Produktprofilen (ehemals &quot;Produktkonfigurationen&quot;) zuzuweisen, die in Brand Portal als Gruppen angezeigt werden. Weitere Informationen zum Hinzufügen von Benutzern in der [!UICONTROL Admin Console] finden Sie unter [Hinzufügen eines Benutzers](brand-portal-adding-users.md#add-a-user) (befolgen Sie die Schritte 4 bis 7, um einen Benutzer hinzuzufügen).

## Brand Portal-Sprachen {#brand-portal-language}

Sie können die Brand Portal-Sprache unter Adobe [!UICONTROL Experience Cloud-Einstellungen] ändern.

![Benachrichtigung zu Zugriffsanforderungen](assets/BPLang.png)

Gehen Sie wie folgt vor, um die Sprache zu ändern:

1. Wählen Sie im oberen Menü [!UICONTROL Benutzer] > [!UICONTROL Profil bearbeiten] aus.

   ![Profil bearbeiten](assets/EditBPProfile.png)

1. Wählen Sie auf der Seite [!UICONTROL Experience Cloud Settings] eine aus dem Dropdownmenü [!UICONTROL Language] aus.

## Wartungsbenachrichtigung in Brand Portal {#brand-portal-maintenance-notification}

Bevor Brand Portal planmäßig zur Wartung heruntergefahren wird, wird nach dem Anmelden bei Brand Portal eine Benachrichtigung als Banner angezeigt. Beispiel für eine Benachrichtigung:

![](assets/bp_maintenance_notification.png)

Sie können diese Benachrichtigung schließen und Brand Portal weiterhin verwenden. Diese Benachrichtigung erscheint bei jeder neuen Sitzung.

## Versions- und Systeminformationen {#release-and-system-information}

* [Neuerungen](whats-new.md)
* [Versionshinweise](brand-portal-release-notes.md)
* [Unterstützte Dateiformate](brand-portal-supported-formats.md)

## Verwandte Ressourcen {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM-Foren](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
