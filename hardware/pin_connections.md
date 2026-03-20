# STM32F407VGTx Pin Connections

| Peripheral              | STM32 Pin | Component              | Mode/Type              | Notes                                      |
|------------------------|-----------|------------------------|------------------------|--------------------------------------------|
| PIR Sensor             | PA1       | Motion Sensor          | GPIO_INPUT             | High when motion detected                  |
| Green LED              | PD12      | Onboard Green LED      | GPIO_OUTPUT            | ON when no motion                          |
| Red LED (Onboard)      | PD14      | Onboard Red LED        | GPIO_OUTPUT            | ON when motion detected                    |
| Red LED (External)     | PD3       | External Red LED       | GPIO_OUTPUT            | ON when motion detected                    |
| Buzzer                 | PD1       | Active Buzzer          | GPIO_OUTPUT            | ON for 2s on motion                        |
| Servo Motor            | PE9       | SG90 Servo             | TIM1_CH1 (PWM output)  | 50 Hz PWM, duty controls 0°–180°           |
| LCD (I2C) - SCL        | PB6       | 16x2 I2C LCD Display   | I2C1_SCL               | Address 0x4E (shifted 7-bit I2C)           |
| LCD (I2C) - SDA        | PB7       | 16x2 I2C LCD Display   | I2C1_SDA               |                                            |