---
title: Häufig gestellte Fragen
description: Hier erhalten Sie Antworten auf häufig gestellte Fragen, die in Adobe Experience Manager Assets Brand Portal veröffentlicht wurden.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 24%

---

# Häufig gestellte Fragen {#frequently-asked-questions}

Die häufig gestellten Fragen zu Brand Portal betreffen die Fragen und Probleme von Endbenutzern, auf die sie bei der Arbeit mit der neuesten Version von Experience Manager Assets Brand Portal 6.4.6 oder früheren Versionen stoßen können.


## Häufig gestellte Fragen zu Brand Portal 6.4.6  {#faqs-bp646}

**Frage: Der vorhandene alte OAuth-Endpunkt (`https://legacy-oauth.cloud.adobe.io/login`) funktioniert nicht. Was könnte der Grund sein?**

**Antwort:** alte OAuth-Konfiguration wird nicht mehr unterstützt. Aktualisieren Sie die Experience Manager Assets-Autoreninstanzen auf das neueste Service Pack und konfigurieren Sie es über Adobe Developer Console. Weitere Informationen finden Sie unter [Konfigurieren von Experience Manager Assets mit Brand Portal](configure-aem-assets-with-brand-portal.md). Um die alte OAuth-Konfiguration jedoch bis zum Upgrade verwenden zu können, ändern Sie den alten OAuth-Endpunkt in `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Frage: Ich kann die Assets des Beitragsordners nach der Aktualisierung auf Adobe Developer Console nicht von Brand Portal in Experience Manager Assets veröffentlichen. Meine Autoreninstanz befindet sich unter Experience Manager Assets 6.5.4. Was könnte der Grund sein?**

**Antwort:** Ja, es gibt ein bekanntes Problem bei der Veröffentlichung von Assets des Beitragsordners in Experience Manager Assets 6.5.4 über die Adobe Developer Console.

Das Problem wurde in Experience Manager Assets 6.5.5. behoben. Sie können Ihre Experience Manager Assets-Instanz auf das neueste Service Pack aktualisieren und [Ihre Konfigurationen in Adobe Developer Console aktualisieren](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65).


**Frage: Ich sehe den Inhalt des Beitragsordners, der in Brand Portal in Experience Manager Assets veröffentlicht wurde, nicht. Was könnte der Grund sein?**

**Antwort:** Wenden Sie sich an Ihren Experience Manager Assets-Administrator, um die Konfigurationen zu überprüfen, und stellen Sie sicher, dass für Ihren Brand Portal-Mandanten nur eine Experience Manager Assets-Autoreninstanz konfiguriert ist.

Dieses Problem tritt möglicherweise auf, wenn Sie einen Brand Portal-Mandanten in mehreren Experience Manager Assets-Autoreninstanzen konfiguriert haben. Beispielsweise konfiguriert der Administrator denselben Brand Portal-Mandanten in der Experience Manager Assets-Autoreninstanz einer Staging- und Produktionsumgebung. In diesem Fall erfolgt der Trigger der Asset-Veröffentlichung in Brand Portal, aber die Experience Manager Assets-Autoreninstanz kann das Asset nicht importieren, da der Replikationsagent das Anfrage-Token nicht erhält.


**Frage: Ich kann keine Assets von Experience Manager Assets in Brand Portal veröffentlichen. Im Replikationsprotokoll wird angegeben, dass bei der Verbindung eine Zeitüberschreitung aufgetreten ist. Gibt es eine schnelle Lösung?**

**Antwort:** In der Regel schlägt die Veröffentlichung mit einem Zeitüberschreitungsfehler fehl, wenn sich mehrere ausstehende Anfragen in der Replikationswarteschlange befinden. Um das Problem zu beheben, konfigurieren Sie die Replikationsagenten so, dass keine Zeitüberschreitung erfolgt.

Gehen Sie wie folgt vor, um den Replikationsagenten zu konfigurieren:

1. Melden Sie sich bei Ihrer Experience Manager Assets-Autoreninstanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Bereitstellung]** > **[!UICONTROL Replikation]**.
1. Klicken Sie auf der Seite Replikation auf **[!UICONTROL `Agents on author`]**. Sie sehen die vier Replikationsagenten für Ihren Brand Portal-Mandanten.
1. Klicken Sie auf die Replikationsagenten-URL, um die Agentendetails zu öffnen.
1. Klicken Sie **[!UICONTROL Bearbeiten]**, um die Einstellungen für den Replikationsagenten zu bearbeiten.
1. Klicken Sie in den Agenteneinstellungen auf die Registerkarte **[!UICONTROL Erweitert]**.
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Verbindung schließen]**.
1. Wiederholen Sie die Schritte 4 bis 7, um alle vier Replikationsagenten zu konfigurieren.
1. Starten Sie den Server neu und überprüfen Sie die Verbindung.


## Häufig gestellte Fragen zu Brand Portal 6.4.5  {#faqs-bp645}

**Frage: Was ist die größte Änderung in Brand Portal Version 6.4.5?**

**Antwort:** Mit Experience Manager Assets Brand Portal 6.4.5 können Benutzer Inhalte hochladen und den Beitragsordner direkt aus Brand Portal wieder in Experience Manager Assets veröffentlichen, ohne dass Administratorrechte erforderlich sind. Weitere Informationen finden Sie in [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).



**Frage: Habe ich den Zugriff auf vorhandene Assets, Funktionen oder Konfigurationen verloren, die ich erstellt habe?**

**Antwort:** Alle vorhandenen Funktionen und Konfigurationen bleiben intakt. Es gibt keine Auswirkungen auf Ihre Endbenutzer und Ihre Inhalte bleiben unverändert.



**Frage: Wann wechsle ich zur neuen Version von Brand Portal?**

**Antwort:** Brand Portal 6.4.5 wurde im Oktober 2019 veröffentlicht. Und die nächste Brand Portal-Version wird für März 2020 erwartet.
Für Updates und Versionsänderungen empfiehlt Adobe, die [Versionshinweise](brand-portal-release-notes.md) und &quot;[ in Brand Portal&quot; ](whats-new.md).



**Frage: Sind meine Benutzer betroffen?**

**Antwort:** Die Brand Portal-Version 6.4.5 befindet sich ausschließlich in Brand Portal, sodass sie keine Auswirkungen auf Ihre Endbenutzenden hat.



**Frage: Muss ich als Brand Portal-Anwender etwas unternehmen?**

**Antwort:** Version Brand Portal 6.4.5 enthält eine neue Funktion namens Asset-Beschaffung. Der Administrator muss die Asset-Beschaffungsfunktion in Experience Manager Assets konfigurieren, um die Funktion für die Brand Portal-Benutzer zu aktivieren. Weitere Informationen finden Sie unter [Aktivieren der Asset-Beschaffung](brand-portal-asset-sourcing.md).



**Frage: Wer kann einen Beitragsordner erstellen?**

**Antwort:** Jeder Experience Manager Assets-Benutzer, der berechtigt ist, einen Ordner in Experience Manager Assets zu erstellen, kann einen **Beitragsordner** erstellen. Um einen Ordner **Beitrag** zu erstellen, erstellen Sie einen Ordner des Typs **Asset-Beitrag**.
Dieser Ordner ist für die aktiven Brand Portal-Benutzer freigegeben, die daraufhin Beiträge beisteuern können.



**Frage: Was enthält ein Beitragsordner?**

**Antwort:** **Beitrag** Ordner enthält zwei Unterordner **NEU** und **FREIGEGEBEN**. Zunächst ist der Ordner NEU leer, und der Ordner SHARED enthält den Referenzinhalt (wiederverwendbare Assets) für die Brand Portal-Benutzer.
Die Brand Portal-Benutzer greifen auf den **Beitragsordner** zu und laden Inhalte in den Ordner **NEU** hoch.



**Frage: Kann ich den Namen eines vorhandenen Beitragsordners ändern?**

**Antwort:** **Nein** Sie können den Namen eines vorhandenen Ordners **Beitrag** nicht ändern.



**Frage: Was sind die Asset-Anforderungen in Bezug auf den Beitrag?**

**Antwort:** Das **Brief**-Dokument im **Contribution**-Ordner und der Referenzinhalt im **SHARED**-Ordner helfen Brand Portal-Benutzern, die Beitragsanforderungen und -erwartungen zu verstehen. Zusammen werden sie als Asset-Anforderungen bezeichnet.

**Frage: Kann ich Assets in einen beliebigen zulässigen Ordner hochladen?**

**Antwort:** nicht alle zulässigen Ordner. Ein Brand Portal-Benutzer kann Inhalte nur in den Ordner &quot;**&quot; hochladen** den der Experience Manager Assets- oder Brand Portal-Administrator freigibt.



**Frage: Wie erhalte ich Zugriff auf einen Beitragsordner?**

**Antwort:** Sie können nur auf einen **Beitragsordner** zugreifen, wenn dieser für Sie freigegeben wurde. Sie erhalten eine E-Mail-/Push-Benachrichtigung, sobald ein Beitragsordner für Sie freigegeben wird. Sie können über den in der E-Mail freigegebenen Link auf den Beitragsordner zugreifen. Alternativ können Sie sich bei Ihrer Brand Portal-Instanz anmelden und zum Glockensymbol navigieren, um Benachrichtigungen über den Zugriff auf den Beitragsordner zu erhalten.

>[!NOTE]
>
>Wenn Sie kein Brand Portal-Benutzer sind, bitten Sie den Experience Manager Assets-Administrator, Ihr Benutzerkonto in der Admin Console zu erstellen. Fügen Sie dann Ihr Profil zur Benutzerkonfigurationsdatei in der Brand Portal-Benutzerliste hinzu.


**Frage: Was ist das Format der CSV-Datei für den Benutzerimport?**

**Antwort:** Das Format entspricht dem, was Admin Console für den Massenimport von Benutzern unterstützt. E-Mail-Adresse, Vorname und Nachname sind obligatorisch.



**Frage: Worauf wird die Liste der Benutzer (Brand Portal-Mitwirkende) in der Dropdown-Liste Asset-Beitrag des Benutzers gefüllt?**

**Antwort:** Die Benutzer in der Dropdown-Liste werden aus der in Experience Manager Assets hochgeladenen Datei für die Brand Portal-Benutzerkonfiguration (.csv) gefüllt.



**Frage: Wo kann ich den Status von Import- und Veröffentlichungsaufträgen sehen?**

**Antwort:** In Experience Manager Assets können Sie den Status eines Imports auf der Auftragsseite **asynchron** sehen. In Brand Portal können Sie den Status eines Veröffentlichungsauftrags unter **[!UICONTROL Tools > Asset-Beitragsstatus]** anzeigen.



**Frage: Wie häufig wird ein Importauftrag ausgeführt, der regelmäßig im Experience Manager ausgeführt wird?**

**Antwort:** In Experience Manager Assets wird die Abfrage alle fünf Minuten ausgeführt.



**Frage: Gibt es einen Schwellenwert dafür, wie oft ein Ordner von Brand Portal in Experience Manager Assets veröffentlicht werden kann?**

**Antwort:** Nein, alle Assets im Ordner **NEU** werden unabhängig davon, ob sie zuvor veröffentlicht wurden, in Experience Manager Assets veröffentlicht. Jedes Mal **wenn ein** Beitragsordner“ von Brand Portal in Experience Manager Assets veröffentlicht wird, ersetzt er den Inhalt des Ordners **NEU**.



**Frage: Wie können neue Assets in einen Beitragsordner hochgeladen werden?**

**Antwort:** Informationen finden Sie in der ausführlichen Dokumentation [Hochladen von Assets in den Beitragsordner](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Frage: Ich kann keine Miniaturansichten oder Vorschauen für die Assets sehen, die in den Ordner „NEU“ hochgeladen wurden.**

**Antwort:** Es ist wie vorgesehen, da es am Ende von Brand Portal keine Ausführung von Workflows gibt.



**Frage: Was passiert, wenn ein Ordner von Experience Manager Assets an Brand Portal veröffentlicht wird, das sich im Fluss befindet?**

**Antwort:** In Experience Manager Assets werden Protokolle für jedes Mal aufgezeichnet, wenn ein Ordner in Brand Portal veröffentlicht wird. Zum Zeitpunkt der Veröffentlichung werden alle Assets, die nicht in Brand Portal veröffentlicht wurden, zu einer Replikations-Warteschlange hinzugefügt. Assets, die nach dem Auslösen des Veröffentlichungsauftrags zum Ordner hinzugefügt wurden, werden nicht in Brand Portal veröffentlicht. Wenn ein Experience Manager Assets-Benutzer den Ordner erneut veröffentlicht, werden nur die zuvor nicht veröffentlichten (und in der Replikationswarteschlange vorhandenen) Assets in Brand Portal veröffentlicht. Dieser Prozess gilt für alle Ordner, die aus Experience Manager Assets in Brand Portal veröffentlicht wurden, sowie für den Ordner FREIGEGEBEN in einem Beitragsordner.

**Frage: An wen wende ich mich bei Fragen?**

**Antwort:** Kontaktieren Sie Ihren Adobe-Kundenbetreuer oder den Support.

>[!NOTE]
>
>Der Veröffentlichungszeitplan ist vorläufig und kann sich ändern. Wenden Sie sich an Ihren Adobe-Kundenbetreuer oder den Support, um den aktualisierten Versionsplan zu erhalten.


## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kundinnen und Kunden verfügbar. Wenn Sie -Kunde sind und Zugriff benötigen, wenden Sie sich an Ihren Adobe Account Manager.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
