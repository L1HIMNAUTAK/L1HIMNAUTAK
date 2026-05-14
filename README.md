<!--
  GitHub Profile README — Mike Gonzales
  Save this as `README.md` in a repo named EXACTLY the same as your GitHub username.
  That special repo turns into your profile landing page.

  TODO before publishing:
  - Replace `L1HIMNAUTAK` with your actual GitHub handle (search the file).
  - Replace contact links (email, LinkedIn) with your preferred public ones.
  - Adjust the experience years / metrics if any number doesn't match.
-->

<h1 align="center">Mike Gonzales</h1>

<p align="center">
  <em>Senior Software Engineer &nbsp;·&nbsp; Network &amp; Infrastructure Engineer</em>
</p>

<p align="center">
  <a href="mailto:mike.gonzales@lkygroup.com">
    <img src="https://img.shields.io/badge/email-mike.gonzales%40lkygroup.com-0a66c2?style=flat-square&logo=microsoftoutlook&logoColor=white" alt="Email" />
  </a>
  <a href="https://lkygroup.com">
    <img src="https://img.shields.io/badge/Company-LKY%20Group-0f172a?style=flat-square" alt="Company" />
  </a>
  <a href="https://github.com/L1HIMNAUTAK?tab=followers">
    <img src="https://img.shields.io/github/followers/L1HIMNAUTAK?label=Followers&style=flat-square&color=0a66c2" alt="Followers" />
  </a>
</p>

---

## About

Full-stack software engineer and network/infrastructure architect at **LKY Group**, where I lead the design and operation of internal business systems and the network plumbing that supports them. My work spans the entire delivery lifecycle: requirements, system architecture, application development, deployment, hardening, monitoring, and on-call recovery.

I am most effective at the intersection of software and infrastructure — building Laravel and Flutter applications and the multi-tenant, segmented networks, virtualization clusters, and edge-routing setups they run on.

---

## Core Competencies

| Software Engineering | Network &amp; Infrastructure |
|---|---|
| Full-stack web application design (Laravel, Livewire, Filament) | Multi-host Proxmox VE clustering and LXC/VM provisioning |
| Cross-platform mobile development with Flutter | MikroTik RouterOS firewall, VLAN segmentation, and queue trees |
| Relational database design (PostgreSQL, MySQL) | Cisco IOS access-layer configuration |
| API design, authentication, and version-gated mobile release pipelines | Cloudflare Zero Trust tunnels and DNS automation |
| UI/UX systems with Tailwind CSS and design-token discipline | Server hardening (fail2ban, UFW, SSH key-only, kernel tuning) |
| CI-style release tooling, idempotent shell automation | Synology NAS deployment, CIFS/NFS integration, and backup strategy |

---

## Featured Projects

### IMS — Inventory Management System
Internal Laravel 11 application for inventory, transactions, and operations across LKY Group properties. Designed around thin controllers, Form Request validation, route model binding, and a service/action layer for business logic. Tailwind + Alpine UI with strict accessibility and responsive-first layout.

**Stack:** Laravel 11 · PHP 8.2 · MySQL · Livewire · Tailwind CSS · Alpine.js · Vite

### TMS — Transport Management System
End-to-end transport platform combining a Laravel server, client application, and Raspberry Pi–based vehicle barrier controllers at entry/exit gates. Real-time gate operations, PostgreSQL backing store accessed through an SSH-tunneled jump host, and Cloudflare-fronted production endpoints.

**Stack:** Laravel · Docker · PostgreSQL · Raspberry Pi · Cloudflare Tunnel · Debian

### HRIS — HR Information System &amp; Mobile App
Laravel 12 + PostgreSQL HR platform with PgBouncer pooling, twelve scheduled jobs, and a companion Flutter mobile app distributed through an internal APK portal at `apk.lky.systems`. Built a one-command release pipeline (`release-apk.sh`) that bumps the pubspec, builds the APK, uploads to a Synology share, registers the release in the database, and verifies the version-check API — gating clients via `force_update` and `min_required_version` flags.

**Stack:** Laravel 12 · PHP 8.2 · PostgreSQL 17 · PgBouncer · Flutter · Dart · Redis

### BioServer — ZKTeco Biometric Attendance Management
Internal Laravel/Blade application that ingests biometric punches from ZKTeco devices and surfaces attendance, scheduling, and exception reporting for LKY Group operations. _Private repository._

**Stack:** Laravel · PHP · Blade · MySQL

### Hotel Management System (in design)
Four-phase, ~110-table system covering reservations, front office, housekeeping, F&amp;B, and back-office accounting for hotel operations under the LKY Group portfolio. Currently in architectural planning.

**Stack (planned):** Laravel · PostgreSQL · Livewire · Filament

