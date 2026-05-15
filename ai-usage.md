# AI Usage Log — stm32-sensor-logger

AI tools (Claude) used during development. Short log per day.

## Day 1 — May 8, 2026
- Troubleshooting STM32CubeIDE installation (missing CubeMX components).
- Code written from CubeMX-generated templates and ST official examples.

## Day 2 — May 9, 2026
- Breadboard wiring layout for external LED on D6/PB10.
- Counter + modulo pattern for non-blocking two-rate blink.
- Git setup and first commit workflow.
- All hardware verified on bench; all code reviewed and edited by me before flashing.

## Day 3 — May 14, 2026
- Tactile button wiring (4-pin, straddling breadboard central gap).
- GPIO input with internal pull-up configured in CubeMX.
- Active-LOW button read with HAL_GPIO_ReadPin.
- Multimeter setup attempted, parked for separate session (not needed for Day 3).
- Debugged button orientation by rotating 90° (fixed instantly).

## Day 4 - May 15, 2026
- printf retarget via _write() override - standard pattern from STM32 community.
- Edge detection idiom for button state transitions.
- Tera Term install and 115200 baud config.
- All code reviewed and edited by me before flashing.