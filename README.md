# Überblick über bisher durchgeführte Projekte (Produktiv und im HomeLab)

Besitzer/-in: wwlabs Homelab
Verifizierung: Verifiziert
Tags: Administration, Homelab, SUMUP, WWLABS

Hier sind sämtliche Projekte aufgeführt, die ich bisher durchgeführt habe.

Die Umsetzung erfolgte im Home-Lab, im Praktikum für Kunden, in der Cloud oder für das persönliche Umfeld.

Die Liste ist nicht vollständig, da einige Topics in Vergessenheit geraten sind. Die Liste wird bei Gelegenheit fortgeführt.

Für die meisten Inhalte werden nach und nach eigene Artikel aus meinen Notizen folgen.

Die Sortierung ist nicht nach Wichtigkeit oder grad der Kenntnisse, sondern rein zufällig!

---

## **Virtualisierung** 


- ProxMox: gute Kenntnisse
- Einrichtung von Virtualisierungs-Cluster aus 3-4 Nodes mit Einsatz von ProxMox
- ProxMox Backupserver Global Replication zwischen mehreren Standorten
- VMware, Virtual Box und Hyper-Virtualisierung
- Microsoft Virtual PC als erster Hypervisor
- Android Emulatoren: BlueStacks, Nox Player, BlissOS, Remix OS, Andy, Android x86 VM und Genymotion als persönlicher Favorit Android Emulator

## Mail

- Exchange-Server für Kunden im Praktikum
- MailQow via Docker und onPrem (Linux Mailserver-Stack)
- Einrichtung von SPF, DKIM und DMARC
- Mailpiler als Mailarchiv

## Docker

- Docker und Docker Compose (Windows & Linux, Desktop & Terminal)
- Portainer als grafisches Management-Tool für Docker
- Dockge zur Administrierung von Docker Compose

## VPN

- OpenVPN für mehrere Kunden im Praktikum
- Wireguard-Server als LXC-Container und Verbindung mit Windows, Linux und Android
- Twingate: im regelmäßigen Einsatz, moderne Zero Trust Network Access Solution
- Cloudflare Zero Trust Network Access (ZTNA) und Cloudflare Tunnel
- OPNsense: Site-to-Site Tunnel mittels Wireguard zur Verbindung von 2 Standorten

## Benutzerverwaltung

- Microsoft Active Directory und Group Policies, gute Kenntnisse
- Samba-Server: Linux Domaincontroller auf dem Raspberry Pi 400
- OpenLDAP-Server als LXC-Container im HomeLab (Test-Deployment)
- TurnKey Domaincontroller, Linux DC mit GUI als LCX-Container
- UCS Univention Corporate Server, Debian-basierte Lösung, DC mit GUI

## Scripting

- PowerShell gute Kenntnisse,
- z.B. als deutlich erweitertes Schulprojekt: Skripte zur Erstellung einer Infrastruktur aus 2 DCs, 1 FS und 1 Client mittels Hyper-V, unattended Windows-Installation, Installation aller benötigten Serverrollen und Dienste, AD-Domain-Erstellung und Join aller Domainmember, Erstellung von 20 Usern aus einer CSV, Einrichtung von Berechtigungsgruppen aus einer CSV und Zuweisung von Berechtigungen nach dem Konzept AGDLP, Erstellung von mehrschichtigen Netzwerk-Freigaben auf dem FS und Vergabe von Berechtigungen
- Linux-Bash, gute Kenntnisse
- z.B. mein Github-Postinstall-Script: Update, Installation der Standardtools, Einrichtung von SSH, Einrichtung von meiner individualisierten MOTD-Meldung, Installation von Starship, FastFetch und Nerd Fonts, Anpassung der BashRC und und eigener Aliase
- erste Kenntnisse in Python

## Webauftritt und CMS

