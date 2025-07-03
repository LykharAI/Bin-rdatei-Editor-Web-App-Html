# Binärdatei-Editor-Web-App-Html

Der Binärdatei-Editor ist eine in sich geschlossene Single-Page-Application (SPA), die als Werkzeug für Entwickler, IT-Spezialisten und technisch Interessierte dient. Sie ermöglicht die schnelle Inspektion und editieren von Binärdateien direkt im Browser. 

Alle Dateioperationen finden lokal im Speicher des Browsers statt, was maximale Geschwindigkeit und Datenschutz gewährleistet.
Features
 * Lokales Laden: Öffnen Sie .bin-Dateien oder beliebige andere Dateien von Ihrem lokalen System.
 * Interaktive Hex/ASCII-Ansicht: Die Daten werden übersichtlich mit Adress-Offset, Hexadezimalwerten und der entsprechenden ASCII-Darstellung angezeigt.
 * Direktes Bearbeiten: Klicken Sie auf einen beliebigen Hex- oder ASCII-Wert, um ihn zu ändern. Die korrespondierende Darstellung wird automatisch aktualisiert.
 * Änderungen speichern: Laden Sie die modifizierten Daten als neue Datei auf Ihren Computer herunter.
 * 100% Client-Side: Die Anwendung ist vollständig in Vanilla JavaScript, HTML5 und Tailwind CSS geschrieben. Es findet keine Server-Kommunikation statt.
 * Responsives Design: Die Benutzeroberfläche passt sich an verschiedene Bildschirmgrößen an.
Erste Schritte
Es ist kein Build-Prozess oder eine Installation notwendig.

Die Anwendung benötigt im Wesentlichen zwei Hauptkomponenten:
 * Datei-Ladefunktion: Eine Möglichkeit für den Benutzer, eine lokale .bin-Datei in die Anwendung zu laden.
 * Hex-Editor-Ansicht: Eine Schnittstelle, die den Inhalt der Datei in einem für Menschen lesbaren Hexadezimalformat darstellt und Bearbeitungen ermöglicht.
Beispielcode (HTML, CSS und JavaScript)
Dieser Code erstellt eine einfache Webseite, die eine Binärdatei laden und ihren Inhalt als Hex-Dump anzeigen kann. Änderungen werden ebenfalls widergespiegelt.
1. HTML-Datei (index.html)
Diese Datei strukturiert die Webseite mit einem Dateiauswahlfeld und einem Bereich für die Hex-Ansicht.

Wie man es benutzt
 * Speichern: Speichern Sie die drei Code-Blöcke als index.html, style.css und app.js im selben Ordner.
 * Öffnen: Öffnen Sie die index.html-Datei in Google Chrome.
 * Laden: Klicken Sie auf "Datei auswählen" und wählen Sie eine .bin-Datei von Ihrem Computer.
 * Anzeigen und Bearbeiten: Der Inhalt wird als Hex-Code angezeigt. Sie können die Hex-Werte direkt im Textfeld bearbeiten.
 * Speichern: Klicken Sie auf "Änderungen speichern", um die bearbeitete Datei herunterzuladen.
Dies ist eine grundlegende Implementierung. Für eine vollwertige Anwendung könnten Sie Funktionen wie die Anzeige von ASCII-Äquivalenten, Suchen & Ersetzen und eine bessere Fehlerbehandlung hinzufügen.

Lokal ausführen
 * Laden Sie die index.html-Datei aus diesem Repository herunter.
 * Öffnen Sie die index.html-Datei in einem modernen Webbrowser wie Google Chrome, Firefox oder Edge.
Beitrag leisten
Beiträge zur Weiterentwicklung der App sind willkommen! Wenn Sie Ideen für neue Funktionen haben oder einen Fehler gefunden haben, lesen Sie bitte die CONTRIBUTING.md-Datei und erstellen Sie einen Pull Request oder ein Issue.


Binärdatei-Editor (Web-App)
Ein moderner, browserbasierter Hex-Editor zum Anzeigen und Bearbeiten von Binärdateien. Diese Anwendung läuft vollständig clientseitig – es werden keine Daten an einen Server gesendet.




