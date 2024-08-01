---
title: Häufig gestellte Fragen
description: Hier erhalten Sie Antworten auf häufig gestellte Fragen, die in Adobe Experience Manager Assets Brand Portal veröffentlicht wurden.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4c701781e7dc62b9d2b018fd13b1ae9616bbb840
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 24%

---

# Häufig gestellte Fragen {#frequently-asked-questions}

Die häufig gestellten Fragen zu Brand Portal betreffen die Fragen und Probleme von Endbenutzern, die bei der Arbeit mit der neuesten Version von Experience Manager Assets Brand Portal 6.4.6 oder früheren Versionen auftreten könnten.


## Häufig gestellte Fragen zu Brand Portal 6.4.6  {#faqs-bp646}

**Frage: Der vorhandene alte OAuth-Endpunkt (`https://legacy-oauth.cloud.adobe.io/login`) funktioniert nicht. Was könnte der Grund sein?**

**Antwort:** Die alte OAuth-Konfiguration wird nicht mehr unterstützt. Aktualisieren Sie die Experience Manager Assets-Autoreninstanzen auf das neueste Service Pack und konfigurieren Sie es über Adobe Developer Console. Weitere Informationen finden Sie unter [Konfigurieren von Experience Manager Assets mit Brand Portal](configure-aem-assets-with-brand-portal.md). Um die alte OAuth-Konfiguration jedoch bis zum Upgrade verwenden zu können, ändern Sie den alten OAuth-Endpunkt in `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Frage: Nach dem Upgrade auf Adobe Developer Console kann ich die Assets des Beitragsordners nicht von Brand Portal in Experience Manager Assets veröffentlichen. Meine Autoreninstanz befindet sich unter Experience Manager Assets 6.5.4. Was könnte der Grund sein?**

**Antwort:** Ja, es gibt ein bekanntes Problem beim Veröffentlichen der Assets des Beitragsordners über Adobe Developer Console in Experience Manager Assets 6.5.4.

Das Problem wurde in Experience Manager Assets 6.5.5. behoben. Sie können Ihre Experience Manager Assets-Instanz auf das neueste Service Pack aktualisieren und [Ihre Konfigurationen in Adobe Developer Console aktualisieren](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65).


**Frage: Der Inhalt des Beitragsordners wird nicht aus Brand Portal in Experience Manager Assets veröffentlicht. Was könnte der Grund sein?**

**Antwort:** Wenden Sie sich an Ihren Experience Manager Assets-Administrator, um die Konfigurationen zu überprüfen und sicherzustellen, dass Ihr Brand Portal-Mandant mit nur einer Experience Manager Assets-Autoreninstanz konfiguriert ist.

Dieses Problem tritt möglicherweise auf, wenn Sie einen Brand Portal-Mandanten in mehreren Experience Manager Assets-Autoreninstanzen konfiguriert haben. Beispielsweise konfiguriert der Administrator denselben Brand Portal-Mandanten auf der Experience Manager Assets-Autoreninstanz einer Staging- und Produktionsumgebung. In diesem Fall können die Asset-Veröffentlichungs-Trigger in Brand Portal, aber die Experience Manager Assets-Autoreninstanz kann das Asset nicht importieren, da der Replikationsagent das Anfrage-Token nicht erhält.


**Frage: Ich kann keine Assets aus Experience Manager Assets in Brand Portal veröffentlichen. Im Replikationsprotokoll wird angegeben, dass bei der Verbindung eine Zeitüberschreitung aufgetreten ist. Gibt es eine schnelle Lösung?**

**Antwort:** Normalerweise schlägt die Veröffentlichung mit einem Zeitüberschreitungsfehler fehl, wenn die Replikationswarteschlange mehrere ausstehende Anforderungen enthält. Um das Problem zu beheben, konfigurieren Sie die Replikationsagenten so, dass keine Zeitüberschreitung erfolgt.

Gehen Sie wie folgt vor, um den Replikationsagenten zu konfigurieren:

1. Melden Sie sich bei Ihrer Experience Manager Assets-Autoreninstanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Bereitstellung]** > **[!UICONTROL Replikation]**.
1. Klicken Sie auf der Seite Replikation auf **[!UICONTROL `Agents on author`]**. Sie sehen die vier Replikationsagenten für Ihren Brand Portal-Mandanten.
1. Klicken Sie auf die Replikationsagenten-URL, um die Agentendetails zu öffnen.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]** , um die Einstellungen des Replikationsagenten zu bearbeiten.
1. Klicken Sie in den Agenteneinstellungen auf die Registerkarte **[!UICONTROL Erweitert]** .
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Verbindung schließen]**.
1. Wiederholen Sie die Schritte 4 bis 7, um alle vier Replikationsagenten zu konfigurieren.
1. Starten Sie den Server neu und überprüfen Sie die Verbindung.


## Häufig gestellte Fragen zu Brand Portal 6.4.5  {#faqs-bp645}

**Frage: Was ist die wichtigste Änderung in Brand Portal 6.4.5?**

**Antwort:** Mit Experience Manager Assets Brand Portal 6.4.5 können Benutzer Inhalte hochladen und den Beitragsordner direkt aus Brand Portal wieder in Experience Manager Assets veröffentlichen, ohne Administratorrechte zu benötigen. Weitere Informationen finden Sie in [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).



**Frage: Habe ich den Zugriff auf vorhandene Assets, Funktionen oder Konfigurationen verloren, die ich erstellt habe?**

**Antwort:** Alle vorhandenen Funktionen und Konfigurationen bleiben intakt. Es gibt keine Auswirkungen auf Ihre Endbenutzer und Ihre Inhalte bleiben unverändert.



**Frage: Wann ziehe ich auf die neue Version von Brand Portal um?**

**Antwort:** Brand Portal 6.4.5 wurde im Oktober 2019 für die Produktion freigegeben. Die nächste Brand Portal-Version wird für März 2020 erwartet.
Für Updates und Versionsänderungen empfiehlt Adobe, die [Versionshinweise](brand-portal-release-notes.md) und [Neue Funktionen in Brand Portal](whats-new.md) zu verfolgen.



**Frage: Sind meine Benutzer betroffen?**

**Antwort:** Die Brand Portal-Version 6.4.5 ist ausschließlich in Brand Portal verfügbar, sodass keine Auswirkungen auf Ihre Endbenutzer auftreten.



**Frage: Ist von meiner Seite als Brand Portal-Benutzer eine Aktion erforderlich?**

**Antwort:** Brand Portal-Version 6.4.5 enthält eine neue Funktion namens &quot;Asset-Beschaffung&quot;. Der Administrator muss die Asset-Beschaffungsfunktion in Experience Manager Assets konfigurieren, um die Funktion für Brand Portal-Benutzer zu aktivieren. Weitere Informationen finden Sie unter [Aktivieren der Asset-Beschaffung](brand-portal-asset-sourcing.md).



**Frage: Wer kann einen Beitragsordner erstellen?**

**Antwort:** Jeder Experience Manager Assets-Benutzer, der zum Erstellen eines Ordners in Experience Manager Assets berechtigt ist, kann einen Ordner &quot;**Beitrag**&quot;erstellen. Erstellen Sie zum Erstellen eines Ordners vom Typ **Beitrag** einen Ordner vom Typ **Asset-Beitrag**.
Dieser Ordner ist für die aktiven Brand Portal-Benutzer freigegeben, die daraufhin Beiträge beisteuern können.



**Frage: Was enthält ein Beitragsordner?**

**Antwort:** **Beitragsordner** enthält zwei Unterordner **NEU** und **FREIGEGEBEN**. Zunächst ist der Ordner NEU leer, und der Ordner SHARED enthält den Referenzinhalt (wiederverwendbare Assets) für die Brand Portal-Benutzer.
Die Brand Portal-Benutzer greifen auf den **Beitragsordner** zu und laden Inhalte in den Ordner **NEU** hoch.



**Frage: Kann ich den Namen eines vorhandenen Beitragsordners ändern?**

**Antwort:** **Nein**, Sie können den Namen eines vorhandenen **Beitragsordners** nicht ändern.



**Frage: Was sind Asset-Anforderungen mit Beitrag vom Typ r.t?**

**Antwort:** Das Dokument **Kurz** im Ordner **Beitrag** und der Referenzinhalt im Ordner **SHARED** helfen Brand Portal-Benutzern, die Beitragsanforderungen und -erwartungen zu verstehen. Gemeinsam werden sie als Asset-Anforderungen bezeichnet.

**Frage: Kann ich Assets in einen beliebigen zulässigen Ordner hochladen?**

**Antwort:** Nicht alle zulässigen Ordner. Ein Brand Portal-Benutzer kann Inhalte nur in den Ordner **Beitrag** hochladen, den der Experience Manager Assets- oder Brand Portal-Administrator freigegeben hat.



**Frage: Wie erhalte ich Zugriff auf einen Beitragsordner?**

**Antwort:** Sie können nur dann auf einen Ordner **Beitrag** zugreifen, wenn dieser für Sie freigegeben wurde. Sie erhalten eine E-Mail-/Pulsbenachrichtigung, sobald ein Beitragsordner für Sie freigegeben wurde. Sie können über den in der E-Mail freigegebenen Link auf den Beitragsordner zugreifen. Alternativ können Sie sich bei Ihrer Brand Portal-Instanz anmelden und zum Glockensymbol für Benachrichtigungen navigieren, um auf den Beitragsordner zuzugreifen.

>[!NOTE]
>
>Wenn Sie kein Brand Portal-Benutzer sind, bitten Sie den Experience Manager Assets-Administrator, Ihren Benutzer in der Admin Console zu erstellen. Fügen Sie dann Ihr Profil zur Benutzerkonfigurationsdatei in der Brand Portal-Benutzerliste hinzu.


**Frage: Welches Format hat die CSV-Datei für den Benutzerimport?**

**Antwort:** Das Format entspricht dem, was Admin Console für den Massenimport von Benutzern unterstützt. E-Mail-Adresse, Vorname und Nachname sind obligatorisch.



**Frage: Wie wird die Liste der Benutzer (Brand Portal-Mitarbeiter) in der Dropdown-Liste &quot;Asset-Beitragsbenutzer&quot;gefüllt?**

**Antwort:** Die Benutzer in der Dropdown-Liste werden aus der Brand Portal-Benutzerkonfigurationsdatei (.csv) gefüllt, die in Experience Manager Assets hochgeladen wurde.



**Frage: Wo kann ich den Status von Import- und Veröffentlichungsaufträgen sehen?**

**Antwort:** In Experience Manager Assets können Sie den Status eines Imports auf der Auftragsseite **async** sehen. In Brand Portal können Sie den Status eines Veröffentlichungsauftrags unter **[!UICONTROL Tools > Asset-Beitragsstatus]** anzeigen.



**Frage: Wie häufig wird ein Importauftrag ausgeführt, der regelmäßig in Experience Manager ausgeführt wird?**

**Antwort:** In Experience Manager Assets wird die Abfrage alle fünf Minuten ausgeführt.



**Frage: Gibt es einen Schwellenwert dafür, wie oft ein Ordner von Brand Portal in Experience Manager Assets veröffentlicht werden kann?**

**Antwort:** Nein, alle Assets im Ordner **NEU** werden unabhängig davon, ob sie zuvor veröffentlicht wurden, in Experience Manager Assets veröffentlicht. Jedes Mal, wenn ein **Beitragsordner** aus Brand Portal in Experience Manager Assets veröffentlicht wird, ersetzt er den Inhalt des Ordners **NEU** .



**Frage: Wie werden neue Assets in einen Beitragsordner hochgeladen?**

**Antwort:** Weitere Informationen finden Sie in der ausführlichen Dokumentation zum [Hochladen von Assets in den Beitragsordner](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Frage: Ich kann keine Miniaturansichten oder Vorschauen für die Assets anzeigen, die in den Ordner NEU hochgeladen wurden.**

**Antwort:** Sie ist wie vorgesehen, da am Brand Portal-Ende kein Workflow ausgeführt wird.



**Frage: Was passiert, wenn ein Ordner von Experience Manager Assets in Brand Portal veröffentlicht wird, der sich im Fluss befindet?**

**Antwort:** In Experience Manager Assets werden Protokolle für jedes Mal verwaltet, wenn ein Ordner in Brand Portal veröffentlicht wird. Zum Zeitpunkt der Veröffentlichung werden alle Assets, die nicht in Brand Portal veröffentlicht werden, einer Replikationswarteschlange hinzugefügt. Assets, die nach dem Auslösen des Veröffentlichungsauftrags zum Ordner hinzugefügt wurden, werden nicht in Brand Portal veröffentlicht. Wenn ein Experience Manager Assets-Benutzer den Ordner erneut veröffentlicht, werden nur die Assets in Brand Portal veröffentlicht, die zuvor noch nicht veröffentlicht wurden (in der Replikationswarteschlange). Dieser Prozess gilt für alle Ordner, die aus Experience Manager Assets in Brand Portal veröffentlicht werden, und für den Ordner FREIGEGEBEN in einem Beitragsordner.

**Frage: An wen kann ich mich bei Fragen wenden?**

**Antwort:** Wenden Sie sich an Ihren Adobe-Kundenbetreuer oder an den Kundensupport.

>[!NOTE]
>
>Der Veröffentlichungszeitplan ist vorläufig und kann geändert werden. Wenden Sie sich an Ihren Adobe-Kundenbetreuer oder an den Kundensupport, um den aktualisierten Veröffentlichungszeitplan zu erhalten.


## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kundinnen und Kunden verfügbar. Wenden Sie sich an Ihren Adobe Account Manager, wenn Sie Kunde sind und Zugriff benötigen.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