- Ghost, modernes CMS als eigene Webseite, Docker und OnPrem
- WordPress für einen Kunden im Praktikum, deployed als LCX-Container auf ProxMox mit MariaDB, Redis, PhpMyAdmin, Fail2Ban und SSH-Zugang mit Public Key Authentifizierung
- Drupal, Django & Processwire CMS als Docker & onPrem im HomeLab
- Hugo: simpler “static website Generator” mittels Markup-Dateien als Docker, LXC, Github Pages & Cloudflare Pages
- Grav: simples CMS, Markup-Files in Ordners, mit grafischer Verwaltung

## Fileserver, NAS, RAID

- Windows Fileserverrolle auf Windows Server 2018, 2022 und 2025
- OpenMediaVault: moderne Debian basierte NAS-Lösung
- Unraid: moderne NAS-Lösung mit sehr vielen Funktionen
- TrueNAS: FreeBSD basiertes und sehr umfangreiches NAS-OS, RAID mit ZFS, nutzt ECC-RAM
- zmb-Fileserver: vom Bashclub bereitgestellte Samba Fileserver-Lösung als LXC-Container
- Debian mit manuell erstellten SMB und NFS-Shares und ZFS-Dateisystem
- Turnkey Fileserver als LXC-Container mit einer Web-UI
- Kodi: freier Media-Server auf dem Raspberry Pi

## Wiki, Doku-System, SSOK

- DokuWiki als Docker und LXC
- WikiJS, Wiki-System mit Markup, HTML, WYSIWYG-Editor und weiteren Funktionen
- Notion als Wissenssammlung und Notizbuch
- OneNote und Obsidian als Notizbuch und “Single Source of Knowledge”
- Raneto, Plattform zur Verwaltung der Wissensdatenbank, Markup
- Bookstack, Docsie, Fosswiki, MoinMoin, Documize, xWiki und Pelican als Testdeployment via Docker und als LXC, bei der Suche nach einem guten Wiki/Doku System
- PineDocs: simple grafische Lösung zur Darstellung z.B. einer Doku
- HBStack: moderne grafische Darstellung von Inhalten und Markup-Files
- ReadtheDocs: Framework zur Verwaltung von Dokus

## Collab-Tools

- Nextcloud als LXC, Docker, Bitnami und Turnkey Templates
- z.B. für einen Kunden im Praktikum: Deployment von Nextcloud als LXC, mit Fail2Ban, Webmin, MariaDB und Redis, Integration von OnlyOffice Docs
- OnlyOffice Workspace und Documentserver als selfhosted Plattform zur gleichzeitigen, gemeinsamen Arbeit an Office-Dokumenten, Desktop, Browser und auf dem Android
- Excalidraw und draw.io, selfhosted Tools zur kollaborativen Erstellung von Diagrammen, Whiteboards, Skizzen usw., Zugriff mittels Browser

## Monitoring, Notifications

- Uptime Kuma: selfhosted Monitoring Tool zur Überwachung der Erreichbarkeit, der gesamten HomeLab-Infrastruktur im dauerhaften Einsatz
- Grafana in Kombination mit Prometheus oder InfluxDB in mehreren Szenarien, via Docker und als onPrem-Installation
- Netdata: als Grafana alternative, Monitoring des ProxMox-Clusters & von Portainer-Hosts, Cloud und als selfhosted Linux-Installation
- Observium: Open Source Network Monitoring Tool als Turnkey-LXC
- Gotify: selfhosted Notification-Server in GO, mit entsprechenden Bashskripten zur Benachrichtigung bei verfügbaren Updates, Abschluss von ZFS Scrub usw.
- Eigene Notification-Bots in Telegram & Zoho z.B. Benachrichtigung bei Downtime in Uptime Kuma

## Kommunikation:

3CX: selfhosted VOIP-Telefonanlage, im HomeLab und für diverse Kunden im Praktikum

PBXWare: alternative VOIP-Telefonanlage im HomeLab zum Testen
