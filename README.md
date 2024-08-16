# nogasm-i2c
adding i2c connectivity (slave address 0x08)

```
+-------------+-------------+-------------+-------------+-------------+
| Byte 1      | Byte 2      | Byte 3      | Byte 4      | Byte 5      |
+-------------+-------------+-------------+-------------+-------------+
| Motor Speed | Pressure    | Pressure    | avgPressure | avgPressure |
|             | (High Byte) | (Low Byte)  | (High Byte) | (Low Byte)  |
+-------------+-------------+-------------+-------------+-------------+
```

You need to soilder: (left teensy lc - right esp32dev)
- 18(SDA) -> 21(SDA)
- 19(SCL) -> 22(SCL)
- GND -> GND
- 5v -> 5v

See nogasm-bridge for home assistant auto discovery bridge
