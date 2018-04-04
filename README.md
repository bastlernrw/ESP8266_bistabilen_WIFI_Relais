# ESP8266_bistabilen_WIFI_Relais

Auf Basis eines ESP8266 Clones soll hier Schaltmodul Vorgestellt werden,  das an die SNOFF Module angelehnt ist. 
Diese können zum dauerhaften schalten von 230 Volt verwendet werden. Die Entsprechenden Relais müssen hier aber dauerhaft angesteuert werden. 
Um diesem Manko des dauerhaft aktiven Stromes durch das Relais Abhilfe zu schaffen,  habe ich mich für Bistabile Relais entschieden. Die Ansteuerung erfolgt hier über Motortreiber die auch das umpolen ( EIN- / AUS schalten ) ermöglichen sollen.

Belegung der ESP8266 Funktionen

* 1 REST über 10K Widerstand an 3V3 
* 2 ADC an Pfostenleiste
* 3 CH_PD über 10K Widerstand an 3V3
* 4 GPIO 16 EIN / AUS Vollbrücke Umschalten 
* 5 GPIO 14 Auswahl Relais 1
* 6 GPIO 12 Auswahl Relais 2
* 7 GPIO 13 Ausgang Optokoppler 1
* 8 VCC
* 9 GND
* 10 GPIO 15 muss per def. beim starten auf LOW 
* 11 GPIO  2  LED WLAN Modul ( hier nur Symboliosch )
* 12 GPIO  0  über Jumper zum Flashen auf low
* 13 GPIO  4  SDA I2C
* 14 GPIO  5  SCL I2C
* 15 GPIO  3  RxD0 ( Firmware Update Pfostenleiste )  
* 16 GPIO  1  TxD0 ( Firmware Update Pfostenleiste )
* 17 GPIO 11  Ausgang Optokoppler 2
*  18 GPIO  7  Input 1
* 19 GPIO  9  Input 2 
* 20 GPIO 10 SPIWD
* 21 GPIO  8  MOSI
* 22 GPIO  6  CLK
