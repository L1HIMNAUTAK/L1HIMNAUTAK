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

#### Languages &amp; Runtimes
![PHP](https://img.shields.io/badge/PHP-8.4-777BB4?style=flat-square&logo=php&logoColor=white)
![C#](https://img.shields.io/badge/C%23-12-239120?style=flat-square&logo=csharp&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-3.x-0175C2?style=flat-square&logo=dart&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES2024-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-7-5391FE?style=flat-square&logo=powershell&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-5-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Standard-336791?style=flat-square&logo=postgresql&logoColor=white)

#### Backend Frameworks
![Laravel](https://img.shields.io/badge/Laravel-12-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET](https://img.shields.io/badge/ASP.NET-Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Livewire](https://img.shields.io/badge/Livewire-3-4E56A6?style=flat-square&logo=livewire&logoColor=white)
![Filament](https://img.shields.io/badge/Filament-3-F59E0B?style=flat-square&logo=laravel&logoColor=white)

#### Frontend
![Blade](https://img.shields.io/badge/Blade-Templating-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Alpine.js](https://img.shields.io/badge/Alpine.js-3-8BC0D0?style=flat-square&logo=alpinedotjs&logoColor=black)
![Heroicons](https://img.shields.io/badge/Heroicons-2-7C3AED?style=flat-square)
![Lucide](https://img.shields.io/badge/Lucide-Icons-F56565?style=flat-square&logo=lucide&logoColor=white)

#### Mobile
![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?style=flat-square&logo=flutter&logoColor=white)
![Android Studio](https://img.shields.io/badge/Android%20Studio-2024-3DDC84?style=flat-square&logo=androidstudio&logoColor=white)

#### Databases &amp; Caching
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17-336791?style=flat-square&logo=postgresql&logoColor=white)
![PgBouncer](https://img.shields.io/badge/PgBouncer-pooler-336791?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-MSSQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-7-DC382D?style=flat-square&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-3-003B57?style=flat-square&logo=sqlite&logoColor=white)

#### Infrastructure &amp; Virtualization
![Proxmox VE](https://img.shields.io/badge/Proxmox%20VE-8-E57000?style=flat-square&logo=proxmox&logoColor=white)
![LXC](https://img.shields.io/badge/LXC-Containers-323330?style=flat-square&logo=linuxcontainers&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Engine-2496ED?style=flat-square&logo=docker&logoColor=white)
![Dockge](https://img.shields.io/badge/Dockge-UI-2496ED?style=flat-square)
![nginx](https://img.shields.io/badge/nginx-Reverse%20Proxy-009639?style=flat-square&logo=nginx&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-HTTPd-D22128?style=flat-square&logo=apache&logoColor=white)
![Synology](https://img.shields.io/badge/Synology-DSM-11225E?style=flat-square&logo=synology&logoColor=white)

#### Networking &amp; Security
![MikroTik](https://img.shields.io/badge/MikroTik-RouterOS%207-293239?style=flat-square&logo=mikrotik&logoColor=white)
![Cisco](https://img.shields.io/badge/Cisco-IOS-1BA0D7?style=flat-square&logo=cisco&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-Zero%20Trust-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![WireGuard](https://img.shields.io/badge/WireGuard-VPN-88171A?style=flat-square&logo=wireguard&logoColor=white)
![fail2ban](https://img.shields.io/badge/fail2ban-IPS-D32F2F?style=flat-square)
![UFW](https://img.shields.io/badge/UFW-Firewall-DD4814?style=flat-square&logo=ubuntu&logoColor=white)

#### Operating Systems
![Debian](https://img.shields.io/badge/Debian-12%2F13-A81D33?style=flat-square&logo=debian&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-LTS-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-2019%2F2022-0078D6?style=flat-square&logo=windows&logoColor=white)
![Windows 11](https://img.shields.io/badge/Windows-11-0078D6?style=flat-square&logo=windows11&logoColor=white)

#### Tooling &amp; Practices
![Git](https://img.shields.io/badge/Git-SCM-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-SCM-181717?style=flat-square&logo=github&logoColor=white)
![Composer](https://img.shields.io/badge/Composer-PHP-885630?style=flat-square&logo=composer&logoColor=white)
![NuGet](https://img.shields.io/badge/NuGet-.NET-004880?style=flat-square&logo=nuget&logoColor=white)
![PHPUnit](https://img.shields.io/badge/PHPUnit-Testing-366488?style=flat-square)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-2022-5C2D91?style=flat-square&logo=visualstudio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-Editor-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)

> **Engineering practices**: PSR-12 · Form Requests · Service / Action layer · Route Model Binding · API Resources · Eager Loading · Index discipline · CSRF · Default-deny firewalls · Backup-before-change · Least privilege

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
