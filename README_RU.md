# FRANK

FRANK - это универсальная платформа для эмуляции аппаратного обеспечения на базе Raspberry Pico и Raspberry Zero. Это аппаратный форк проекта [Murmulator](https://murmulator.ru/) от Alex Ekb, включающий множество дополнительных функций.

Название "FRANK" происходит от имени "Франкенштейн", так как он объединяет различные компоненты из разных проектов.

## Поддерживаемые платформы

FRANK поддерживает эмуляцию различных платформ, включая:

- **ZX Spectrum**: Эмуляция классического 8-битного домашнего компьютера; позволяет пользователям запускать оригинальное программное обеспечение и игры для ZX Spectrum. Также поддерживает улучшенные версии ZX Spectrum с дополнительными функциями.
- **Atari 800**: Поддержка эмуляции семейства домашних компьютеров Atari 8-bit.
- **NES**: Эмуляция Nintendo Entertainment System (Dendy).
- **Game Boy**: Эмуляция оригинальных Game Boy, Game Boy Color и Game Boy Advance.
- **Sega Master System**: Эмуляция домашней консоли Sega Master System.
- **Sega Game Gear**: Эмуляция портативной консоли Sega Game Gear.
- И многие другие.

Эти возможности эмуляции делают FRANK универсальной платформой для любителей ретро-компьютеров и энтузиастов.

## Как сделать самостоятельно

Вы можете заказать печатные платы у любого производителя. Я рекомендую [JLCPCB](https://jlcpcb.com/), но вы можете выбрать любого поставщика. Размер печатной платы FRANK менее 10x10 см, что делает производство максимально недорогим.

Вы можете скачать файлы Gerber [здесь](./gerber/). Последняя ревизия - 1.12.

Вам потребуются следующие компоненты:

| Компонент | Описание               | Кол-во | Тип                | Ссылка                                                                 |
|-----------|------------------------|--------|--------------------|------------------------------------------------------------------------|
| AU1       | AUDIO OUT              | 1      | PJ-325C            | [Link](https://www.aliexpress.com/item/1005006710837751.html)           |
| AU2       | AUDIO IN               | 1      | PJ-325C            | [Link](https://www.aliexpress.com/item/1005006710837751.html)           |
| C1,C2,C3,C6 | 1u                   | 4      | Polar              | [Link](https://www.aliexpress.com/item/1005002524973878.html)           |
| C4,C7,C8,C14,C5,C13 | 100n         | 6      | SMD                | [Link](https://www.aliexpress.com/item/32964553793.html)                |
| C9,C10,C15 | 10u                   | 3      | 0805               | [Link](https://www.aliexpress.com/item/32964553793.html)                |
| C11,C12   | 10n                    | 2      | 0805               | [Link](https://www.aliexpress.com/item/32964553793.html)                |
| C16       | 220u                   | 1      | Polar              | [Link](https://www.aliexpress.com/item/1005002524973878.html)           |
| CON1      | Display                | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| CON2      | OUT                    | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| CON3      | IN                     | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| D1,D2,D3  | 1N4148                 | 3      | SOD-323            | [Link](https://www.aliexpress.com/item/1005007681952673.html)           |
| D4,D5,D6,D7,PWR2 | 3V3             | 5      | SOD-323            | [Link](https://www.aliexpress.com/item/32997486634.html)                |
| DB1       | RS232                  | 1      | DB9 Female         | [Link](https://www.aliexpress.com/item/4000659356343.html)              |
| DB2,DB3   | Joystick               | 2      | DB9 Female         | [Link](https://www.aliexpress.com/item/4000659356343.html)              |
| HDMI1     | HDMI                   | 1      | Female 4 DIP       | [Link](https://www.aliexpress.com/item/1005005248842433.html)           |
| JP1       | JMP RUN                | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP2       | Main Jumpers           | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP3       | GP18 Jumper            | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP4       | GP19 Jumper            | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP5       | JMP PSRAM              | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP6       | RS232 Jumpers          | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP7,JP9,JP10 | RP ZERO +5V Jumper  | 3      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| JP8       | I2S                    | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| KB1       | PS/2                   | 1      | PS/2 6P            | [Link](https://www.aliexpress.com/item/4000106131593.html)              |
| L1        | LED                    | 1      | 0805               | [Link](https://www.aliexpress.com/item/838002118.html)                  |
| MAX1      | MAX232CSE+             | 1      | SO 16PIN           | [Link](https://www.aliexpress.com/item/1005006286473801.html)           |
| PSR1      | PSRAM                  | 1      | SOP8               | [Link](https://www.aliexpress.com/item/1005006440914173.html)           |
| PWR1      | 5V                     | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| Q1,Q2     | BC850                  | 2      | SOT-23             | [Link](https://www.aliexpress.com/item/33017911878.html)                |
| R1,R2,R11,R35,R36,R37,R38,R55 | 1K | 8    | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R3,R4,R5,R6,R7,R8,R9,R10,R40,R41,R42,R43,R44,R45 | 270R | 14 | 0805 | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R12,R13,R14,R25,R26 | 330R         | 5      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R15,R16,R17,R30,R33 | 1k           | 5      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R18,R19,R20,R21,R27,R28,R29,R34 | 10K | 8  | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R22,R23,R24,R47,R48 | 100R         | 5      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R31,R32   | 2k                     | 2      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R39       | 750R                   | 1      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R46       | 300R                   | 1      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R49,R50,R51,R52,R53 | 150R         | 5      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R54       | 51R                    | 1      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| R56,R57   | 5.1K                   | 2      | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)           |
| RP1       | RP2040 Pico            | 1      | Pico               | [Link](https://www.aliexpress.com/item/1005006055009344.html)           |
| RP2       | RP 2040 Zero           | 1      | Zero               | [Link](https://www.aliexpress.com/item/1005006354505058.html)           |
| SC1       | VIDEO (Soft Composite) | 1      | RCA-103            | [Link](https://www.aliexpress.com/item/1005006152724809.html)           |
| SD1       | Micro SD               | 1      | Push-Push          | [Link](https://www.aliexpress.com/item/1005004214252441.html)           |
| SW1       | SW_Push_Dual           | 1      | 3 x 3 x 1.5 mm     | [Link](https://www.aliexpress.com/item/1005001629293584.html)           |
| TDA1      | TDA1387T               | 1      | SOP-8              | [Link](https://www.aliexpress.com/item/32995595000.html)                |
| UART1     | UART                   | 1      | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)           |
| USB1      | USB Type C             | 1      | 16 Pin SMT         | [Link](https://www.aliexpress.com/item/1005005500797563.html)           |
| VGA1      | VGA                    | 1      | DB15 Female 90 Degree | [Link](https://www.aliexpress.com/item/32842951548.html)               |

## Джамперы

На печатной плате есть несколько джамперов, которые включают или отключают различные функции FRANK.

### JP1

Соединяет пины RUN и RST на Pico. Обычно не подключается.

### JP2

Основные джамперы, которые включают/выключают некоторые базовые функции.

*Важно*: Подключайте джамперы горизонтально; каждая строка представляет собой отдельный переключатель.

| Джампер    | Описание                                       |
|------------|------------------------------------------------|
| RST        | Подключает RST к GPIO23 на Pico                |
| PS/2 CLK   | Включает клавиатуру PS/2 (подключает пин CLK)  |
| PS/2 DATA  | Включает клавиатуру PS/2 (подключает пин DATA) |
| BEEP       | Включает пищалку (подключает BEEP_OUT к GPIO28)|
| L          | Включает левый аудиоканал                      |
| R          | Включает правый аудиоканал                     |
| LOAD       | Включает функцию загрузки с ленты              |

Если вы запаяли чип TDA, включите его, установив вторые пины джамперов "L" и "R" JP2 к JP8.

![alt text](images/jp2.png)

### JP3, JP4 и JP5

Подключите джамперы JP3, JP4 и JP5 для работы PSRAM, если вы запаяли его. Если вы не хотите использовать чип PSRAM, оставьте джампер JP5 не запаянным.

### JP6

Эти джамперы должны быть подключены, если вы собираетесь использовать функцию RS232 в FRANK. Каждый из четырех переключателей соединяет соответствующие пины Pico и MAX232.

*Примечание*: RS232 использует GPIO16 и GPIO17 на Pico, которые также используются геймпадом.

### JP7

Этот джампер включает второй геймпад.

### JP8

Этот джампер включает первый геймпад.

*Примечание*: RS232 использует GPIO16 с первым геймпадом. Возможно, стоит отключить этот джампер, если вы собираетесь использовать RS232.