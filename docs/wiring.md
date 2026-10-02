# Wiring guide

This is a low-voltage prototype wiring plan for **Trailer Level Monitor GPS Trip Logging**. Confirm every module's datasheet because breakout-board pinouts vary.

| Component | Suggested pin | Role | Check |
| --- | --- | --- | --- |
| cellular modem | 7 | Digital I/O | Confirm the module voltage and pinout before power-up. |
| GPS module | 8 | Digital I/O | Confirm the module voltage and pinout before power-up. |
| Status output | LED_BUILTIN | Output | Use a resistor when an external LED is fitted. |

## Power

- Use a regulated supply sized for the selected modules.
- Join grounds unless an interface is explicitly isolated.
- Do not connect mains voltage directly to a development board.
- Add a fuse, emergency stop, and certified isolation where a real actuator can create risk.
