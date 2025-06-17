# Proto-Projekt
# 📟 Raspberry Pi LCD-Anzeige mit Node-RED

## 🎯 Ziel des Projekts

Dieses Projekt zeigt, wie man mit einem Raspberry Pi, Node-RED und einem LCD-Display Informationen anzeigt. Durch Drücken eines physischen Knopfs sollen automatisch:

- **In der oberen Zeile des LCDs:** die aktuelle Temperatur
- **In der unteren Zeile:** das aktuelle Tagesdatum

angezeigt werden.

---

## 🧰 Tools und Technologien

| Komponente            | Beschreibung                              |
|-----------------------|-------------------------------------------|
| **Raspberry Pi**      | Zentrale Steuereinheit                    |
| **Node-RED**          | Visuelle Programmierumgebung              |
| **LCD-Display (16x2)**| Anzeige der Informationen über I2C       |
| **Python**            | Ansteuerung des LCD-Displays              |
| **GPIO Button**       | Auslöser zur Anzeige                      |
| **(Optional) Sensor** | z. B. DHT11/DHT22 für Temperaturmessung   |

---

## ⚙️ Vorbereitung

### 🔌 Raspberry Pi einrichten

1. Raspberry Pi OS installieren
2. I2C aktivieren:
   ```bash
   sudo raspi-config
   → Interfacing Options → I2C → Enable
