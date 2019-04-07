## My own Docker Nextcloud config

Die installation erfolgt komplet über ansible.

Es handelt sich um eine Standart Nextcloud, Docker, Nginx reverse Proxy Config
Ich verwende als Datenbank eine mariadb bzw. einen mariadb Container.

Die Daten liegen ausehalb der Container, so das eine aktuallisierung kein Problem machen sollte.

Einzig die uploadsize.conf ist nicht standart.
Hier erhöhe ich die max datei größe.

### Container:
- jwilder/nginx-proxy
- jrcs/letsencrypt-nginx-proxy-companion
- nextcloud
- mariadb:latest
- kmb32123/youtube-dl-server 
