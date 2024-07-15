# Ersteinrichtung von element.io
Matrix ist ein Kommunikationsprotokoll, das ähnlich wie E-Mail, dezentral aufgebaut ist. Das heißt, es gibt nicht eine zentrale Instanz, über die sämtlicher Datenverkehr abgewickelt wird, sondern mehrere sogenannte *Heim-Server*, bei denen man sich analog zu E-Mail einen Account einrichten kann und eine Adresse erhält in der Form @benutzername:server. Die Kommunikation ist je nach Konfiguration des Heim-Servers auch serverübergreifend möglich. Zur Dezentralität gehört auch, dass es nicht nur den **einen** Client zur Kommunikation gibt, wie z.B. die Apps für WhatsApp, Telegram, Signal und Co., sondern dass es auch hier mehrere freie Alternativen mit unterschiedlichem Funktionsumfang gibt, die beliebig gewählt werden sollen.
Die für unsere Zwecke geeignetste App heißt *element* und wird von matrix.org, den Entwicklern des Protokolls maßgeblich mitentwickelt.

1. Auf [https://element.io/download](https://element.io/download) entweder die Browser-App starten - der direkte Link hierzu lautet: [https://app.element.io](https://app.element.io/#/login) - oder die App für Dein Betriebssystem herunterladen. Das gleiche funktioniert im Falle von Mobilgeräten natürlich auch direkt aus dem App Store/Play Store heraus.
2. Danach zum Einloggen die Adresse des Heim-Servers *reservision.world* durch Klick auf **Bearbeiten** einstellen: 
![Screenshot 2024-07-15 125350](https://github.com/user-attachments/assets/c6d2913d-c589-4743-bd6b-e230419bfea3)
3. Nun lässt sich der Login mit der Google-Workspace-Adresse (@reservision.world) durchführen und die Element-App stellt sich kurz vor. Du bist automatisch Mitglied des Raumes "Allgemein".
4. Zunächst sollten die Schlüssel für die Ende-zu-Ende-Verschlüsselung (E2E) festgelegt werden. Hierzu klickst du auf dein Profilbild und danach auf **Sicherheit**, bzw **Sicherheit und Privatsphäre** in der Mobile-App.
![image](https://github.com/user-attachments/assets/6a7399bc-f847-41e7-8a28-bad8eba251ef)

Danach klickst du unter dem Abschnitt "Verschlüsselte Sicherung" auf den Button **Einrichten**:
![image](https://github.com/user-attachments/assets/4da22452-dd89-47f8-94fe-3c4b1bc3a959)

Nun besteht die Möglichkeit, entweder einen Schlüssel erzeugen zu lassen, den man am besten in einem Passwortmanager speichert, oder eine eigene Passphrase einzugeben (die man idealerweise nur selber kennt 🙂). Soll *element* ausschließlich im Browser verwendet werden, empfiehlt sich die eigene Passphrase, da diese nach jedem Logout wieder eingegeben werden muss. Der autogenerierte Schlüssel ist hierfür zu kryptisch. Wenn du die Desktop-App und evtl. noch eine Mobile-App nutzen möchtest, muss jedoch in der Regel kein Schlüssel eingegeben werden und es kann der automatisch generierte Schlüssel gewählt werden.
> [!CAUTION]
> **WICHTIG!!** Falls der Schlüssel verloren geht, verlierst du Zugriff auf alle vergangenen Nachrichten! Der Account kann natürlich weiterhin genutzt werden, allerdings werden nur zukünftige Nachrichten angezeigt und Nachrichten aus Räumen, die keine Ende-zu-Ende-Verschlüsselung nutzen. Es gibt absolut keine Möglichkeit, den Schlüssel irgendwie wiederherzustellen, falls er verlorengeht!

Kopiere den automatisch generierten Schlüssel in einen Passwortmanager, oder speichere ihn an einem sicheren Ort.


# Erneute Anmeldung im Browser oder Anmeldung auf einem neuen Gerät

- Loggst du dich aus der Browser-App aus und später wieder ein, wird dieser Screen angezeigt. Der gleiche Screen erscheint, wenn du versuchst, dich von einem neuen Gerät/neuen Browser einzuloggen.

![image](https://github.com/user-attachments/assets/86eb3823-23f4-4e4f-95fc-ed66fbd00997)

Hier muss, wie erwähnt, nun der vorher erzeugte oder eigens gewählte Schlüssel eingegeben werden, oder die Verifizierung mit einem anderen Gerät durchgeführt werden, falls es ein anderes Gerät mit aktiver Sitzung gibt. Wählst du die Geräteverifizierung, präsentiert sich folgender Screen im Browser oder in der Desktop-App:
![image](https://github.com/user-attachments/assets/51ed8f8e-8868-4e36-9370-2adeac75a230)

Der QR-Code lässt sich nun aus der element-App heraus von einem Handy oder Tablet scannen oder alternativ lässt sich die Verifizierung auch durch den Abgleich von Emojis durchführen.

---

Ist das neue Gerät ein Mobilgerät, erscheint am oberen Bildschirmrand diese Leiste:

![image](https://github.com/user-attachments/assets/0642574c-5b8a-4b04-80ad-3ca6a5954a7b)

Nach Klick auf die Leiste sieht der Bildschirm wie folgt aus. Zusätzlich musst du auf Anweisungen in der anderen Sitzung achten.

![image](https://github.com/user-attachments/assets/ffeec66e-d2fc-46a2-bb2f-a883b6cb39ca)

Idealerweise bist du noch auf einem anderen Gerät eingeloggt und kannst dieses zur Verifizierung nutzen. Wähle ansonsten **Nutze eine Wiederherstellungsmethode** um den Schlüssel/die Passphrase aus der Ersteinrichtung einzugeben. Wird **Überspringen** gewählt, bleiben E2E-verschlüsselte Nachrichten solange ausgeblendet, bis die Sitzung später verifiziert wird.
> [!WARNING]
> Beim Klick auf **Alle Wiederherstellungoptionen vergessen oder verloren? Alles zurücksetzen** geht der Zugriff auf vergangene Nachrichten unwiederbringlich verloren!

Wird die Geräteverifizierung gewählt, ändert sich der Screen wie folgt und erscheint damit ähnlich der Desktop-Optionen aus dem letzten Abschnitt:

![image](https://github.com/user-attachments/assets/96fa3826-c039-439b-a034-aa59d99b842a)

Bei Wahl von **Mit diesem Gerät scannen** wird in der anderen Sitzung ein QR-Code zum scannen angezeigt. Wählst du stattdessen **Kann nicht einlesen** ändert sich der Screen folgendermaßen und die gezeigten Emojis müssen mit den zeitgleich eingeblendeten auf dem anderen Gerät abgeglichen werden:

![image](https://github.com/user-attachments/assets/3fac3756-43cd-4372-bb7e-91c53e4471f3)

Hat alles geklappt, erscheint ein grünes Wappen, das möglicherweise noch angeklickt werden muss. Danach bist du auf beiden Geräten eingeloggt und kannst dich auch auf einem der Geräte bedenkenlos ausloggen, falls gewünscht.
