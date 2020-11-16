# ntp
NTP Howto

source : https://www.digitalocean.com/community/tutorials/how-to-set-up-time-synchronization-on-debian-10


# date actuelle
**date**
Mon Nov 16 09:37:51 UTC 2020
=> UTC = universel

# Debian Buster NTP
Première chose : la Time Zone
**timedatectl list-timezones**
...
Europe/Moscow
Europe/Oslo
**Europe/Paris**
Europe/Podgorica
Europe/Prague
...
=> liste les TZ disponibles

**timedatectl set-timezone Europe/Paris**
=> règle la TZ

**date**
Mon Nov 16 10:42:26 CET 2020
=> CET = Central European Time
