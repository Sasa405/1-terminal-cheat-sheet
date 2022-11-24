# 1-Terminal-cheat-sheet that is so funny! :joy:
**fb-009-Verzeichnis-Befehle**





Verzeichnis-Befehle


Das **Tilde-Symbol** (~) steht für Ihr Heimatverzeichnis. 
Wenn Sie user sind, dann steht die Tilde (~) für /home/user


**pwd**: Mit dem Befehl pwd können Sie feststellen, in welchem Verzeichnis Sie sich befinden (pwd steht für "print working directory").
**Beispiel**: "pwd" im Desktop-Verzeichnis zeigt "~/Desktop" an. Beachten Sie, dass das GNOME-Terminal diese Informationen auch in der Titelleiste seines Fensters anzeigt. Eine nützliche Gnemonik ist "present working directory".


ls: Mit dem Befehl ls können Sie sich die Dateien in Ihrem aktuellen Verzeichnis anzeigen lassen ("auflisten"). In Verbindung mit bestimmten Optionen können Sie die Größe der Dateien, das Erstellungsdatum und die Berechtigungen der Dateien anzeigen. Beispiel: "ls ~" zeigt Ihnen die Dateien an, die sich in Ihrem Heimatverzeichnis befinden.

cd: Mit dem cd-Befehl können Sie Verzeichnisse wechseln. Wenn Sie ein Terminal öffnen, befinden Sie sich in Ihrem Heimatverzeichnis. Um sich im Dateisystem zu bewegen, verwenden Sie cd. Beispiele:

Um in das Stammverzeichnis zu gelangen, verwenden Sie "cd /".

Um in Ihr Heimatverzeichnis zu wechseln, verwenden Sie "cd" oder "cd ~".

Um eine Verzeichnisebene höher zu navigieren, verwenden Sie "cd ..".

Um zum vorherigen Verzeichnis (oder zurück) zu navigieren, verwenden Sie "cd -".

Übersetzt mit www.DeepL.com/Translator (kostenlose Version)



Um durch mehrere Verzeichnisebenen auf einmal zu navigieren, geben Sie den vollständigen Verzeichnispfad an, zu dem Sie wechseln möchten. Verwenden Sie zum Beispiel "cd /var/www", um direkt zum Unterverzeichnis /www von /var/ zu gelangen. Ein anderes Beispiel: "cd ~/Desktop" führt Sie in das Unterverzeichnis Desktop in Ihrem Heimatverzeichnis.

cp: Der Befehl cp erstellt eine Kopie einer Datei für Sie. Beispiel: "cp file foo" erstellt eine exakte Kopie von "file" und gibt ihr den Namen "foo", aber die Datei "file" ist noch vorhanden. Wenn Sie ein Verzeichnis kopieren, müssen Sie "cp -r Verzeichnis foo" (rekursiv kopieren) verwenden. (Um zu verstehen, was "rekursiv" bedeutet, stellen Sie es sich so vor: Sie kopieren das Verzeichnis und alle seine Dateien und Unterverzeichnisse und alle deren Dateien und Unterverzeichnisse der Unterverzeichnisse und alle deren Dateien und so weiter, "rekursiv")

mv: Der Befehl mv verschiebt eine Datei an einen anderen Ort oder benennt eine Datei um. Beispiele sind folgende: "mv file foo" wird die Datei "file" in "foo" umbenennen. "mv foo ~/Desktop" verschiebt die Datei "foo" in Ihr Desktop-Verzeichnis, benennt sie aber nicht um. Sie müssen einen neuen Dateinamen angeben, um eine Datei umzubenennen.

Um Tipparbeit zu sparen, können Sie "~" anstelle des Home-Verzeichnisses angeben.
Beachten Sie, dass Sie bei der Verwendung von mv mit sudo die Abkürzung ~ verwenden können, da das Terminal die ~ zu Ihrem Heimatverzeichnis expandiert. Wenn Sie jedoch eine Root-Shell mit sudo -i oder sudo -s öffnen, verweist ~ auf das Home-Verzeichnis des Root-Kontos, nicht auf Ihr eigenes.

rm: Verwenden Sie diesen Befehl, um eine Datei in Ihrem Verzeichnis zu entfernen oder zu löschen.


Übersetzt mit www.DeepL.com/Translator (kostenlose Version)

rmdir: Mit dem Befehl rmdir wird ein leeres Verzeichnis gelöscht. Um ein Verzeichnis und seinen gesamten Inhalt rekursiv zu löschen, verwenden Sie stattdessen rm -r.

mkdir: Mit dem Befehl mkdir können Sie Verzeichnisse erstellen. Beispiel: "mkdir music" erstellt ein Verzeichnis namens "music".

Hier ist ein Beispiel dafür, wann es notwendig ist, einen Befehl mit administrativen Rechten auszuführen. Nehmen wir an, ein anderer Benutzer hat versehentlich eines Ihrer Dokumente aus dem Verzeichnis "Dokumente" in das Stammverzeichnis verschoben. Normalerweise würden Sie mv /mydoc.odt ~/Dokumente/mydoc.odt eingeben, um das Dokument zurück zu verschieben, aber standardmäßig dürfen Sie keine Dateien außerhalb Ihres Heimatverzeichnisses ändern. Um dies zu umgehen, müssen Sie sudo mv /mydoc.odt ~/Dokumente/mydoc.odt eingeben. Dadurch wird das Dokument erfolgreich an seinen korrekten Speicherort zurückgeschoben, vorausgesetzt, Sie haben Administratorrechte.

Übersetzt mit www.DeepL.com/Translator (kostenlose Version)


