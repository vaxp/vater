# 🚀 VAXP Terminal (vater)

Vater is the official terminal application for the VAXP-OS distribution. It aims to balance advanced aesthetics ("Vanta Class") with high performance. The UI is built with Flutter while core terminal work uses custom FFI libraries for efficient I/O and PTY emulation.

## ✨ Key Features

- **Vanta Class Aesthetics:** Built on VAXP-OS design language with a Black Acrylic / Blur effect to enhance the desktop experience.
- **Superior FFI Performance:** Uses custom FFI libraries written in system languages to deliver efficient I/O processing and PTY emulation. Targets very low memory usage (under ~60MB idle).
- **Stability in Complex Environments:** Architectural decisions and suggested isolation deployment (Flatpak, etc.) help keep the app stable across different Linux systems.
- **Advanced Stream Handling:** Designed to handle complex interactive terminal programs (for example, htop) with low latency and high responsiveness.

## Building and Running (Linux)

Vater's UI is implemented with Flutter and uses native FFI libraries for core functionality.

### Prerequisites

- Flutter SDK (with Linux desktop support enabled)
- Linux development toolchain: GCC or Clang, CMake, Ninja
- Any additional native libraries required by the FFI components (platform-specific)

### Build steps

Clone the repository and fetch packages:

```bash
git clone <vater repository link>
cd vater
flutter pub get
```

Build for Linux:

```bash
flutter build linux
```

### Run (after building)

Run the built binary (release):

```bash
./build/linux/x64/release/vater
```

## ⚖️ License (VAXPECO)

This project is licensed under the VAXPECO (VAXP Ecosystem Open License).

VAXPECO grants broad freedom to use, modify, distribute, and relicense the code (including the right to close-source derived works).

### 📜 Conditional Attribution Requirement

The project places a conditional requirement on re-using the `vater` name or attributing a modified app to VAXP-OS. Attribution is only permitted if **both** of the following are met:

1. **Aesthetic Criteria (Vanta Class):** The modified project preserves the core Vanta Class / Black Glass visual style and does not remove or substantially alter the essential documented visual features.
2. **Performance Criteria:** The modified project meets or exceeds the documented performance targets (for example, similar or better memory characteristics — ~65MB idle as documented).

This requirement is intended to encourage either (a) respectful preservation of the VAXP identity when keeping the same name, or (b) differentiation under a new name when those criteria are not met.

---

If you need extra help (for example, adding build instructions for development mode, CI steps, or packaging with Flatpak), tell me what you'd like and I can add it to this README.