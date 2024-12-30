---
title: Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal
description: Erfahren Sie, wie Sie Probleme beim parallelen Veröffentlichen beheben können.
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: ce3a7a5232f32c86b4930f9079bed5f04d001d8f
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 49%

---

# Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

In Brand Portal wird die Konfiguration mit Experience Manager Assets unterstützt, damit genehmigte Marken-Assets nahtlos in die Experience Manager Assets-Autoreninstanz aufgenommen oder darin veröffentlicht werden können. Nach der [Konfiguration](../using/configure-aem-assets-with-brand-portal.md) repliziert die Benutzerin bzw. der Experience Manager-Autor mithilfe eines Replikationsagenten ein oder mehrere ausgewählte Assets zur genehmigten Verwendung durch Brand Portal-Benutzende in Brand Portal Cloud Service. In Experience Manager 6.2 SP1-CFP5, Experience Manager CFP 6.3.0.2 und höher werden mehrere Replikationsagenten verwendet, um eine schnelle parallele Veröffentlichung zu gewährleisten.

>[!NOTE]
>
>Um eine erfolgreiche Konfiguration von Experience Manager Assets Brand Portal mit Experience Manager Assets sicherzustellen, empfiehlt Adobe ein Upgrade auf Experience Manager 6.4.1.0. Aufgrund einer Einschränkung in Experience Manager 6.4 tritt beim Konfigurieren von Experience Manager Assets mit Brand Portal ein Fehler auf und die Replikation schlägt fehl.

Beim Konfigurieren eines Cloud Service für Brand Portal unter **[!UICONTROL /etc/cloudservice]** werden alle erforderlichen Benutzenden und Token automatisch generiert und im Repository gespeichert. Die Cloud-Service-Konfiguration wird erstellt, Service-Benutzer, die für Replikation und Replikationsagenten erforderlich sind, um Inhalte zu replizieren, werden ebenfalls erstellt. Hierbei werden vier Replikationsagenten erstellt. Wenn Sie zahlreiche Assets aus Experience Manager in Brand Portal veröffentlichen, werden diese in die Warteschlange gestellt und über Round Robin unter diesen Replikationsagenten verteilt.

Jedoch kann das Veröffentlichen zwischenzeitlich aufgrund zu großer Sling-Aufträge, erhöhter Netzwerk- und **[!UICONTROL Datenträger-E/A]** in der Experience Manager-Autoreninstanz oder geringer Leistung der Experience Manager-Autoreninstanz scheitern. Adobe empfiehlt, die Verbindung mit einem oder mehreren Replikationsagenten zu testen, bevor Sie mit der Veröffentlichung beginnen.

![](assets/test-connection.png)

## Beheben von Problemen bei der ersten Veröffentlichung: Überprüfen der Veröffentlichungskonfiguration {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

So validieren Sie Ihre Veröffentlichungskonfigurationen:

1. Fehlerprotokolle überprüfen
1. Überprüfen, ob der Replikationsagent erstellt wurde
1. Testen Sie die Verbindung.

**Prüfen der Protokollfragmente beim Erstellen des Cloud Service**

Überprüfen Sie die Tail-Protokolle. Überprüfen Sie, ob der Replikationsagent erstellt wurde oder nicht. Wenn die Erstellung des Replikationsagenten fehlschlägt, bearbeiten Sie den Cloud-Service, indem Sie kleinere Änderungen im Cloud-Service vornehmen. Validieren und überprüfen Sie erneut, ob der Replikationsagent erstellt wurde oder nicht. Falls nicht, bearbeiten Sie den Service erneut.

Wenn der Cloud Service beim wiederholten Bearbeiten nicht ordnungsgemäß konfiguriert ist, melden Sie ein Daycare-Ticket.

**Testen der Verbindung mit Replikationsagenten**

Protokoll anzeigen, wenn im Replikationsprotokoll Fehler gefunden werden:

1. Wenden Sie sich an den Adobe-Support.

1. Wiederholen Sie die [Bereinigung](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) und erstellen Sie die Veröffentlichungskonfiguration erneut.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## Vorhandene Veröffentlichungskonfigurationen in Brand Portal bereinigen {#clean-up-existing-config}

Die Veröffentlichung schlägt oft mit dem Fehler „401 unauthorized“ fehl, da dem Benutzer (z. B. `mac-<tenantid>-replication`) der neueste private Schlüssel fehlt und in den Replikationsagenten-Protokollen kein anderer Fehler gemeldet wird. Wenn Sie keine Problembehebung vornehmen möchten, können Sie stattdessen eine neue Konfiguration erstellen. Damit die neue Konfiguration richtig funktioniert, sollten Sie bei der Einrichtung der Experience Manager-Autoreninstanz Folgendes bereinigen:

1. Navigieren Sie zu `localhost:4502/crx/de/` (unter Berücksichtigung der Tatsache, dass Sie die Autoreninstanz auf `localhost:4502:` ausführen)
i. `/etc/replication/agents.author/mp_replication` löschen
II. Löschen von `/etc/cloudservices/mediaportal/<config_name>`

