#Bluetooth Beamer Fernsteuerung
Aug 24th, 2014

Viele Beamer bieten die Möglichkeit der Steuerung via RS-232-Schnittstelle. Mithilfe eines Bluetooth-Seriell-Wandlers (HC-06) sowie eines Pegelwandlers wird im Folgenden eine Bluetooth-Schnittstelle zur Fernsteuerung per Android App entwickelt.

###Hardware
![Beamer mit RS-232 Schnittstelle](https://github.com/felixfreyer/Bluetooth-Beamer-Fernsteuerung/raw/main/rs232.png "Beamer mit RS-232 Schnittstelle")
**Abbildung 1: Beamer mit RS-232 Schnittstelle
**

Für die Verwendung des Bluetooth-Seriell-Wandlers muss zunächst der Pegel der RS-232-Schnittstelle angepasst werden. Hierfür wird ein herkömmlicher RS232-TTL Konverter eingesetzt.

![RS232-TTL Konverter](https://github.com/felixfreyer/Bluetooth-Beamer-Fernsteuerung/raw/main/converter.jpg "RS232-TTL Konverter")
**Abbildung 2: RS232-TTL Konverter
**

Als Bluetooth-Seriell-Wandler wird das HC-06 Bluetooth Board verwendet. Dieses kann direkt mit dem Pegelwandler verbunden werden und benötigt keine externe Spannungsversorgung.

![HC-06 Bluetooth-Seriell-Wandler](https://github.com/felixfreyer/Bluetooth-Beamer-Fernsteuerung/raw/main/hc06.jpg "HC-06 Bluetooth-Seriell-Wandler")
**Abbildung 3: HC-06 Bluetooth-Seriell-Wandler
**

Die serielle RS-232-Schnittstelle des Beamers muss anschließend noch an die Konfiguration des HC-06 angepasst werden: Default serail port setting : 9600, N, 8, 1 Pairing code : 1234 Nachdem die verwendete Hardware beschrieben wurde, folgt nun die entwickelte Android App.


###Software

![Android App](https://github.com/felixfreyer/Bluetooth-Beamer-Fernsteuerung/raw/main/screenshot.png "Android App")
**Abbildung 4: Android App
**

Die App ermöglicht die Fernsteuerung des Beamers per Bluetooth. Neben der manuellen Steuerung ist ebenfalls eine Sprachsteuerung implementiert. Für zukünftige Erweiterungen können die „BenQ RS232 Commands“ verwendet werden.

Download: [BeamerRemote.apk](https://github.com/felixfreyer/Bluetooth-Beamer-Fernsteuerung/blob/main/BeamerRemote.apk "BeamerRemote.apk")
