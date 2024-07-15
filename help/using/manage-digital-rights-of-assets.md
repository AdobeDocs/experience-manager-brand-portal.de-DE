---
title: Verwalten der digitalen Rechte von Assets
seo-title: Manage digital rights of assets
description: Das Lizenzieren von Assets und das Festlegen eines Ablaufdatums für Assets und freigegebene Links ermöglichen eine kontrollierte Asset-Nutzung und den Schutz dieser Assets.
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 84%

---

# Verwalten der digitalen Rechte von Assets {#manage-digital-rights-of-assets}

Eine sichere Verteilung und Nutzung von Kreativ-Assets und Markenmaterial ist für den Schutz Ihrer Marke wichtig. Dies kann innerhalb und außerhalb des Unternehmens durch das Verknüpfen eines Ablaufdatums (und einer Uhrzeit) mit genehmigten Assets, die aus AEM in Brand Portal veröffentlicht werden, oder durch Lizenzierung dieser Assets für die bedingte Verwendung durchgesetzt werden. Außerdem können Sie mit Brand Portal ein Ablaufdatum für Links zu den Assets angeben, die über Brand Portal freigegeben werden.

Lesen Sie weiter, um zu erfahren, wie die Assets in Brand Portal gesichert werden, und lernen Sie die zugehörigen Nutzungsberechtigungen kennen.

## Asset-Ablauf {#asset-expiration}

Der Asset-Ablauf ist eine effektive Möglichkeit, die Nutzung der genehmigten Assets in Brand Portal unternehmensweit zu kontrollieren. Alle Assets, die aus AEM Assets in Brand Portal veröffentlicht werden, können ein Ablaufdatum haben, das die Nutzung dieser Assets durch verschiedene Benutzerrollen einschränkt.

### Nutzungsberechtigungen in Bezug auf abgelaufene Assets {#usage-permissions-expired-assets}

In Brand Portal können Administratoren abgelaufene Assets anzeigen, herunterladen und zu Sammlungen hinzufügen. Bearbeiter und Betrachter können dagegen nur abgelaufene Assets anzeigen und sie zu Sammlungen hinzufügen.

Administratoren können abgelaufene Assets aus AEM Assets in Brand Portal veröffentlichen. Abgelaufene Assets können jedoch nicht über einen Link aus Brand Portal freigegeben werden. Wenn Sie ein abgelaufenes Asset aus einem Ordner auswählen, der sowohl abgelaufene als auch nicht abgelaufene Assets enthält, ist die Aktion **[!UICONTROL Link freigeben]** nicht verfügbar. Wenn Sie jedoch einen Ordner auswählen, der abgelaufene und nicht abgelaufene Assets enthält, sind die Aktionen [!UICONTROL Freigeben] und **[!UICONTROL Link freigeben]** verfügbar.

>[!NOTE]
>
>Ein Ordner kann als Link freigegeben werden, selbst wenn er abgelaufene Assets enthält. In diesem Fall werden im Link keine abgelaufenen Assets aufgelistet und nur die nicht abgelaufenen Assets werden freigegeben.

In der folgenden Tabelle werden die Nutzungsberechtigungen der abgelaufenen Assets angezeigt:

|   | **[!UICONTROL Linkfreigabe]** | **[!UICONTROL Download]** | **[!UICONTROL Eigenschaften]** | **[!UICONTROL Zu Sammlung hinzufügen]** | **[!UICONTROL Löschen]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrator]** | Nicht verfügbar | Verfügbar | Verfügbar | Verfügbar | Verfügbar |
| **[!UICONTROL Bearbeiter]** | Nicht verfügbar | Nicht verfügbar | Verfügbar | Verfügbar | Nicht verfügbar |
| **[!UICONTROL Betrachter]** | Nicht verfügbar | Nicht verfügbar | Verfügbar | Verfügbar | Nicht verfügbar |
| **[!UICONTROL Gastbenutzer]** | Nicht verfügbar | Nicht verfügbar | Verfügbar | Verfügbar | Nicht verfügbar |

>[!NOTE]
>
>Wenn Betrachter und Bearbeiter einen Ordner mit abgelaufenen und nicht abgelaufenen Assets herunterladen, werden nur die nicht abgelaufenen Assets heruntergeladen. Wenn ein Ordner nur abgelaufene Assets enthält, wird ein leerer Ordner heruntergeladen.

### Gültigkeitsstatus und Assets {#expiration-status-of-assets}

Sie können den Gültigkeitsstatus der Assets in der **[!UICONTROL Kartenansicht]** anzeigen. Eine rote Markierung auf der Karte zeigt an, dass das Asset abgelaufen ist.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>In Listen- und Spaltenansichten wird der Ablaufstatus von Assets nicht angezeigt.

## Ablauf des Asset-Links {#asset-link-expiration}