Über diese Web-App
Der Binärdatei-Editor ist eine in sich geschlossene Single-Page-Application (SPA), die als Werkzeug für Entwickler, IT-Spezialisten und technisch Interessierte dient. Sie ermöglicht die schnelle Inspektion und Manipulation von Binärdateien direkt im Browser, ohne dass eine Installation von Desktop-Software erforderlich ist.
Alle Dateioperationen finden lokal im Speicher des Browsers statt, was maximale Geschwindigkeit und Datenschutz gewährleistet.
Features
 * Lokales Laden: Öffnen Sie .bin-Dateien oder beliebige andere Dateien von Ihrem lokalen System.
 * Interaktive Hex/ASCII-Ansicht: Die Daten werden übersichtlich mit Adress-Offset, Hexadezimalwerten und der entsprechenden ASCII-Darstellung angezeigt.
 * Direktes Bearbeiten: Klicken Sie auf einen beliebigen Hex- oder ASCII-Wert, um ihn zu ändern. Die korrespondierende Darstellung wird automatisch aktualisiert.
 * Änderungen speichern: Laden Sie die modifizierten Daten als neue Datei auf Ihren Computer herunter.
 * 100% Client-Side: Die Anwendung ist vollständig in Vanilla JavaScript, HTML5 und Tailwind CSS geschrieben. Es findet keine Server-Kommunikation statt.
 * Responsives Design: Die Benutzeroberfläche passt sich an verschiedene Bildschirmgrößen an.
Erste Schritte
Es ist kein Build-Prozess oder eine Installation notwendig.
  
 * : Lokal ausführen
 * Laden Sie die index.html-Datei aus diesem Repository herunter.
 * Öffnen Sie die index.html-Datei in einem modernen Webbrowser wie Google Chrome, Firefox oder Edge.
Beitrag leisten

Hex-Editor-Ansicht: Eine Schnittstelle, die den Inhalt der Datei in einem für Menschen lesbaren Hexadezimalformat darstellt und Bearbeitungen ermöglicht.
Beispielcode (HTML, CSS und JavaScript)
Dieser Code erstellt eine einfache Webseite, die eine Binärdatei laden und ihren Inhalt als Hex-Dump anzeigen kann. Änderungen werden ebenfalls widergespiegelt.
1. HTML-Datei (index.html)
Diese Datei strukturiert die Webseite mit einem Dateiauswahlfeld und einem Bereich für die Hex-Ansicht.
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Binärdatei-Editor</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Einfacher Binärdatei-Editor</h1>
        <p>Wählen Sie eine .bin-Datei aus, um ihren Inhalt anzuzeigen und zu bearbeiten.</p>
        <input type="file" id="fileInput" accept=".bin">
        <div id="hex-editor" contenteditable="true"></div>
        <button id="saveButton">Änderungen speichern</button>
    </div>
    <script src="app.js"></script>
</body>
</html>

2. CSS-Datei (style.css)
Diese Datei sorgt für ein einfaches und übersichtliches Layout.
body {
    font-family: Arial, sans-serif;
    background-color: #f0f2f5;
    color: #333;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
}

.container {
    background: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    width: 80%;
    max-width: 900px;
}

h1 {
    text-align: center;
    color: #1e88e5;
}

input[type="file"] {
    display: block;
    margin: 1.5rem auto;
}

#hex-editor {
    font-family: 'Courier New', Courier, monospace;
    white-space: pre;
    background-color: #fafafa;
    border: 1px solid #ddd;
    padding: 1rem;
    margin-top: 1rem;
    min-height: 300px;
    overflow-x: auto;
}

button {
    display: block;
    width: 100%;
    padding: 0.8rem;
    margin-top: 1.5rem;
    background-color: #1e88e5;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 1rem;
}

button:hover {
    background-color: #1565c0;
}

