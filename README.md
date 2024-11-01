# Home Server Docker Scripts - README

Welcome to your home server setup! This README covers the essentials and extra features in your Docker scripts, so you can easily run and manage your server with style and precision. Due to being a software engineer my documentation in this is well "iNtUItIvE". Thanks to ChatGPT for generating well "most" of this documentation. It doesnt have my sense of humour yet.

## Why I uploaded this?

I started slowly setting up my own self-hosted services for easier access. Mainly for Plex in order to watch movies and shows. Won't say how i get them but you can use it self-host your entire content and its a creative way to learn how does networking, infrastructure and distributed computing work in the modern age.

So what better way to do then to learn and share my work for others to provide valuable feedback and maybe learn on how to run their own services.

I am sure many others upload their scripts and they are probably more clear and robust than mine but mine are basic and "should" get the job done, hopefully.

---

## 🛠️ What’s in This Repository?

This repository contains Docker Compose scripts and configurations designed for a flexible, powerful home server setup. Use these scripts to run a suite of self-hosted applications, ranging from media servers to cloud storage, network ad blockers, and more. Customize each service to fit your needs and scale up or down as you see fit!

### Highlights

- **Easy Setup**: Just run `docker-compose up -d` to start services effortlessly.
- **Modular Design**: Each service is configured in its own directory, making it easy to add, remove, or adjust applications.
- **Self-Hosting Essentials**: Core services include media streaming, file storage, VPN, DNS-based ad-blocking, and more.
- **Backup and Restore Support**: Regular updates and persistent volumes ensure your data is safe.
- **Customizable and Scalable**: Start with the basics or load up with more advanced services; everything is adaptable to your hardware.

---

## 🎩 Requirements

Before running the scripts, make sure you have:

- **Docker** installed ([Install Docker](https://docs.docker.com/get-docker/))
- **Docker Compose** for orchestrating multiple containers ([Install Docker Compose](https://docs.docker.com/compose/install/))
- **Storage Space** to handle media, backup, and persistent data volumes
- **Basic Linux Knowledge** (recommended for command-line usage)

---

## 🚀 Quick Start

1. **Clone the Repository**  
   Clone this repository to your server:
   ```bash
   git clone https://github.com/vishmango117/HomeServer.git
   cd HomeServer
   ```
2. **Access the different types of scripts by overall function**
   There are different scripts i use categorized into 4 main areas.

   1. Core Services such as Plex and Immich for Photo and Video streaming and hosting,
   2. Download Box that use qbittorrent, and all the \*arrs for tracking and following movies, and tv series.
   3. DNS for local DNS management using Pi-Hole.
   4. DevSandbox which comprises of a localized version of Github codespaces using open source versions of vscode in the browsers and my own Jupyter Server.
   5. More to be populated and updated.

   Each zone has a reverse-proxy script and a monitoring docker compose script to setup up traefik (reverse-proxy) and connection to portainer for container metrics and management of resources.

## Some Additional Information

I will be uploading the scripts over time to sanitize the scripts some of the credentials are just hard-coded into the docker scripts after i kept futzing with the .env file and they just refused to work like as if they are on strike.
