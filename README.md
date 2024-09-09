# Pudim Kubernetes Infrastructure

This repository contains the yml files for all the deployments on my home kubernetes cluster (called Pudimnetes). It is the heart of all the selfhosted systems I use every day. It runs everything from a plex server, a mqtt broker, some data collectors, my smart home hub, many websites, and a very useful telegram bot.

## Deployments

### Self-hosted infrastructure

My Kubernetes cluster runs quite a lot of services I use frequently. Here are some of them:

 - Jellyfin: a self-hosted and open source local media library
 - Plex: a closed-source competitor of Jellyfin
 - Nextcloud: an open source Google Drive alternative
 - HomeAssistant: An open source smart home hub
 - A [private git server](https://github.com/LeRenner/private-git-docker) for large and private git projects I have
 - Wireguard: a VPN that runs in some of the servers I have access to
 - An Icecast server for my [Congohas Airport web radio](https://pudim.xyz/radio)
 - A Transmission torrent client for all my Linux ISOs ;)

### Personal projects

I also run many of my small projects on my cluster! Some of them are:

- My [smart lights](https://github.com/LeRenner/pudimLights)
- A [Logger](https://github.com/LeRenner/iOSLogger) for my iOS shortcuts
- My Mom's personal website
- My anonymous messages website
- My projects website: [pudim.xyz](https://github.com/LeRenner/pudim.xyz)