Beim Teilen von Assets über Links können Administratoren und Bearbeiter über das Feld **[!UICONTROL Ablauf]** im Dialogfeld **[!UICONTROL Linkfreigabe]** ein Ablaufdatum und eine Ablaufuhrzeit einstellen. Standardmäßig beträgt die Ablauffrist des Links sieben Tage ab dem Datum, an dem der Link freigegeben wird.

![](assets/asset-link-sharing.png)

So wird sichergestellt, dass Assets, die als Links freigegeben werden, an dem Tag und zu der Uhrzeit ablaufen, die Brand Portal-Administratoren und -Bearbeiter festgelegt haben. Nach diesem Ablaufdatum können sie nicht mehr angezeigt und heruntergeladen werden. Da die über Links freigegebenen Assets auch von externen Benutzern angezeigt werden können, die nicht zur Organisation gehören, können Sie durch Festlegen des Ablaufs sicherstellen, dass Ihre genehmigten Assets geschützt sind und über einen bestimmten Zeitraum für keine unbekannten Personen sichtbar sind.

Weitere Informationen zur Linkfreigabe finden Sie unter [Assets als Link freigeben](../using/brand-portal-link-share.md).

## Lizenzierte Assets {#licensed-assets}

Das Herunterladen von lizenzierten Assets aus Brand Portal unterliegt einer Lizenzvereinbarung. Diese Vereinbarung für lizenzierte Assets wird angezeigt, wenn Sie das Asset direkt aus Brand Portal oder über einen freigegebenen Link herunterladen. Unabhängig davon, ob die Assets abgelaufen sind oder nicht, können alle Benutzer lizenzgeschützte Assets anzeigen. Das Herunterladen und Verwenden abgelaufener lizenzierter Assets ist jedoch eingeschränkt. Informationen zum Verhalten abgelaufener lizenzierter Assets und zulässiger Aktivitäten basierend auf Benutzerrollen finden Sie unter [Nutzungsberechtigungen abgelaufener Assets](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

Lizenzgeschützte Assets verfügen über eine [angehängte Lizenzvereinbarung](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html?lang=de). Dies geschieht, indem die Metadateneigenschaften des Assets in [!DNL Experience Manager Assets] festgelegt werden.

Ein Asset gilt als geschützt, wenn es eine der folgenden (oder beide) Metadateneigenschaften enthält:

* `xmpRights:WebStatement`: Diese Eigenschaft verweist auf den Pfad der Seite, die die Lizenzvereinbarung für das Asset enthält. `xmpRights:WebStatement` sollte ein gültiger Pfad im Repository sein.
* `adobe_dam:restrictions`: Beim Wert dieser Eigenschaft handelt es sich um unformatierten HTML-Code, der die Lizenzvereinbarung angibt.


Wenn Sie sich für das Herunterladen von lizenzgeschützten Assets entscheiden, werden Sie je nach den Eigenschaften der Metadaten auf die Seite **[!UICONTROL Copyright-Management]** umgeleitet.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | Copyright-Management |
| --- | --- | --- |
| Ja | - | Die Benutzeroberfläche wird sowohl in Assets als auch in Brand Portal angezeigt |
| - | Ja (ungültiger Pfad) | Keine Schnittstelle |
| Ja | Ja (ungültiger Pfad) | Keine Schnittstelle |
| Ja | Ja (gültiger Pfad) | Die Benutzeroberfläche wird in Assets oder Brand Portal angezeigt </br> Abhängig davon, ob der Pfad für Assets oder Brand Portal (oder beides) gültig ist. |

![](assets/asset-copyright-mgmt.png)

Hier müssen Sie das Asset auswählen, das Sie herunterladen möchten, und die zugehörige Lizenzvereinbarung akzeptieren. Wenn Sie die Lizenzvereinbarung nicht annehmen, wird die Schaltfläche **[!UICONTROL Herunterladen]** nicht aktiviert.

![](assets/licensed-asset-download-2.png)

Falls die Auswahl mehrere geschützte Assets enthält, wählen Sie jeweils eines aus, nehmen Sie die Lizenzvereinbarung an und fahren Sie mit dem Herunterladen des Assets fort.

## Erstellen von Berichten zu abgelaufenen Assets {#generate-report-about-expired-assets}

Administratoren können einen Bericht erstellen und herunterladen, in dem alle Assets aufgeführt sind, die innerhalb eines bestimmten Zeitraums abgelaufen sind. Dieser Bericht enthält ausführliche Informationen zu den abgelaufenen Assets, etwa Größe, Art, Pfad mit der angegebenen Position des Assets in der Asset-Hierarchie, Ablaufdatum des Assets und dessen Veröffentlichungszeitpunkt. Die Spalten dieses Berichts können angepasst werden, um basierend auf den Benutzeranforderungen mehr Daten anzuzeigen.

![](assets/assets-expired.png)

Weitere Informationen zur Berichtsfunktion finden Sie unter [Mit Berichten arbeiten](../using/brand-portal-reports.md#work-with-reports).
