# SimpleClock — Rainmeter Skin

An elegant desktop clock for [Rainmeter](https://www.rainmeter.net/) that sits centred over your wallpaper and shows the time **down to the second**.

---

## Preview

```
┌──────────────────────────────────────────────────┐
│                                                  │
│                   14:37:09                       │   ← live, updates every second
│                                                  │
│  ──────────────────────────────────────────────  │
│           Wednesday, January 15 2025             │
│                                                  │
└──────────────────────────────────────────────────┘
```

- **Frosted-glass card** — blurs whatever wallpaper sits behind it (Windows 10+)  
- **Centred automatically** — adapts to any screen resolution  
- **Zero dependencies** — uses Segoe UI Light (built into Windows 10/11)  
- Updates every **1 second** exactly

---

## Installation

### Option A — One-click installer (recommended)

1. Download and install [Rainmeter](https://www.rainmeter.net/) if you haven't already.
2. Double-click **`SimpleClock.rmskin`** — Rainmeter will install and load it automatically.

### Option B — Manual

1. Copy the **`Skins/SimpleClock`** folder into:
   ```
   %USERPROFILE%\Documents\Rainmeter\Skins\
   ```
2. Open Rainmeter (system tray icon → **Manage**).
3. Click **Refresh All**, then expand **SimpleClock** and double-click `SimpleClock.ini`.

---

## Customisation

Open `SimpleClock.ini` in any text editor (Notepad works fine).  
All tweakable settings are grouped under the `[Variables]` section at the top:

| Variable    | Default             | Description                                  |
|-------------|---------------------|----------------------------------------------|
| `CardFill`  | `8,10,28,185`       | Card background colour (R,G,B,Alpha 0–255)   |
| `CardBorder`| `255,255,255,30`    | Card border colour                           |
| `TimeFace`  | `Segoe UI Light`    | Font for the time — any installed font works |
| `TimeSize`  | `72`                | Time font size (points)                      |
| `TimeColor` | `255,255,255,255`   | Time text colour                             |
| `DateFace`  | `Segoe UI`          | Font for the date                            |
| `DateSize`  | `14`                | Date font size (points)                      |
| `DateColor` | `175,200,255,210`   | Date text colour                             |
| `SepColor`  | `255,255,255,35`    | Separator line colour                        |

### Switch to 12-hour time

In `[MeasureTime]`, change:
```ini
Format=%H:%M:%S
```
to:
```ini
Format=%I:%M:%S %p
```

### Move the clock

Right-click the skin → **Settings** → uncheck **Keep on screen** / drag it wherever you like, then lock it back.

---

## Requirements

| Requirement | Minimum |
|-------------|---------|
| Rainmeter   | 4.0     |
| Windows     | 10 (for blur effect; works on 8.1+ without blur) |

---

## License

MIT — do whatever you like with it.
