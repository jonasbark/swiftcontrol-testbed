# swiftcontrol-testbed

A web-based testing tool for SRAM Bluetooth devices using the Web Bluetooth API.

## Features

- 🔌 Connect to SRAM devices via Bluetooth Web API
- 📊 Automatically subscribe to all notification/indication characteristics
- 📖 Read all readable characteristics
- 🔄 Test shift operations (Shift Up/Shift Down)
- 📋 Copy logs to clipboard for analysis
- ⚙️ Toggle between SRAM-only and any BLE device modes

## Usage

1. Open [sram_test.html](./sram_test.html) in Chrome, Edge, or Opera browser (Web Bluetooth support required)
2. Use the "Only SRAM devices" checkbox to filter:
   - **Checked**: Only show SRAM devices (with full service access)
   - **Unchecked**: Show all BLE devices
3. Click "Connect to Device" and select your device
4. Use the buttons to interact with your device:
   - **Read All**: Read all readable characteristics
   - **Shift Up/Down**: Test shift operations
   - **Copy to Clipboard**: Copy all logs

## Development

The page is automatically deployed to GitHub Pages when changes are pushed to the main branch.

## Requirements

- Modern browser with Web Bluetooth API support (Chrome, Edge, or Opera)
- HTTPS connection (required for Web Bluetooth)
- Bluetooth-enabled device

## Security

The application uses proper escaping to prevent XSS vulnerabilities and only connects to devices explicitly selected by the user.

