# MRL Tools

A single-page web tool with two main features:

## Features

### 🔍 狀態碼查詢 (Status Code Decoder)
Decode hexadecimal status codes for master controller diagnostics:
- **STAT** – System status register
- **INPUT G** – Input signal register
- **RNCS** – NV-SRAM checksum status
- **GLST** – Galil card/axis status (16-bit & 32-bit)
- **RLS** – Robot limit switch status (16-bit & 32-bit)
- **ALST** – Pre-aligner status

Each decoder shows:
- Binary representation of the hex value
- Bit-by-bit breakdown with English & Chinese descriptions
- Highlighted triggered bits
- Screenshot download button

### 🔄 單位轉換 (Unit Converter)
- **氣壓換算** – Pressure (Torr, Pa, kPa, MPa, PSI, atm, bar, mbar, kg/cm², mmHg)
- **匯率換算** – Currency (TWD, USD, EUR, JPY, GBP, and more; live rates via API)
- **數字單位換算** – Numerical (M, B, T, 萬, 億, 兆)
- **體積換算** – Volume (m³, cm³, L, mL, gal, cc, ft³, fl oz)
- **長度換算** – Length (m, cm, mm, km, in, ft)

## Tech Stack

- Pure HTML / CSS / JavaScript (no build step required)
- [Google Fonts – Inter & JetBrains Mono](https://fonts.google.com/)
- [html2canvas](https://html2canvas.hertzen.com/) for screenshot export
- [exchangerate-api.com](https://www.exchangerate-api.com/) & [CoinGecko](https://www.coingecko.com/) for live currency rates

## Usage

Open `index.html` directly in any modern browser — no server needed.

> GitHub Pages is supported. Set the source branch to `main` and the root to `/`.
