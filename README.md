# OmniStream

OmniStream is a collection of Docker containers and utilities/commands for building a personal streaming server with your own media residing on cloud providers' data storage platform.  You can pick from an assortment of options and containers and have full control to tweak settings and processes without have any former knowledge of Docker and a minimal skillset in Linux.

---
WARNING - Most code is written; this is being ported into a GIT project and it is strongly recommended that you do NOT clone this project until this message is removed.  Until then, it is quite possible that anything downloaded from here will not yet be a complete project.
---

## TL;DR
Download and install on a fresh Debian-like system with
`wget tinyurl.com/omniSetup -O /tmp/setup && chmod 700 /tmp/setup && /tmp/setup`

Documentation:  https://omnistream.cloud

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
* Transmission
* Transmission VPN - like transmission but forces downloads through a VPN so as not to share your server's IP
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
* Portainer - Full stack Docker management
* OVPN - OpenVPN server
* Apache - Host your own web projects
* Speed - Test the speed to and from your server to your client (true speed test between your endpoints)
### Databases
* MySQL
* MariaDB
* Postgre
* MS SQL Server
* Redis + Redis Commander

In almost all cases, each container is not dependent on any others meaning you can pick and choose which of the above (other than core) you would or would not like to use.  Obviously, running something like Tautulli without Plex may be useless but you can still choose to do this (say to configure Tautulli to monitor a Plex installation elsewhere).

## Additional features
* Menu-driven setup:  Get up and running in no time!
* Easy updates:  keep OmniStream and containers on the most recent build automatically.
* Personal container management:  add your own Docker containers to be managed by the OmniStream stack
* Command-line and menu-based functions for simplified management
* CloudFlare integration (optional):  Automatically add and/or remove DNS entries for containers upon startup and shutdown respectively.  Includes setting caching options.
* System backup for easy restore:  Includes differential backups for large containers (eg. Plex) to minimize storage and API transfer limitations.
* Plug-in scripting:  add your own functionality to critical scripts
...

## Acknowledgements (to be expanded and detailed)
* perPLEXed
* Rclone
* Animosity
* Original app and container developers
