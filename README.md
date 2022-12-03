# OmniStream

OmniStream is a collection of Docker containers and utilities/commands for building a personal streaming server with your own media residing on cloud providers' data storage platform.  You can pick from an assortment of options and containers and have full control to tweak settings and processes without have any former knowledge of Docker and a minimal skillset in Linux.

## TL;DR
Download and install on a fresh Debian-like system with
`wget tinyurl.com/omniSetup -O /tmp/setup && chmod 700 /tmp/setup && /tmp/setup`

- Documentation:  https://omnistream.cloud
- Repository:   https://github.com/kelinger/OmniStream
- Discussions:  https://github.com/kelinger/OmniStream/discussions
- Report bugs:  https://github.com/kelinger/OmniStream/issues

---

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
### Cataloging Tools
* Radarr - Movie cataloging and downloading
* Sonarr - TV Show cataloging and downloading
* Lidarr - Music library management
* Medusa
* Organizr
* Jackett
* Bazarr
* Ombi
* Monitorr
* Prowlarr - Search centralization and management for other ---arr containers
### Utilities and extras
* Portainer - Full stack Docker management
* NetData - server and container statistics and monitoring
* NextCloud - Suite of cloud apps similar to Google, Microsoft, Dropbox, and other offerings
* OVPN - OpenVPN server
* Speed - Test the speed to and from your server to your client (true speed test between your endpoints)
* Apache - Host your own web projects
* Portainer Agent - Manage multiple servers with Portainer by adding this to remote servers
* WatchState - Sync watch status between Plex, Emby, and Jellyfin
* OnlyOffice - Web-based Office apps that can be integrated into NextCloud (create/edit online)
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
* CloudFlare integration (optional):  Automatically add and/or remove DNS entries for containers upon startup and shutdown respectively.  Includes setting caching options.  Also enables wildcard certificates (one certificate per domain versus one per container) when using CloudFlare.
* System backup for easy restore:  Includes differential backups for large containers (eg. Plex) to minimize storage and API transfer limitations.
* Plug-in scripting:  add your own functionality to critical scripts

...

## Acknowledgements (to be expanded and detailed)
* perPLEXed
* Rclone
* Animosity
* Original app and container developers
