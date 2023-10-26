# Pudim Kubernetes Infrastructure

This repository contains the yml files for all the deployments on my home kubernetes cluster (called Pudim). It is the heart of all the selfhosted systems I use every day. It runs everything from a plex server, a mqtt broker, some data collectors, my smart home hub, many websites, including a Grafana, and a very useful telegram bot.

## Deployments

### Websites

The main websites running on this cluster are:

 - Jellyfin: selfhosted and open source local media library
 - Plex: closed source selfhosted local media library
 - Nextcloud: syncs files and backups
 - Pudim Website: main page for my projects website Pudim.xyz, containing subpages for my smart lights, the Pudim Mailer, and some other smaller projects
 - Grafana: collects and visualizes data from my home

### Proxies and message routers:

Some containers just redirect messages to their correct places. Some of them are:

 - PLS backend: receives HTTP requests from the lights API and sends MQTT packets for the lights
 - Pudim Mailer: receives messages from the Mailer frontend and forwards them as MQTT packets to the telegram messenger
 - Telegram Messenger: receives messages over MQTT and sends them to the Telegram Bot API
 - Mosquitto: MQTT broker that routed most of the messages on my local network
 - TOR: makes the Pudim website available over The Onion Router
