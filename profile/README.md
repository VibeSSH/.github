# VibeSSH

<p align="center">
  <img src="https://raw.githubusercontent.com/VibeSSH/.github/main/profile/vibessh-dashboard.png"
       alt="The VibeSSH dashboard: two nodes with live CPU and memory, and the applications running on them"
       width="880">
</p>

**Run your Linux servers from a desktop app. Nothing to host, no panel to maintain.**

VibeSSH is a desktop application for Windows and Linux that manages Linux
machines over plain SSH — and the things you actually run on them: Minecraft
servers, databases, bots. You install it on your own computer. You do not
install anything on the server to make it work, and you never expose another
web service just to administer one.

No domain. No SSL certificate. No nginx. No hosted panel.

## What it does

**Servers.** SSH with tabbed terminals, an SFTP file browser with an editor,
live metrics and processes, systemd and Docker actions, and temporary port
forwards.

**Applications.** A server, a database or a bot managed as one unit rather
than as a pile of shell commands — started, stopped, backed up, with its own
files, ports, environment and logs. Fourteen blueprints ship with it: Paper,
Purpur, Velocity, Waterfall, MariaDB, MongoDB, Redis, NATS, phpMyAdmin,
Node.js and Python bots, and generic ones for anything else. They run as
Docker containers, systemd units, or plain processes — including on your own
machine, where nothing needs installing at all.

**Vibe Network.** A private WireGuard mesh between your nodes, with DNS names
for applications, so one server reaches another without publishing a port to
the internet.

**Firewall.** ufw rules follow from the ports you chose to publish — including
the container traffic that ufw alone silently fails to filter, which is the
usual reason a "closed" port is open.

**Backups.** Application directories, by hand or on a schedule, kept locally
and optionally uploaded to S3, Cloudflare R2 or MinIO.

**Migration from Pterodactyl.** Servers move across with their files and
configuration.

**Vibe AI.** Answers questions about *your* servers, grounded in the built-in
guide, using an API key you provide.

## Get it

Windows installer, AppImage, `.deb` and `.tar.gz`:
[**latest release**](https://github.com/VibeSSH/vibessh-releases/releases/latest)

Site and documentation: [**vibessh.dev**](https://vibessh.dev)

## Do I need an account?

No. Nodes, applications, files, the terminal, the firewall and backups all
work without signing in to anything.

An account exists only for teams and shared servers, and the backend behind it
is one you run yourself — VibeSSH operates no account service, and your
credentials never leave your machine. SSH passwords and key passphrases live
in the operating system's own credential store, never in a configuration file.

## Status

Public beta, released regularly. Licensed under AGPL-3.0.
