# stm32-sensor-logger

STM32F411RE embedded systems learning project — sensor logging, GPIO, I2C, UART, state machine.

Part of an 8-month roadmap toward small-satellite avionics / on-board ML for CubeSats.

## Hardware

- **MCU board:** STM32 Nucleo-F411RE
- **Sensors:** BME280 (temperature/humidity/pressure, I2C), MPU6050 (IMU, I2C)
- **Storage:** microSD via SPI breakout
- **Comms:** USART2 over ST-Link virtual COM port
- **Tools:** AZDelivery 8-ch 24MHz logic analyzer, PeakTech 1035 multimeter

## Roadmap

- **Project 1 (Month 1):** GPIO + I2C sensor + UART state machine
- **Project 2 (Month 2):** RTOS task scheduling
- **Project 3 (Month 3):** Custom PCB in KiCad
- **Project 4–5:** Edge ML inference on CubeSat-class hardware
- **Project 6:** HIL test rig

## Progress

### Day 1 — May 8, 2026
Onboard LED (LD2 / PA5) blinking at 1 Hz. HAL-based, CubeMX-generated project.

### Day 2 — May 9, 2026
External LED on D6 (PB10), 330 ohm series resistor.
Two-rate non-blocking blink using counter + modulo: LD2 at 1 Hz, external LED at 2.5 Hz, base tick 100 ms.

### Day 3 — May 14, 2026
External push button on D8 (PA9, internal pull-up). When pressed, base tick drops from 100 ms to 30 ms — both LEDs blink ~3× faster. Active-LOW input. First GPIO input pin.

---

This project uses AI-assisted development (Claude). See `ai-usage.md` for the usage log.
