# ESP8266_bistabilen_WIFI_Relais

Auf Basis eines ESP8266 Clones sollen hier Schaltmodule Vorgestellt werden das an die SNOFF Module angelehnt ist. 
Diese können zum dauerhaften schalten von 230 Volt verwendet werden. Die Entsprechenden Relais müssen hier aber dauerhaft angesteuert werden. 
Um diesem Manko  des dauerhaft aktiven Stromes durch das Relais Abhilfe zu schaffen habe ich mich für Bistabile Relais entschieden. Die Ansteuerung erfolgt hier über Motortreiber die auch das umpolen ( EIN- / AUS schalten ) ermöglichen sollen.

Belegung der ESP8266 Funktionen

    01 REST über 10K Widerstand an 3V3
    02 ADC an Pfostenleiste
    03 CH_PD über 10K Widerstand an 3V3
    04 GPIO 16 EIN / AUS Vollbrücke Umschalten
    05 GPIO 14 Auswahl Relais 1
    06 GPIO 12 Auswahl Relais 2
    07 GPIO 13 Ausgang OC 1
    08
    09 GPIO 11 Ausgang OC2
    10 GPIO 7 Input 1
    11 GPIO 9 Input 2
    12 GPIO 10
    13 GPIO 8
    14 GPIO 6
    15
    16 GPIO 15 muss per def. beim starten auf LOW
    17 GPIO 2 LED WLAN Modul ( hier nur Symboliosch )
    18 GPIO 0 über Jumper zum Flashen auf low
    19 GPIO 4 SDA I2C
    20 GPIO 5 SCL I2C
    21 GPIO 3 RxD0 ( Firmware Update Pfostenleiste )
    22 GPIO 1 TxD0 ( Firmware Update Pfostenleiste )
