# Central Transport Tracker – Update System

## 🇵🇱 Polski

Repozytorium służy jako **centralny system aktualizacji aplikacji Central Transport Tracker**.  
Zawiera wszystkie pliki niezbędne do dystrybucji aktualizacji aplikacji, modułów oraz komponentów dodatkowych.

Repozytorium jest wykorzystywane przez **instalator / updater aplikacji**, który:
- sprawdza dostępność nowych wersji,
- pobiera wymagane pliki,
- aktualizuje aplikację oraz moduły.

---

## Zawartość repozytorium

W repozytorium znajdują się:

- 📦 Spakowane moduły aplikacji (`.zip`)
- 🎨 Assety graficzne (ikony, komunikaty)
- 🧩 Pliki telemetryczne Win32 / Win64 do *Euro Truck Simulator 2*
- 🖥️ Binarka aplikacji **Central Transport Tracker**
- 🔄 Instalator / updater aplikacji
- 📄 Plik `latest.json` zawierający informacje o aktualnej wersji

---

## Struktura folderów

```text
CTT_GITHUB
├── assets
│   ├── check.png
│   ├── error.png
│   ├── icon.ico
│   └── icon.png
│
├── builds
│   └── Central Transport Tracker.exe
│
├── installer
│   └── CTT_Installer.exe
│
├── modules
│   ├── mod_delivery_quests.zip
│   ├── mod_discord_rpc.zip
│   ├── mod_telemetry.zip
│   └── mod_updater.zip
│
├── releases
│   └── latest.json
│
├── Win32
│   └── scs-telemetry.dll
│
└── Win64
    └── scs-telemetry.dll
```

---

## Opis katalogów

### `assets`
Pliki graficzne wykorzystywane przez aplikację oraz instalator/updater.

### `builds`
Aktualna wersja binarna aplikacji **Central Transport Tracker**.

### `installer`
Instalator oraz updater odpowiedzialny za:
- pierwszą instalację aplikacji,
- aktualizacje aplikacji,
- pobieranie i aktualizowanie modułów.

### `modules`
Moduły aplikacji spakowane w archiwa `.zip`, ładowane dynamicznie przez core aplikacji.

### `releases`
Plik `latest.json` zawierający informacje o:
- numerze wersji,
- dostępnych aktualizacjach,
- plikach wymaganych do pobrania.

### `Win32` / `Win64`
Pliki telemetryczne (`scs-telemetry.dll`) dla **Euro Truck Simulator 2**, w zależności od architektury systemu.

---

## Informacja

Repozytorium **nie jest przeznaczone do bezpośredniego uruchamiania przez użytkownika końcowego**.  
Służy wyłącznie jako zaplecze aktualizacji dla aplikacji **Central Transport Tracker**.

---

## 🇬🇧 English

This repository serves as the **central update system for the Central Transport Tracker application**.  
It contains all files required for distributing application updates, modules, and additional components.

The repository is used by the **application installer / updater**, which:
- checks for new versions,
- downloads required files,
- updates the application and its modules.

---

## Repository Contents

The repository includes:

- 📦 Packed application modules (`.zip`)
- 🎨 Graphic assets (icons, status images)
- 🧩 Win32 / Win64 telemetry files for *Euro Truck Simulator 2*
- 🖥️ Central Transport Tracker application binary
- 🔄 Application installer / updater
- 📄 `latest.json` file containing version information

---

## Folder Structure

```text
CTT_GITHUB
├── assets
│   ├── check.png
│   ├── error.png
│   ├── icon.ico
│   └── icon.png
│
├── builds
│   └── Central Transport Tracker.exe
│
├── installer
│   └── CTT_Installer.exe
│
├── modules
│   ├── mod_delivery_quests.zip
│   ├── mod_discord_rpc.zip
│   ├── mod_telemetry.zip
│   └── mod_updater.zip
│
├── releases
│   └── latest.json
│
├── Win32
│   └── scs-telemetry.dll
│
└── Win64
    └── scs-telemetry.dll
```

---

## Notice

This repository is **not intended to be run directly by end users**.  
It is used exclusively as an update backend for the **Central Transport Tracker** application.
