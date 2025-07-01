# Proto-Projekt

[Zum Planner](https://github.com/users/ThePitPool/projects/2)

#LCD-Anzeige mit Node-RED auf dem Raspberry Pi

Projekt zur Anzeige der aktuellen Temperatur auf einem LCD-Display per Knopfdruck, gesteuert über Node-RED auf einem Raspberry Pi.

---

##Ziel des Projekts

Ziel ist es, mit einem Taster ein 16x2-LCD-Display so anzusteuern, dass:
- **oben** Temperatur steht,
- **unten** Die Temperatur in Grad ausgeschrieben.

Die Anzeige erfolgt nach 1-2 Sekunde nach Tastendruck und basiert auf der Verknüpfung von Hardware (GPIOs, I2C-LCD) und Software (Node-RED & Python).

---

##Projektphasen

### Phase 1: Planung & Konzeption
- Definition des Projektziels
- Auswahl der benötigten Hardware und Software
- Grobe Struktur und Zeitplan festlegen  
** Wichtigkeit:** Grundlegend für einen effizienten und strukturierten Ablauf.

---

### Phase 2: Hardware-Vorbereitung
- LCD-Display per I2C anschließen
- Taster korrekt an GPIO anschließen
- Optional: Temperatur-Sensor (z. B. DHT22) anschließen
- I2C im Raspberry Pi aktivieren  
** Wichtigkeit:** Fehlerfreie Verkabelung ist Voraussetzung für ein funktionierendes System.

---

### Phase 3: Software-Einrichtung
- Node-RED auf dem Raspberry Pi installieren  
  [Node-RED auf Raspberry Pi installieren – YouTube-Tutorial](https://www.youtube.com/watch?v=8BjZpWn5GIE)
- Python3 + LCD-Bibliotheken installieren:
  ```bash
  sudo apt-get install python3-smbus i2c-tools
  pip3 install RPLCD
### Phase 4: Node-RED-Flow erstellen
- GPIO-Eingang für Taster konfigurieren
- Temperatur über (Sensor) oder API abrufen
- LCD mit Python-Skript ansteuern (z. B. über exec-Node)
- Flow testen und debuggen

---

Lösungsansätze
- Visuelle Programmierung: Dank Node-RED ist die Steuerlogik leicht verständlich, wartbar und flexibel.
- Modularer Aufbau: Jede Komponente (LCD, Button, Temperatur) funktioniert eigenständig.
- Kombination aus Python und Node-RED: So wird die einfache Bedienbarkeit von Node-RED mit der Hardware-Nähe von - - Python vereint.
- Erweiterbarkeit: Das System lässt sich leicht mit neuen Funktionen (Web-Dashboard, Wetter-API, Zeiterfassung  etc.) erweitern.
- Fehlertoleranz: Durch Testphasen und Debugging in Node-RED werden Fehler früh erkannt und eliminiert.

---

### 🛠 Verwendete Technologien
Hardware
- Raspberry Pi (z. B. 3B oder 4)
- 16x2 LCD-Display mit I2C-Modul
- GPIO-Taster
(Optional): Temperatursensor (z. B. DHT22, DS18B20)
🔧 Software & Tools
- Node-RED (Flow-Programmierung)
- Python 3 (für LCD-Ansteuerung)


---

Warum ist das Projekt einzigartig?
Verbindet Elektronik, visuelle Programmierung, Skripting, I2C-Kommunikation und GUI-Elemente.
Ideal für Einsteiger: Es benötigt keine tiefen Kenntnisse in Programmierung oder Elektronik, ist aber dennoch technisch spannend.
Praktischer Nutzen: Kann als Grundmodul für eine Wetterstation, ein Raumüberwachungsgerät oder ein smartes Display dienen.
Fördert das Verständnis für GPIOs, Datenverarbeitung, Visualisierung und Automatisierung.
Die Kombination aus Knopf und Display erzeugt direkt Feedback, perfekt für Vorführungen oder Lernzwecke.

---



