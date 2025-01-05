# FRANK

FRANK ist eine vielseitige Hardware-Emulationsplattform, die auf Raspberry Pico und Raspberry Zero basiert. Es handelt sich um einen Hardware-Fork des [Murmulator](https://murmulator.ru/) Projekts von Alex Ekb, der zahlreiche zusätzliche Funktionen integriert.

Der Name "FRANK" leitet sich von "Frankenstein" ab, da es verschiedene Komponenten aus unterschiedlichen Projekten integriert, ähnlich wie Dr. Frankenstein sein Monster aus verschiedenen Körperteilen erschuf. Diese Kombination ermöglicht es FRANK, ein einzigartiges und leistungsstarkes Set an Fähigkeiten zu bieten.

## Unterstützte Plattformen

FRANK unterstützt die Emulation für eine Vielzahl von Plattformen, darunter:

- **ZX Spectrum**: Emuliert den klassischen 8-Bit-Heimcomputer und ermöglicht es Benutzern, originale ZX Spectrum-Software und -Spiele auszuführen. Es unterstützt auch erweiterte Versionen des ZX Spectrum mit zusätzlichen Funktionen.
- **Atari 800**: Unterstützt die Emulation der Atari 8-Bit-Heimcomputerfamilie.
- **NES**: Emuliert das Nintendo Entertainment System und ermöglicht es Benutzern, klassische NES-Spiele zu spielen.
- **Game Boy**: Bietet Emulation für die originalen Game Boy-, Game Boy Color- und Game Boy Advance-Handheld-Konsolen.
- **Sega Master System**: Emuliert die Sega Master System-Heimkonsole.
- **Sega Game Gear**: Unterstützt die Emulation der Sega Game Gear-Handheld-Konsole.
- Und viele mehr.

Diese Emulationsfähigkeiten machen FRANK zu einer vielseitigen Plattform für Retro-Computing-Enthusiasten und Hobbyisten.

## Wie man seinen eigenen FRANK baut

Sie können die PCBs bei jedem Hersteller bestellen. JLCPCB wird empfohlen, aber Sie können jeden Lieferanten wählen. Die FRANK PCB-Größe beträgt weniger als 10x10 cm, was die Produktion kostengünstig macht.

Sie können die Gerber-Dateien [hier](./gerber/) herunterladen. Die neueste Revision ist 1.12.

Die folgenden Teile werden benötigt, um Ihren eigenen FRANK zu bauen:

| Referenz  | Wert                   | Menge | Typ                | AliExpress                                                                 |
|-----------|------------------------|-------|--------------------|----------------------------------------------------------------------------|
| AU1       | AUDIO OUT              | 1     | PJ-325C            | [Link](https://www.aliexpress.com/item/1005006710837751.html)               |
| AU2       | AUDIO IN               | 1     | PJ-325C            | [Link](https://www.aliexpress.com/item/1005006710837751.html)               |
| C1,C2,C3,C6 | 1u                   | 4     | Polar              | [Link](https://www.aliexpress.com/item/1005002524973878.html)               |
| C4,C7,C8,C14,C5,C13 | 100n         | 6     | SMD                | [Link](https://www.aliexpress.com/item/32964553793.html)                    |
| C9,C10,C15 | 10u                   | 3     | 0805               | [Link](https://www.aliexpress.com/item/32964553793.html)                    |
| C11,C12   | 10n                    | 2     | 0805               | [Link](https://www.aliexpress.com/item/32964553793.html)                    |
| C16       | 220u                   | 1     | Polar              | [Link](https://www.aliexpress.com/item/1005002524973878.html)               |
| CON1      | Display                | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| CON2      | OUT                    | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| CON3      | IN                     | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| D1,D2,D3  | 1N4148                 | 3     | SOD-323            | [Link](https://www.aliexpress.com/item/1005007681952673.html)               |
| D4,D5,D6,D7,PWR2 | 3V3             | 5     | SOD-323            | [Link](https://www.aliexpress.com/item/32997486634.html)                    |
| DB1       | RS232                  | 1     | DB9 Female         | [Link](https://www.aliexpress.com/item/4000659356343.html)                  |
| DB2,DB3   | Joystick               | 2     | DB9 Female         | [Link](https://www.aliexpress.com/item/4000659356343.html)                  |
| HDMI1     | HDMI                   | 1     | Female 4 DIP       | [Link](https://www.aliexpress.com/item/1005005248842433.html)               |
| JP1       | JMP RUN                | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP2       | Main Jumpers           | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP3       | GP18 Jumper            | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP4       | GP19 Jumper            | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP5       | JMP PSRAM              | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP6       | RS232 Jumpers          | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP7,JP9,JP10 | RP ZERO +5V Jumper  | 3     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| JP8       | I2S                    | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| KB1       | PS/2                   | 1     | PS/2 6P            | [Link](https://www.aliexpress.com/item/4000106131593.html)                  |
| L1        | LED                    | 1     | 0805               | [Link](https://www.aliexpress.com/item/838002118.html)                      |
| MAX1      | MAX232CSE+             | 1     | SO 16PIN           | [Link](https://www.aliexpress.com/item/1005006286473801.html)               |
| PSR1      | PSRAM                  | 1     | SOP8               | [Link](https://www.aliexpress.com/item/1005006440914173.html)               |
| PWR1      | 5V                     | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| Q1,Q2     | BC850                  | 2     | SOT-23             | [Link](https://www.aliexpress.com/item/33017911878.html)                    |
| R1,R2,R11,R35,R36,R37,R38,R55 | 1K | 8   | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R3,R4,R5,R6,R7,R8,R9,R10,R40,R41,R42,R43,R44,R45 | 270R | 14 | 0805 | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R12,R13,R14,R25,R26 | 330R         | 5     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R15,R16,R17,R30,R33 | 1k           | 5     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R18,R19,R20,R21,R27,R28,R29,R34 | 10K | 8 | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R22,R23,R24,R47,R48 | 100R         | 5     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R31,R32   | 2k                     | 2     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R39       | 750R                   | 1     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R46       | 300R                   | 1     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R49,R50,R51,R52,R53 | 150R         | 5     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R54       | 51R                    | 1     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| R56,R57   | 5.1K                   | 2     | 0805               | [Link](https://www.aliexpress.com/item/1005005600798857.html)               |
| RP1       | RP2040 Pico            | 1     | Pico               | [Link](https://www.aliexpress.com/item/1005006055009344.html)               |
| RP2       | RP 2040 Zero           | 1     | Zero               | [Link](https://www.aliexpress.com/item/1005006354505058.html)               |
| SC1       | VIDEO (Soft Composite) | 1     | RCA-103            | [Link](https://www.aliexpress.com/item/1005006152724809.html)               |
| SD1       | Micro SD               | 1     | Push-Push          | [Link](https://www.aliexpress.com/item/1005004214252441.html)               |
| SW1       | SW_Push_Dual           | 1     | 3 x 3 x 1.5 mm     | [Link](https://www.aliexpress.com/item/1005001629293584.html)               |
| TDA1      | TDA1387T               | 1     | SOP-8              | [Link](https://www.aliexpress.com/item/32995595000.html)                    |
| UART1     | UART                   | 1     | 2.54               | [Link](https://www.aliexpress.com/item/1005007039504981.html)               |
| USB1      | USB Type C             | 1     | 16 Pin SMT         | [Link](https://www.aliexpress.com/item/1005005500797563.html)               |
| VGA1      | VGA                    | 1     | DB15 Female 90 Degree | [Link](https://www.aliexpress.com/item/32842951548.html)                  |

## Jumper

Auf der PCB befinden sich mehrere Jumper, die verschiedene Funktionen des FRANK aktivieren oder deaktivieren.

### JP1

Verbindet die RUN- und RST-Pins des Pico. Normalerweise ist dies nicht verbunden.

### JP2

Dies sind die Hauptjumper, die einige der Kernfunktionen aktivieren.

*Wichtig*: Verbinden Sie die Jumper horizontal; jede Reihe stellt ihren eigenen Schalter dar.

| Jumper     | Beschreibung                                  |
|------------|-----------------------------------------------|
| RST        | Verbinden Sie RST mit GPIO23 des Pico         |
| PS/2 CLK   | PS/2-Tastatur aktivieren (CLK-Pin verbinden)  |
| PS/2 DATA  | PS/2-Tastatur aktivieren (DATA-Pin verbinden) |
| BEEP       | Beeper aktivieren (BEEP_OUT zu GPIO28)        |
| L          | Linken Audioausgangskanal aktivieren          |
| R          | Rechten Audioausgangskanal aktivieren         |
| LOAD       | Kassettenladefunktion aktivieren              |

Der Audioteil ist etwas komplex. Wenn Sie den TDA-Chip löten, aktivieren Sie ihn, indem Sie die zweiten Pins der "L"- und "R"-Jumper von JP2 mit JP8 verbinden.

![alt text](images/jp2.png)

### JP3, JP4 und JP5

Verbinden Sie die JP3-, JP4- und JP5-Jumper, um PSRAM zu aktivieren, falls vorhanden. Wenn Sie den PSRAM-Chip nicht löten möchten, lassen Sie den JP5-Jumper wie er ist.

### JP6

Diese Jumper sollten verbunden werden, wenn Sie die RS232-Funktionalität des FRANK nutzen möchten. Jeder der vier Schalter verbindet die entsprechenden Pins von Pico und MAX232.

*Hinweis*: RS232 teilt sich GPIO16 und GPIO17 des Pico, die auch vom Gamepad verwendet werden.

### JP7

Dieser Jumper aktiviert das zweite Gamepad.

### JP8

Dieser Jumper aktiviert das erste Gamepad.

*Hinweis*: RS232 teilt sich GPIO16 mit dem ersten Gamepad. Es könnte ratsam sein, diesen Jumper zu entfernen, wenn Sie RS232 verwenden möchten.