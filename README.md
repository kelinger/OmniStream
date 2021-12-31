# OmniStream

OmniStream is a collection of Docker containers and utilities/commands for building a personal streaming server with your own media residing on cloud providers' data storage platform.  You can pick from an assortment of options and containers and have full control to tweak settings and processes without have any former knowledge of Docker and a minimal skillset in Linux.

## Currently supported containers (included in OmniStream setup)
### Core components
* Oauth - For many containers, you can bypass their built in authentication and instead utilize an oauth provider, such as Google, for a single-sign-on experience.
* Watchtower - oversee your containers and install updates as they become available
* AutoHeal - restart failed containers
* Traefik - a front end reverse proxy that registers your containers with Let's Encrypt for free SSL certificates.  Supports integration with CloudFlare for wildcard domains as well as individual certificates for each site.  Also allows reverse proxy to sites not part of the OmniStream project.
### Streamers
* Plex - Plex Media Server with or without hardware transcoding
* Emby - Emby Server with or without hardware transcoding
* Jellyfin - Jellyfin Server with or without hardware transcoding
* Tautulli - Plex reporting and tracking
* Embystat - Emby reporting and tracking
### Usenet
* NZBget - Usenet downloader
* SABnzbd - Usenet downloader
* Hydra - Usenet indexer and search engine
### BitTorrent Engines
* Deluge
* qBitTorrent
* Transmission
* Transmission VPN - like transmission but forces downloads through a VPN so as not to share your server's IP
* rTorrent
### Cataloging Tools
* Radarr - Movie cataloging and downloading
* Sonarr - TV Show cataloging and downloading
* Lidarr
* Medusa
* Organizr
* Jackett
* Bazarr
### Utilities and extras
* NextCloud
* NetData - server and container statistics and monitoring
* Guacamole
* Portainer - Full stack Docker management
* OVPN - OpenVPN server
* Apache
* Speed - Test the speed to and from your server to your client (true speed test between your endpoints)
### Databases
* MySQL
* MariaDB
* Postgre
* MS SQL Server
* Redis

In almost all cases, each container is not dependent on any others meaning you can pick and choose which of the above (other than core) you would or would not like to use.  Obviously, running something like Tautulli without Plex may be useless but you can still choose to do this (say to configure Tautulli to monitor a Plex installation elsewhere).

...

## Aknowledgements (to be expanded and detailed)
* perPLEXed
* Rclone
* Animosity
* Original app and container developers
