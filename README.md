# Zebra RFID SDK Sample (TC501)

This project demonstrates how to integrate the Zebra RFID SDK into an Android application to interact with Zebra RFID readers (e.g., RFD40, RFD8500).

## Core Functionalities

- **Initialization**: Setting up the `Readers` instance and choosing the transport layer.
- **Discovery**: Locating available RFID readers via Bluetooth, USB, or Serial.
- **Connection Management**: Connecting and disconnecting from selected readers.
- **Event Handling**: Responding to reader appearance and disappearance (auto-reconnect).
- **Inventory & Barcode**: Basic RFID tag inventory and barcode scanning support.

## Getting Started

### Prerequisites
- Zebra RFID SDK (`api3lib-release.aar`) included in the project.
- Android 12+ requires Bluetooth permissions (`BLUETOOTH_SCAN`, `BLUETOOTH_CONNECT`).

### Quick Start
1. Initialize the `RFIDHandler` in your Activity.
2. The SDK will automatically attempt to find and connect to a paired reader.
3. Use `performConnect()` and `performDisconnect()` to manage the lifecycle manually.

For detailed design and code snippets, see [design.md](./design.md).