1. Gehen Sie zu localhost:4502/useradmin:\
   i. Nach `mac-<tenantid>replication` suchen
II. Diesen Benutzer löschen

Jetzt ist das System bereinigt. Jetzt können Sie versuchen, eine Cloud Service-Konfiguration zu erstellen und weiterhin die vorhandene JWT-Anwendung zu verwenden. Es ist nicht erforderlich, eine Anwendung zu erstellen. Aktualisieren Sie stattdessen den öffentlichen Schlüssel aus der neu erstellten Cloud-Konfiguration.

>[!NOTE]
>
>Ändern Sie keine automatisch generierten Einstellungen.


## Problem mit der Sichtbarkeit der Developer Connection-JWT-Anwendung {#developer-connection-jwt-application-tenant-visibility-issue}

Wenn auf `https://legacy-oauth.cloud.adobe.io/`, werden alle Organisationen (Mandanten) aufgelistet, für die die aktuellen Benutzer Systemadministrator sind. Wenn Sie den Organisationsnamen hier nicht finden oder Sie hier keine Anwendung für einen erforderlichen Mandanten erstellen können, überprüfen Sie, ob Sie über ausreichende (Systemadministrator-)Rechte verfügen.

Auf dieser Benutzeroberfläche gibt es ein bekanntes Problem, nämlich dass für jeden Mandanten nur die zehn wichtigsten Anwendungen sichtbar sind. Wenn Sie die Anwendung erstellen, bleiben Sie auf dieser Seite und erstellen Sie ein Lesezeichen für die URL. Navigieren Sie nicht zur Auflistungsseite des Programms und finden Sie das von Ihnen erstellte Programm. Sie können diese URL mit Lesezeichen direkt aufrufen und die Anwendung bei Bedarf aktualisieren oder löschen.

Die JWT-Anwendung wird unter Umständen nicht korrekt aufgelistet. Daher wird empfohlen, die URL beim Erstellen einer JWT-Anwendung zu notieren oder mit einem Lesezeichen zu versehen.

## Laufende Konfiguration funktioniert nicht mehr {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Wenn ein Replikationsagent, mit dem das Veröffentlichen in Brand Portal bisher korrekt funktionierte, keine Veröffentlichungsaufträge mehr verarbeitet, prüfen Sie die Replikationsprotokolle. In Experience Manager ist eine Funktion zur automatischen Wiederholung integriert. Wenn das Veröffentlichen eines bestimmten Assets scheitert, wird automatisch ein Wiederholungsversuch gestartet. Wenn ein temporäres Problem auftritt, z. B. ein Netzwerkfehler, kann es während eines erneuten Versuchs erfolgreich sein.

Wenn es kontinuierliche Veröffentlichungsfehler gibt und die Warteschlange blockiert ist, überprüfen Sie die **[!UICONTROL Testverbindung]**. Versuchen Sie, die gemeldeten Fehler zu beheben.

Basierend auf den Fehlern wird empfohlen, ein Support-Ticket zu erstellen, damit das Entwicklungsteam von Brand Portal Ihnen bei der Lösung der Probleme helfen kann.

## Brand Portal-IMS-Konfigurations-Token abgelaufen {#token-expired}

Wenn Ihre Brand Portal-Umgebung abrupt beendet wird, kann es sein, dass die IMS-Konfigurationen nicht ordnungsgemäß funktionieren. Das System zeigt eine fehlerhafte IMS-Konfiguration an und gibt in einer Fehlermeldung (ähnlich der folgenden) an, dass Ihr Zugriffs-Token abgelaufen ist.

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

Um dieses Problem zu beheben, empfiehlt Adobe, die IMS-Konfiguration manuell zu speichern und zu schließen und den Gesundheitsstatus erneut zu überprüfen. Wenn die Konfigurationen nicht funktionieren, löschen Sie die vorhandenen Konfigurationen und erstellen Sie eine neue.


## Konfigurieren von Replikationsagenten, um Verbindungsabbrüche wegen Zeitüberschreitung zu verhindern {#connection-timeout}

Normalerweise schlägt der Veröffentlichungsauftrag mit einem Zeitüberschreitungsfehler fehl, wenn die Replikationswarteschlange mehrere ausstehende Anforderungen enthält. Um das Problem zu beheben, konfigurieren Sie die Replikationsagenten so, dass keine Zeitüberschreitung erfolgt.

Gehen Sie wie folgt vor, um den Replikationsagenten zu konfigurieren:

1. Melden Sie sich bei der AEM Assets-Autorenistanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Bereitstellung]** > **[!UICONTROL Replikation]**.
1. Klicken Sie auf der Seite Replikation auf **[!UICONTROL `Agents on author`]**. Sie sehen die vier Replikationsagenten Ihres Brand Portal-Mandanten.
1. Klicken Sie auf die Replikationsagenten-URL und dann auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie in den Agenteneinstellungen auf die Registerkarte **[!UICONTROL Erweitert]**.
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Verbindung schließen]**.
1. Wiederholen Sie die Schritte 4 bis 7, um alle vier Replikationsagenten zu konfigurieren.
1. Starten Sie den Server neu.
