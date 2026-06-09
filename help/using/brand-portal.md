---
title: Überblick über Experience Manager Assets Brand Portal
description: Erfahren Sie, wie Sie mit Experience Manager Assets Brand Portal genehmigte Kreativ-Assets einfach abrufen, kontrollieren und sicher und geräteübergreifend an externe Parteien und interne Geschäftsbenutzer verteilen können.
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
TQID: https://experienceleague.adobe.com/oBDmsUsNSLapEzQa9r4J-vZqTz2qe0cPW6hU1EYzrXU
product_v2:
  - id: d09181b5-a36a-43de-ba01-36641440bc43
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2:
  - id: da0dfbce-df02-4f8b-b32d-a4e3b1d05085
subfeature_v2:
  - id: e00c7c12-7035-41fe-ad76-1ec82c8c3f01
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 870850fd29819d96017608f1db48d46b38c62bff
workflow-type: tm+mt
source-wordcount: 1549
ht-degree: 55%

---

# Überblick über Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als Marketing-Experte müssen Sie manchmal mit Channel-Partnern und internen Geschäftsbenutzern zusammenarbeiten, um relevante digitale Inhalte für Kunden zu erstellen, zu verwalten und schnell bereitzustellen. Die zeitnahe Bereitstellung relevanter Inhalte für die gesamte Customer Journey ist ein wichtiger Faktor für Nachfragegenerierung, Konversionen, Interaktionen und Kundentreue.

Die Entwicklung von Lösungen, die die effiziente und sichere Freigabe von Dingen wie genehmigten Markenlogos, Kampagnen-Assets oder Produkt-Shots mit Teams, Partnern und Wiederverkäufern unterstützen, stellt jedoch eine Herausforderung dar. Um in diesem Prozess sowohl Effizienz als auch Sicherheit zu gewährleisten, ist eine sorgfältige Planung und Ausführung erforderlich.

**Adobe Experience Manager (AEM) Assets Brand Portal** konzentriert sich auf die Notwendigkeit der Zusammenarbeit des Marketing-Experten mit den global verteilten Brand Portal-Benutzern durch die Bereitstellung von Funktionen zur Asset-Verteilung und zum Asset-Beitrag.

Mit der Asset-Verteilung können Sie genehmigte Kreativ-Assets abrufen, kontrollieren und sicher und geräteübergreifend an externe Parteien und interne Geschäftsbenutzer verteilen. Der Asset-Beitrag ermöglicht es den Brand Portal-Benutzenden jedoch, Assets in Brand Portal hochzuladen und in Experience Manager Assets zu veröffentlichen, ohne Zugriff auf die Autorenumgebung zu benötigen. Die Beitragsfunktion wird in Brand Portal als **Assets-Beschaffung bezeichnet**. Gemeinsam verbessern sie das Brand Portal-Gesamterlebnis bei der Asset-Verteilung und -Bereitstellung durch Brand Portal-Benutzende (externe Agenturen/Teams), beschleunigen die Time-to-Market für Assets und verringern das Risiko von Verstößen gegen Richtlinien und unbefugtem Zugriff.
Siehe [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).

Die browserbasierte Portalumgebung ermöglicht das einfache Hochladen, Durchsuchen, Suchen, Anzeigen einer Vorschau und Exportieren von Assets in genehmigten Formaten.

## Konfigurieren von Experience Manager Assets mit Brand Portal {#configure-brand-portal}

Die Konfiguration von Adobe Experience Manager Assets mit Brand Portal bietet Benutzern von Brand Portal Funktionen zur Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets.

>[!NOTE]
>
>Die Konfiguration von Experience Manager Assets mit Brand Portal wird von Experience Manager Assets as a Cloud Service sowie Experience Manager Assets 6.3 und höher unterstützt.

>[!IMPORTANT]
>
> * Brand Portal befindet sich im Wartungsmodus. Alle neuen Produktinnovationen sind in [Content Hub](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview) verfügbar.
> * Wenn Sie Brand Portal noch aktivieren müssen, wenden Sie sich mit Details zu Ihrem Anwendungsfall und anderen spezifischen Anforderungen an den Adobe-Support.
> * Brand Portal ist nicht mit [Assets Prime](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/assets-prime) oder [Assets Ultimate](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/assets-ultimate-overview) verfügbar. Bestehende Assets as a Cloud Service-Kunden, die bereits Zugriff auf Brand Portal haben, können diese jedoch auch bei der Umstellung auf Assets Ultimate verwenden.

