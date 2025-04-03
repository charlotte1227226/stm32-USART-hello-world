# stm32-USART-hello-world

使用 STM32F103C8T6 的 USART 外設實現透過 UART 傳送 `"Hello World!"` 到電腦端的範例。

---

## 專案簡介

本專案使用 STM32F103C8T6 開發板，透過 USART1 傳送字串資料至電腦端。
開發環境為 STM32CubeIDE，資料由 USB 模組接收並可由串口調試助手顯示。

---

## 硬體需求

- STM32F103C8T6 開發板（Blue Pill）
- USB to TTL 模組（如 CH340 或 FT232）
- 杜邦線數條
- 電腦

---

## 接線說明

| STM32F103C8T6 | USB 模組 |
|---------------|--------------|
| PA9 (TX)      | RX           |
| PA10 (RX)     | TX           |
| GND           | GND          |

請確認 TX ↔ RX 交叉接法。

---

## 開發環境

- STM32CubeIDE
- STM32 標準外設庫（或 HAL）
- GCC 工具鏈（內建於 STM32CubeIDE）
- 串口調試助手

---

## 預設參數

- USART Port: **USART1**
- Baud rate: **115200 bps**
- Data bits: **8**
- Stop bit: **1**
- Parity: **None**

---
