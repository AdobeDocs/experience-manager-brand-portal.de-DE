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
workflow-type: ht
source-wordcount: '1500'
ht-degree: 100%

---

# Häufig gestellte Fragen {#frequently-asked-questions}

Die häufig gestellten Fragen zu Brand Portal betreffen die Fragen und Probleme von Endbenutzenden, die bei der Arbeit mit der neuesten Version 6.4.6 von Experience Manager Assets Brand Portal oder mit früheren Versionen auftreten können.


## Häufig gestellte Fragen zu Brand Portal 6.4.6 {#faqs-bp646}

**Frage: Der vorhandene alte OAuth-Endpunkt (`https://legacy-oauth.cloud.adobe.io/login`) funktioniert nicht. Was könnte der Grund sein?**

**Antwort:** Die alte OAuth-Konfiguration wird nicht mehr unterstützt. Sie müssen die Autoreninstanzen von Experience Manager Assets auf das neueste Service Pack aktualisieren und es mithilfe der Adobe Developer Console konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren von Experience Manager Assets mit Brand Portal](configure-aem-assets-with-brand-portal.md). Um die alte OAuth-Konfiguration jedoch bis zum Upgrade verwenden zu können, ändern Sie den alten OAuth-Endpunkt in `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Frage: Nach der Aktualisierung auf Adobe Developer Console kann ich die Assets des Beitragsordners von Brand Portal nicht in Experience Manager Assets veröffentlichen. Meine Autoreninstanz befindet sich unter Experience Manager Assets 6.5.4. Was könnte der Grund sein?**

**Antwort:** Ja, es gibt ein bekanntes Problem bei der Veröffentlichung von Assets des Beitragsordners in Experience Manager Assets 6.5.4 über die Adobe Developer Console.

Das Problem wurde in Experience Manager Assets 6.5.5. behoben. Sie können Ihre Experience Manager Assets-Instanz auf das neueste Service Pack aktualisieren und [Ihre Konfigurationen in Adobe Developer Console aktualisieren](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65).


**Frage: Ich sehe den Inhalt des Beitragsordners, der in Brand Portal veröffentlicht wurde, nicht in Experience Manager Assets. Was könnte der Grund sein?**

**Antwort:** Wenden Sie sich an Ihre Experience Manager Assets-Admins, um die Konfigurationen überprüfen zu lassen, und stellen Sie sicher, dass für den Brand Portal-Mandanten nur eine einzige Autoreninstanz konfiguriert ist.

Dieses Problem tritt möglicherweise auf, wenn Sie einen Brand Portal-Mandanten in mehreren Experience Manager Assets-Autoreninstanzen konfiguriert haben. Wenn z. B. die Admins denselben Brand Portal-Mandanten in der Experience Manager Assets-Autoreninstanz der Staging- und Proudktionsumgebung konfigurieren, wird die Asset-Veröffentlichung in Brand Portal zwar ausgelöst, die Experience Manager Assets-Autoreninstanz kann das Asset jedoch nicht importieren, da der Replikationsagent das Anfrage-Token nicht erhält.


**Frage: Ich kann keine Assets aus Experience Manager Assets in Brand Portal veröffentlichen. Im Replikationsprotokoll wird angegeben, dass bei der Verbindung eine Zeitüberschreitung aufgetreten ist. Gibt es eine schnelle Lösung?**

**Antwort:** Normalerweise schlägt die Veröffentlichung mit einem Zeitüberschreitungsfehler fehl, wenn die Replikationswarteschlange mehrere ausstehende Anfragen enthält. Um das Problem zu beheben, konfigurieren Sie die Replikationsagenten so, dass keine Zeitüberschreitung erfolgt.

Gehen Sie wie folgt vor, um den Replikationsagenten zu konfigurieren:

1. Melden Sie sich bei Ihrer Experience Manager Assets-Autoreninstanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Bereitstellung]** > **[!UICONTROL Replikation]**.
1. Klicken Sie auf der Seite „Replikation“ auf **[!UICONTROL `Agents on author`]**. Sie sehen die vier Replikationsagenten für Ihren Brand Portal-Mandanten.
1. Klicken Sie auf die Replikationsagenten-URL, um die Agentendetails zu öffnen.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**, um die Einstellungen des Replikationsagenten zu bearbeiten.
1. Klicken Sie in den Agenteneinstellungen auf die Registerkarte **[!UICONTROL Erweitert]**.
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Verbindung schließen]**.
1. Wiederholen Sie die Schritte 4 bis 7, um alle vier Replikationsagenten zu konfigurieren.
1. Starten Sie den Server neu und überprüfen Sie die Verbindung.


## Häufig gestellte Fragen zu Brand Portal 6.4.5  {#faqs-bp645}

**Frage: Was ist die wichtigste Änderung in Version 6.4.5 von Brand Portal?**

**Antwort:** Mit Experience Manager Assets Brand Portal 6.4.5 können Benutzende Inhalte hochladen und den Beitragsordner direkt aus Brand Portal wieder in Experience Manager Assets veröffentlichen, ohne dass Administratorrechte erforderlich sind. Weitere Informationen finden Sie unter [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).



**Frage: Verliere ich den Zugriff auf vorhandene Assets, Funktionen oder Konfigurationen, die ich erstellt habe?**

**Antwort:** Alle bestehenden Funktionen und Konfigurationen stehen weiterhin zur Verfügung. Es gibt keine Auswirkungen auf Ihre Endbenutzenden und Ihre Inhalte bleiben unverändert.



**Frage: Wann findet der Wechsel zur neuen Brand Portal-Version statt?**

**Antwort:** Brand Portal 6.4.5 wurde im Oktober 2019 für die Produktion freigegeben. Die nächste Brand Portal-Version wird voraussichtlich im März 2020 veröffentlicht.
Bezüglich Updates und Versionsänderungen wird empfohlen, die [Versionshinweise](brand-portal-release-notes.md) und [Neuigkeiten in Brand Portal](whats-new.md) zu verfolgen.



**Frage: Sind meine Benutzenden betroffen?**

**Antwort:** Die Brand Portal-Version 6.4.5 ist ausschließlich innerhalb von Brand Portal verfügbar, sodass keine Auswirkungen auf Ihre Endbenutzenden auftreten.



**Frage: Muss ich als Benutzerin oder Benutzer von Brand Portal irgendwelche Aufgaben durchführen?**

**Antwort:** Brand Portal-Version 6.4.5 enthält eine neue Funktion namens „Asset-Beschaffung“. Die Admins müssen die Asset-Beschaffung in Experience Manager Assets konfigurieren, um diese Funktion für die Brand Portal-Benutzenden zu aktivieren. Weitere Informationen finden Sie unter [Aktivieren der Asset-Beschaffung](brand-portal-asset-sourcing.md).



**Frage: Wer kann einen Beitragsordner erstellen?**

**Antwort:** Alle Experience Manager Assets-Benutzenden, die berechtigt sind, einen neuen Ordner in Experience Manager Assets zu erstellen, können einen **Beitragsordner** erstellen. Erstellen Sie zum Erstellen eines **Beitragsordners** einen neuen Ordner des Typs **Asset-Beiträge**.
Dieser Ordner ist für die aktiven Brand Portal-Benutzenden freigegeben, die Beiträge beisteuern können.



**Frage: Was enthält ein Beitragsordner?**

**Antwort:** Ein **Beitragsordner** enthält zwei Unterordner **NEU** und **FREIGEGEBEN**. Zunächst ist der Ordner NEU leer, und der Ordner SHARED enthält den Referenzinhalt (wiederverwendbare Assets) für die Brand Portal-Benutzer.
Die Brand Portal-Benutzer greifen auf den **Beitragsordner** zu und laden Inhalte in den Ordner **NEU** hoch.



**Frage: Kann ich den Namen eines bestehenden Beitragsordners ändern?**

**Antwort:** **Nein**, Sie können den Namen eines bestehenden **Beitragsordners** nicht ändern.



**Frage: Wie hoch sind die Anforderungen an Asset-Beiträge?**

**Antwort:** Mit dem **Übersichtsdokument** im **Beitragsordner** und dem Referenzinhalt im Ordner **FREIGEGEBEN** können Brand Portal-Benutzende sich über die Beitragsanforderungen und -erwartungen informieren. Diese werden zusammen als Asset-Anforderungen bezeichnet.

**Frage: Kann ich Assets in einen beliebigen zulässigen Ordner hochladen?**

**Antwort:** Nicht in alle zulässigen Ordner. Brand Portal-Benutzende können Inhalte nur in den **Beitragsordner** hochladen, der von Experience Manager Assets- oder Brand Portal-Admins freigegeben wird.



**Frage: Wie erhalte ich Zugriff auf einen Beitragsordner?**

**Antwort:** Sie können nur dann auf einen **Beitragsordner** zugreifen, wenn dieser für Sie freigegeben wurde. Sie erhalten eine E-Mail-/Pulse-Benachrichtigung, sobald ein Beitragsordner für Sie freigegeben wurde. Sie können über den in der E-Mail freigegebenen Link auf den Beitragsordner zugreifen. Alternativ können Sie sich bei Ihrer Brand Portal-Instanz anmelden und zum Glockensymbol für Benachrichtigungen navigieren, um Zugriff auf den Beitragsordner zu erhalten.

>[!NOTE]
>
>Wenn Sie nicht zu den Brand Portal-Benutzenden gehören, bitten Sie die Experience Manager Assets-Admins, Ihnen ein Benutzerkonto in der Admin Console zu erstellen. Fügen Sie dann Ihr Profil zur Benutzerkonfigurationsdatei in der Brand Portal-Benutzerliste hinzu.


**Frage: Welches Format hat die CSV-Datei für den Benutzerimport?**

**Antwort:** Das Format entspricht dem, was Admin Console für den Massenimport von Benutzenden unterstützt. E-Mail-Adresse, Vorname und Nachname sind obligatorisch.



**Frage: Wie wird die Liste der Benutzenden (Brand Portal-Beitragende) in der Dropdown-Liste „Asset-Beitrag-Benutzer“ befüllt?**

**Antwort:** Die Benutzenden in der Dropdown-Liste werden aus der in Experience Manager Assets hochgeladenen Datei für die Brand Portal-Benutzerkonfiguration (.CSV) befüllt.



**Frage: Wo kann ich den Status von Import- und Veröffentlichungsaufträgen sehen?**

**Antwort:** In Experience Manager Assets können Sie den Status eines Imports auf einer **asynchronen** Auftragsseite sehen. In Brand Portal können Sie den Status eines Veröffentlichungsauftrags unter **[!UICONTROL Tools > Asset-Beitragsstatus]** anzeigen.



**Frage: Wie häufig wird ein Importauftrag ausgeführt, der regelmäßig in Experience Manager Assets ausgeführt wird?**

**Antwort:** In Experience Manager Assets wird die Abfrage alle 5 Minuten ausgeführt.



**Frage: Gibt es einen Schwellenwert dafür, wie oft ein Ordner von Brand Portal in Experience Manager Assets veröffentlicht werden kann?**

**Antwort:** Nein, alle Assets im Ordner **NEU** werden unabhängig davon, ob sie jemals zuvor veröffentlicht wurden, in Experience Manager Assets veröffentlicht. Jedes Mal, wenn ein **Beitragsordner** von Brand Portal in Experience Manager Assets veröffentlicht wird, überschreibt er den Inhalt des Ordners **NEU**.



**Frage: Wie werden neue Assets in einen Beitragsordner hochgeladen?**

**Antwort:** Lesen Sie die detaillierte Dokumentation zum [Hochladen von Assets in den Beitragsordner](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Frage: Ich kann keine Miniaturansichten oder Vorschauen für die Assets sehen, die in den Ordner „NEU“ hochgeladen wurden.**

**Antwort:** Das ist normal, da aufseiten von Brand Portal kein Workflow ausgeführt wird.



**Frage: Was passiert, wenn ein Ordner von Experience Manager Assets an Brand Portal veröffentlicht wird, der sich im Fluss befindet?**

**Antwort:** In Experience Manager Assets werden Protokolle für jedes Mal aufgezeichnet, wenn ein Ordner in Brand Portal veröffentlicht wird. Zum Zeitpunkt der Veröffentlichung werden alle Assets, die nicht in Brand Portal veröffentlicht werden, in eine Replikationswarteschlange gestellt. Assets, die erst nach dem Auslösen des Veröffentlichungsauftrags zum Ordner hinzugefügt wurden, werden nicht in Brand Portal veröffentlicht. Wenn Experience Manager Assets-Benutzende den Ordner erneut veröffentlichen, werden nur die zuvor noch nicht veröffentlichten (und in der Replikationswarteschlange vorhandenen) Assets in Brand Portal veröffentlicht. Dieser Prozess gilt für alle Ordner, die von Experience Manager Assets in Brand Portal veröffentlicht werden, und für den Ordner FREIGEGEBEN in einem Beitragsordner.

**Frage: An wen kann ich mich bei Fragen wenden?**

**Antwort:** Kontaktieren Sie die Adobe-Kundenbetreuung oder den Kunden-Support.

>[!NOTE]
>
>Der Veröffentlichungszeitplan ist vorläufig und kann sich ändern. Wenden Sie sich an die Adobe-Kundenbetreuung oder den Kunden-Support, um den aktualisierten Veröffentlichungszeitplan zu erhalten.


## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kundinnen und Kunden verfügbar. Wenn Sie eine Kundin oder ein Kunde sind und Zugriff benötigen, wenden Sie sich an die Adobe-Kundenbetreuung.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
