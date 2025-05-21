# 4L_Nonpc

Ein Performance-Optimierungs-Skript für FiveM, entwickelt von **Life4Tune** für **4Life RP**.  
Dieses Skript reduziert gezielt die Fahrzeug- und Fußgängerpopulation sowie deaktiviert über 50 Welt-Szenarien, um eine stabilere Spielerfahrung zu bieten.

---

## ✨ Features

- Deaktiviert viele native Welt-Szenarien (z. B. Boot-Szenarien, Bauarbeiter, Polizei)
- Reduziert die allgemeine NPC- und Fahrzeuganzahl auf dem Server
- Verbessert die Performance in stark bevölkerten Regionen
- Perfekt für RP-Server, bei denen KI-Verkehr nicht erwünscht ist

---

## ⚙️ Was wird geändert?

- **Fahrzeug-Fernlichter** werden deaktiviert:  
  ```lua
  DisableVehicleDistantlights(true)
  ```

- **NPC- und Fahrzeugdichte wird begrenzt**:  
  ```lua
  SetPedPopulationBudget(5000)
  SetVehiclePopulationBudget(500)
  ```

- **Zufällige Events werden deaktiviert**:  
  ```lua
  SetRandomEventFlag(false)
  ```

- **Mehr als 50 GTA-Szenarien werden deaktiviert**, z. B.:

  - `WORLD_VEHICLE_POLICE`
  - `WORLD_VEHICLE_BOAT_IDLE`
  - `WORLD_VEHICLE_FIRE_TRUCK`
  - `WORLD_VEHICLE_MILITARY_PLANES_BIG`
  - `WORLD_VEHICLE_TRACTOR`
  - u.v.m.

---

## 🛠️ Installation

1. Lege das Skript in deinem Ressourcenordner ab (`resources/[local]/4L_trafficcontrol`).
2. Füge es in deiner `server.cfg` hinzu:

   ```plaintext
   ensure 4L_trafficcontrol
   ```

3. Stelle sicher, dass der Code in einer `client.lua` oder `client/main.lua` liegt.

---

## 🔧 Hinweis

Dieses Skript hat nur clientseitige Auswirkungen und wird automatisch bei allen Spielern geladen, sobald sie den Server betreten. Es wird empfohlen, dieses Skript möglichst früh zu starten, z. B. direkt nach ESX Core.

---

## 👨‍💻 Erstellt von

**Life4Tune**  
Für das Projekt **4Life RP**  
[https://www.4-life.net](https://www.4-life.net)