3. JavaScript-Datei (app.js)
Dies ist die Logik der Anwendung. Sie liest die Datei, konvertiert sie in ein Hex-Format und ermöglicht das Speichern.
document.addEventListener('DOMContentLoaded', () => {
    const fileInput = document.getElementById('fileInput');
    const hexEditor = document.getElementById('hex-editor');
    const saveButton = document.getElementById('saveButton');
    let fileBuffer;
    let originalFilename = 'edited.bin';

    fileInput.addEventListener('change', (event) => {
        const file = event.target.files[0];
        if (!file) {
            return;
        }

        originalFilename = file.name;
        const reader = new FileReader();

        reader.onload = (e) => {
            fileBuffer = e.target.result;
            const view = new Uint8Array(fileBuffer);
            let hexString = '';
            for (let i = 0; i < view.length; i++) {
                // Fügt alle 16 Bytes eine neue Zeile hinzu
                if (i > 0 && i % 16 === 0) {
                    hexString += '\n';
                }
                // Konvertiert das Byte in einen zweistelligen Hex-String
                const hex = view[i].toString(16).padStart(2, '0').toUpperCase();
                hexString += hex + ' ';
            }
            hexEditor.textContent = hexString;
        };

        reader.readAsArrayBuffer(file);
    });

    saveButton.addEventListener('click', () => {
        if (!fileBuffer) {
            alert("Bitte laden Sie zuerst eine Datei.");
            return;
        }

        // Bereinigt den Text und konvertiert ihn zurück in Bytes
        const hexString = hexEditor.textContent.replace(/\s+/g, '');
        const byteArray = new Uint8Array(hexString.length / 2);

        for (let i = 0; i < hexString.length; i += 2) {
            byteArray[i / 2] = parseInt(hexString.substr(i, 2), 16);
        }document.addEventListener('DOMContentLoaded', () => {
    const fileInput = document.getElementById('fileInput');
    const hexEditor = document.getElementById('hex-editor');
    const saveButton = document.getElementById('saveButton');
    let fileBuffer;
    let originalFilename = 'edited.bin';

    fileInput.addEventListener('change', (event) => {
        const file = event.target.files[0];
        if (!file) {
            return;
        }

        originalFilename = file.name;
        const reader = new FileReader();

        reader.onload = (e) => {
            fileBuffer = e.target.result;
            const view = new Uint8Array(fileBuffer);
            let hexString = '';
            for (let i = 0; i < view.length; i++) {
                // Fügt alle 16 Bytes eine neue Zeile hinzu
                if (i > 0 && i % 16 === 0) {
                    hexString += '\n';
                }
                // Konvertiert das Byte in einen zweistelligen Hex-String
                const hex = view[i].toString(16).padStart(2, '0').toUpperCase();
                hexString += hex + ' ';
            }
            hexEditor.textContent = hexString;
        };

        reader.readAsArrayBuffer(file);
    });

    saveButton.addEventListener('click', () => {
        if (!fileBuffer) {
            alert("Bitte laden Sie zuerst eine Datei.");
            return;
        }

        // Bereinigt den Text und konvertiert ihn zurück in Bytes
        const hexString = hexEditor.textContent.replace(/\s+/g, '');
        const byteArray = new Uint8Array(hexString.length / 2);

        for (let i = 0; i < hexString.length; i += 2) {
            byteArray[i / 2] = parseInt(hexString.substr(i, 2), 16);
        }

        // Erstellt ein Blob-Objekt und einen Download-Link
        const blob = new Blob([byteArray], { type: 'application/octet-stream' });
        const link = document.createElement('a');
        link.href = URL.createObjectURL(blob);
        link.download = `edited_${originalFilename}`;
        document.body.appendChild(link);
        link.click();
        document.body.removeChild(link);
    });

Beiträge zur Weiterentwicklung der App sind willkommen! Wenn Sie Ideen für neue Funktionen haben oder einen Fehler gefunden haben, lesen Sie bitte die CONTRIBUTING.md-Datei und erstellen Sie einen Pull Request oder ein Issue.
Lizenz
Dieses Projekt steht unter der Lizenz. Details finden Sie in der LICENSE-Datei.

Marc P.