<!--Experience Manager Assets as a Cloud Service is automatically configured with Brand Portal by activating Brand Portal from the Cloud Manager. The activation workflow creates the required configurations at the backend and activates Brand Portal on the same IMS org as of the Experience Manager Assets as a Cloud Service instance.-->

Experience Manager Assets (On-Premise und Managed Services) wird jedoch manuell mit Brand Portal mithilfe von Adobe Developer Console konfiguriert, wodurch ein Adobe Identity Management Services (IMS)-Token zur Autorisierung des Brand Portal-Mandanten abgerufen wird.

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

Experience Manager Assets Brand Portal ermöglicht den [Gastzugang](#request-access-to-brand-portal) zu Brand Portal. Ein Gastbenutzer benötigt keine Anmeldeinformationen, um das Portal aufzurufen, und hat Zugriff auf die öffentlichen Ordner (und Sammlungen). Als Gastbenutzer können Sie Asset-Details durchsuchen und eine vollständige Asset-Ansicht von Mitgliedern öffentlicher Ordner und Sammlungen anzeigen. Sie können öffentliche Assets suchen, herunterladen und zur Sammlung [!UICONTROL Lightbox] hinzufügen.

Die Gastsitzung verhindert jedoch, dass Sammlungen und gespeicherte Suchen erstellt werden. Benutzer in einer Gastsitzung können nicht auf Einstellungen für Ordner und Sammlungen zugreifen und keine Assets als Link freigeben. Diese Aufgaben kann ein Gastbenutzer ausführen:

* [Öffentliche Assets durchsuchen und darauf zugreifen](browse-assets-brand-portal.md)

* [Nach öffentlichen Assets suchen](brand-portal-searching.md)

* [Öffentliche Assets herunterladen](brand-portal-download-assets.md)

* [Assets zu [!UICONTROL Lightbox] hinzufügen](brand-portal-light-box.md#add-assets-to-lightbox)

Weitere Informationen finden Sie unter [Gastzugang zu Brand Portal](../using/guest-access.md).

### Betrachter {#viewer}

In der [!DNL Admin Console] definierter Brand Portal-Benutzer, der Zugriff auf Brand Portal mit der Rolle „Betrachter“ hat. Ein Benutzer mit dieser Rolle kann sich bei Brand Portal anmelden und auf zulässige Ordner, Sammlungen und Assets zugreifen. Der Benutzer kann außerdem Assets durchsuchen, als Vorschau anzeigen, herunterladen und exportieren (ursprüngliche oder bestimmte Ausgabedarstellungen), Kontoeinstellungen konfigurieren sowie Assets suchen. Diese Aufgaben kann eine Person mit der Rolle „Betrachter“ ausführen:

* [Durchsuchen von Assets](browse-assets-brand-portal.md)

* [Suchen nach Assets](brand-portal-searching.md)

* [Herunterladen von Assets](brand-portal-download-assets.md)

### Bearbeiter {#editor}

Benutzende mit der Rolle „Bearbeiter“ können alle Aufgaben ausführen, die der Rolle „Betrachter“ zur Verfügung stehen. Darüber hinaus kann ein Editor die Dateien und Ordner anzeigen, die ein Administrator freigibt. Benutzende mit der Rolle „Bearbeiter“ können außerdem Inhalte (Dateien, Ordner und Sammlungen) für andere Benutzende freigeben.

Neben den Aufgaben, die ein Betrachter ausführen kann, stehen dem Bearbeiter folgende Aufgaben zur Verfügung:

* [Freigeben von Ordnern](brand-portal-sharing-folders.md)

* [Freigeben von Sammlungen](brand-portal-share-collection.md)

* [Freigeben von Assets als Link](brand-portal-link-share.md)

### Administrator {#administrator}

Zu den Administratoren gehören Benutzer, die in der [!UICONTROL Admin Console als Systemadministrator oder Brand Portal-Produktadministrator markiert &#x200B;]. Administratoren können Systemadministratoren und Benutzer hinzufügen und entfernen, Vorgaben definieren, E-Mails an Benutzer senden sowie Portalnutzung und Speicherberichte anzeigen.

>[!NOTE]
>
>In Brand Portal hat ein Benutzer mit der Rolle „Support-Administrator“ in der [!UICONTROL Admin Console] dieselben Berechtigungen wie ein Systemadministrator.

Ein Administrator kann alle Aufgaben ausführen, die ein Bearbeiter ausführen kann. Im Folgenden finden Sie die zusätzlichen Aufgaben, die ein Administrator ausführen kann:

* [Verwalten von Benutzern, Gruppen und Benutzerrollen](brand-portal-adding-users.md)
* [Anpassen von Hintergrund, Seitenkopfzeilen und E-Mails](brand-portal-branding.md)
* [Verwenden benutzerdefinierter Suchfacetten](brand-portal-search-facets.md)
* [Verwenden eines Metadatenschemas](brand-portal-metadata-schemas.md)
* [Anwenden von Bildvorgaben oder dynamischen Ausgabedarstellungen](brand-portal-image-presets.md)
* [Arbeiten mit Berichten](brand-portal-reports.md)

Zusätzlich zu den oben genannten Aufgaben stehen AEM Assets-Autoren folgende Aufgaben zur Verfügung:

* [Konfigurieren von AEM Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md)
* [Veröffentlichen von Ordnern in Brand Portal](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-folder)
* [Veröffentlichen von Sammlungen in Brand Portal](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-collection)

## Alternativer Alias für Brand Portal-URL {#tenant-alias-for-portal-url}

Ab Brand Portal 6.4.3 können Unternehmen für jede vorhandene URL ihres Brand Portal-Mandanten eine alternative (Alias-)URL verwenden. Die Alias-URL kann erstellt werden, indem ein alternatives Präfix in die URL eingefügt wird.\
Wenn der Mandantenname mehr als 32 Zeichen umfasst, muss ein Mandantenalias erstellt werden.
Beachten Sie, dass nur das Präfix der Brand Portal-URL angepasst werden kann und nicht die gesamte URL. Für eine Organisation mit der vorhandenen Domain `geomettrix.brand-portal.adobe.com` kann beispielsweise auf Anfrage `geomettrixinc.brand-portal.adobe.com` erstellt werden.

Die AEM-Autoreninstanz kann jedoch nur mit [&#x200B; Mandanten-ID-URL &#x200B;](../using/configure-aem-assets-with-brand-portal.md) nicht mit der (alternativen) Mandantenalias-URL konfiguriert werden.

>[!NOTE]
>
>Um einen Alias für den Mandantennamen in einer vorhandenen Portal-URL zu erhalten, müssen Unternehmen den Kunden-Support kontaktieren und die Erstellung eines neuen Mandantenalias anfordern. Überprüfen Sie zunächst, ob der Alias verfügbar ist, und erstellen Sie dann den Alias, um diese Anfrage zu verarbeiten.
>
>Um den alten Alias zu ersetzen oder zu löschen, muss derselbe Prozess befolgt werden.

## Anfordern von Zugriff auf Brand Portal {#request-access-to-brand-portal}

Benutzer können über den Anmeldebildschirm Zugriff auf Brand Portal anfragen. Diese Anfragen werden an Brand Portal-Administratoren gesendet, die über die [!UICONTROL Adobe Admin Console] den Zugriff für Benutzer gewähren. Sobald der Zugriff gewährt wurde, erhalten die Benutzenden eine Benachrichtigungs-E-Mail.

Gehen Sie wie folgt vor, um Zugriff anzufragen:

1. Wählen Sie auf der Brand Portal-Anmeldeseite die Option **[!UICONTROL Hier klicken]** entsprechend **[!UICONTROL Zugriff erforderlich?]**. Um jedoch einer Gastsitzung beizutreten, wählen Sie **[!UICONTROL Hier klicken]** neben **[!UICONTROL Gastzugang?]**.

   ![Brand Portal-Anmeldebildschirm](assets/bp-login-requestaccess.png)

   Die Seite [!UICONTROL Zugriff anfragen] wird geöffnet.

1. Um Zugriff auf das Brand Portal eines Unternehmens anzufragen, benötigen Sie eine gültige [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] oder [!UICONTROL Federated ID].

   Melden Sie sich auf der Seite [!UICONTROL Zugriff anfordern] mit Ihrer ID an (Szenario 1) oder erstellen Sie eine [!UICONTROL Adobe ID] (Szenario 2):

   ![[!UICONTROL Zugriff anfordern]](assets/bplogin_request_access_2.png)

   **Szenario 1**

   1. Wenn Sie über eine [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] oder [!UICONTROL Federated ID] verfügen, klicken Sie auf **[!UICONTROL Anmelden]**.
Die [!UICONTROL Anmeldeseite] wird geöffnet.

   1. Geben Sie Ihre [!UICONTROL Adobe ID]-Anmeldeinformationen ein und klicken Sie auf **[!UICONTROL Anmelden]**.

      ![Adobe-Anmeldung](assets/bplogin_request_access_3.png)

   Sie werden zur Seite [!UICONTROL Zugriff anfordern] weitergeleitet.

   **Szenario 2**

   1. Wenn Sie nicht über eine [!UICONTROL Adobe ID] verfügen, um eine zu erstellen, klicken Sie auf **[!UICONTROL Adobe ID abrufen]** auf der Seite [!UICONTROL Zugriff anfordern].
Die [!UICONTROL Anmeldeseite] wird geöffnet.
   1. Klicken Sie **[!UICONTROL Adobe ID abrufen]**.
Die [!UICONTROL Anmeldeseite] wird geöffnet.
   1. Geben Sie Ihren Vornamen und Nachnamen, E-Mail-Adresse und Passwort ein.
   1. Wählen Sie **[!UICONTROL Anmelden]** aus.

      ![](assets/bplogin_request_access_5.png)

   Sie werden zur Seite [!UICONTROL Zugriff anfordern] weitergeleitet.

1. Auf der nächsten Seite werden der Name des aktuellen Benutzers und die E-Mail-Adresse angezeigt, die zum Anfordern des Zugriffs genutzt werden. Hinterlassen Sie einen Kommentar für den Administrator und klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/bplogin-request-access.png)

## Produkt-Administratoren gewähren Zugriff {#grant-access-to-brand-portal}

Brand Portal-Produkt-Administratoren erhalten die Zugriffsanforderungen im Brand Portal-Benachrichtigungsbereich und per E-Mail ins Postfach.

![Benachrichtigung zu Zugriffsanforderungen](assets/bplogin_request_access_7.png)

Um den Zugriff zu gewähren, müssen Produktadministratoren auf die entsprechende Benachrichtigung im Brand Portal-Benachrichtigungsbereich und dann auf **[!UICONTROL Zugriff gewähren]** klicken.
Alternativ können Produkt-Administratoren dem in der E-Mail mit der Zugriffsanfrage angegebenen Link folgen, um die Adobe [!UICONTROL Admin Console] aufzurufen und den Benutzer zur entsprechenden Produktkonfiguration hinzuzufügen.

Sie werden zur Homepage der [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) weitergeleitet. Verwenden Sie die Adobe [!UICONTROL Admin Console], um Benutzende zu erstellen und diese Produktprofilen (ehemals „Produktkonfigurationen„) zuzuweisen, die in Brand Portal als Gruppen angezeigt werden. Weitere Informationen zum Hinzufügen von Benutzern in der [!UICONTROL Admin Console] finden Sie unter [Hinzufügen von Benutzern](brand-portal-adding-users.md#add-a-user) (befolgen Sie Schritte 4 bis 7, um einen Benutzer hinzuzufügen).

## Brand Portal-Sprachen {#brand-portal-language}

Sie können die Brand Portal-Sprache in Adobe [!UICONTROL Experience Cloud-Einstellungen] ändern.

![Benachrichtigung zu Zugriffsanforderungen](assets/BPLang.png)

Gehen Sie wie folgt vor, um die Sprache zu ändern:

1. Wählen Sie im oberen Menü [!UICONTROL Benutzer] > [!UICONTROL Profil bearbeiten] aus.

   ![Profil bearbeiten](assets/EditBPProfile.png)

1. Wählen Sie auf [!UICONTROL &#x200B; Seite Experience &#x200B;]-Einstellungen eine Sprache aus dem [!UICONTROL -Menü &#x200B;]Sprache“ aus.

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

* [AEM-Foren](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community?profile.language=de)