### WordPress Estate — Multi-Tenant Hosting
Operates several production WordPress properties across two Proxmox hosts, each fronted by its own Cloudflare Tunnel and reverse-proxy stack:
`theorientalhotels.com`, `lkygroup.com`, `mwx.systems`, `wtl.lky.systems`, `lky.systems`, `apk.lky.systems`.
Includes a multisite migration from shared cPanel hosting to fully Dockerized WordPress on dedicated infrastructure.

**Stack:** nginx · php-fpm 8.3/8.4 · MySQL · Docker · Dockge · Cloudflare Tunnel

---

## Open-Source Utilities

Small, focused PowerShell tools for Windows administrators:

- **[StartIsBack-Reset-Script](https://github.com/L1HIMNAUTAK/StartIsBack-Reset-Script)** — Fully resets StartIsBack and cleans all traces, registry keys, and CLSIDs for a clean uninstall or fresh start.
- **[AnyDesk-Reset-Script](https://github.com/L1HIMNAUTAK/AnyDesk-Reset-Script)** — Resets AnyDesk settings, removes traces, and restores it to a fresh state for troubleshooting or clean reinstalls.

---

## Technical Stack

**Languages &amp; Runtimes**
PHP 8.2 / 8.4 · Dart · Bash · Python · SQL

**Backend Frameworks**
Laravel 11 / 12 · Livewire 3 · Filament 3

**Frontend**
Tailwind CSS 3.4+ · Alpine.js 3 · Blade · Vite · Heroicons / Lucide

**Mobile**
Flutter 3.x · Dart · Android Studio

**Databases &amp; Caching**
PostgreSQL 17 · PgBouncer · MySQL 8 · Redis · SQLite

**Infrastructure &amp; Virtualization**
Proxmox VE 8 · LXC · Docker · Dockge · nginx · Apache · code-server · FileBrowser

**Networking**
MikroTik RouterOS 7 · Cisco IOS · VLAN · WireGuard · L2TP/IPsec · Cloudflare Zero Trust · Cloudflare API automation

**Operating Systems**
Debian 12 / 13 · Ubuntu LTS · Synology DSM · Windows Server

**Tooling &amp; Practices**
Git · Composer · PHPUnit · Laravel Pint · PSR-12 · Form Requests · Service / Action layer · API Resources · Eager loading · Index discipline · CSRF · Route model binding

---

## Selected Engineering Highlights

- **Internal APK distribution portal (`apk.lky.systems`)** — Designed a three-tier delivery chain (Cloudflare Tunnel → LXC nginx + FileBrowser → Synology CIFS) with scoped FileBrowser users, autoindex-backed JSON listings, and a custom Tailwind/Alpine landing page consuming the listing directly.
- **One-command Flutter release pipeline** — Built an idempotent shell pipeline that bumps `pubspec.yaml`, runs `flutter build apk --release`, uploads to a Synology share, registers the release in PostgreSQL via a transient PHP boot script, and smoke-tests the version-check endpoint before committing.
- **Cross-host production migration** — Moved `lkygroup.com` from shared cPanel hosting to a dedicated, Dockerized stack on a new Proxmox host, with staging URL, DNS cut-over, and rollback path.
- **Post-incident infrastructure right-sizing** — Recovered HRIS Staging and TMS Production after a Proxmox over-provisioning event, then re-baselined LXC CPU/RAM allocations across two PVE hosts to fit measured workload (e.g. WordPress nodes capped at 2–4 cores / 2–4 GB).
- **Cloudflare Tunnel ingress automation** — Manages tunnel ingress rules and DNS via the Cloudflare API rather than the dashboard, enabling reproducible domain on-boarding (`apk.lky.systems`, `wtl.lky.systems`, and others).
- **Network segmentation and hardening** — VLAN-isolated management, server, user, IoT, and guest networks with default-deny firewall policies; SSH key-only access, fail2ban on public-facing services, and SNMPv3 management.
- **Resilience tooling** — Watchdog timers and post-reboot ordering fixes for services that historically failed after host restarts (nginx network-race, code-server heap leak, Redis AOF corruption recovery).

---

## Working Style

- **Documentation-driven** — every shipped module has a `docs/` entry (modules, features, API, database, testing, deployment).
- **Thin controllers, fat services** — business logic lives in services and actions, not controllers.
- **Accessibility &amp; performance first** — WCAG-AA contrast, semantic HTML, keyboard navigation, lazy loading, and pagination are non-negotiable defaults.
- **Backup before change** — every infrastructure change is preceded by a verified backup and followed by a 48-hour monitoring window.
- **Least privilege** — default-deny firewalls, scoped service accounts, segregated VLANs, and SSH key rotation.

---

## Contact

- **Email:** [mike.gonzales@lkygroup.com](mailto:mike.gonzales@lkygroup.com)
- **Company:** [LKY Group](https://lkygroup.com)
- **GitHub:** [@L1HIMNAUTAK](https://github.com/L1HIMNAUTAK)

<sub>Open to discussing engineering, infrastructure, and platform problems — particularly where software and network design meet.</sub>
