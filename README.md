# ntp
NTP Howto

source : https://www.digitalocean.com/community/tutorials/how-to-set-up-time-synchronization-on-debian-10

# Installer le service NTP
Sous Debian
```sh
root@host ~# apt install ntp
```
Normallement le service se lance tout seul mais on peut vérifier avec ```systemctl status ntp```

# Date actuelle
``` sh
user@host ~# date
Mon Nov 16 09:37:51 UTC 2020
```
=> UTC = universel

# Debian Buster NTP
Première chose : la Time Zone
``` sh
user@host ~# timedatectl list-timezones
...
Europe/Moscow
Europe/Oslo
Europe/Paris
Europe/Podgorica
Europe/Prague
...
```
=> liste les TZ disponibles

``` sh
user@host ~# timedatectl set-timezone Europe/Paris
```
=> règle la TZ
``` sh
user@host ~# date
Mon Nov 16 10:42:26 CET 2020
```
=> CET = Central European Time
