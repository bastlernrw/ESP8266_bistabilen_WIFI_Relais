Alle Befehle und Infos dazu findet man hier:

https://github.com/arendst/Sonoff-Tasmota/wiki/Commands


Beispiel:

Einen Tasmota-Sonoff mit der internen Netzwerk-IP 192.168.178.48 (das ist ein Beispiel!) einschalten:

http://192.168.178.48/cm?cmnd=Power%20On


Da dies eine interne IP-Adresse zur Nutzung hinter einem Router ist, kann das so nicht über das Internet, also außerhalb des Routers, funktionieren. Dazu muß man im Router einen Port weiter leiten. Bei der Fritz-Box auch "Freigabe" genannt. Es gibt auch Router, welche das gar nicht können.


2.) Die Interne IP 192.168.178.48 soll nun über das Internet angesprochen werden können. Hier das Beispiel zur Fritzbox:


Jetzt ist der Tasmota-Sonoff immer unter derselben Adresse über das Internet schaltbar (XXXXXXXX ist euer gewählter Name bei Goip):

http://XXXXXXX.goip.de/cm?cmnd=Power%20On


Um den Sonoff noch abzusichern, empfiehlt es sich in den Tasmota-Einstellungen ein Passwort für den Webservice in den Einstellungen zu hinterlegen. Da der Standard-Benutzer "admin" heißt (kann man auch noch in der Config ändern), ändert sich der Aufruf dann wiefolgt:

XXXXXXXX = gewählter goip-Name & YYYYYYYY = gewähltes Tasmota-Passwort:


http://XXXXXXXX.goip.de/cm?use…=YYYYYYYY&cmnd=Power%20On<http://XXXXXXXX.goip.de/cm?user=admin&password=YYYYYYYY&cmnd=Power%20On>


Jetzt kann das ganze auch mit IFTTT gesteuert werden.



wird noch erweitert
