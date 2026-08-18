# Muhammad Dzul Arsyil

**Senior Mobile & Full-Stack Engineer** — 9+ years building and leading production software across mobile, web, backend, and infrastructure.

Based in Indonesia. Associate degree in Information Processing, Seifu Institute of Technology, Osaka.

Most repositories are private (client work). The projects below represent a selection of production systems I've architected and shipped.

---

## What I Do

Senior engineer and technical lead with 9+ years shipping production systems at scale — 1.4M members, volunteer platforms for 20+ campaigns, systems replacing apps with 1.5M installs. I architect and deliver complex, multi-platform products end-to-end: from Flutter and React Native mobile apps to NestJS and Laravel backends, PostgreSQL schemas, and cloud infrastructure. I've been building Flutter apps since 2019 (pre-null-safety through Riverpod and offline-first architectures), and equally comfortable across the full web and backend stack. I lead small focused teams, set architecture standards, and still write the hard code myself. 30+ projects shipped across government, political tech, healthcare, agriculture, and enterprise domains in Indonesia and Japan.

**Mobile**

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat&logo=flutter&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat&logo=expo&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-FA7343?style=flat&logo=swift&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Vue](https://img.shields.io/badge/Vue-4FC08D?style=flat&logo=vuedotjs&logoColor=white)
![Nuxt](https://img.shields.io/badge/Nuxt-00DC82?style=flat&logo=nuxtdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=flat&logo=reactquery&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

**Backend**

![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat&logo=laravel&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)

**Databases & Infra**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![Valkey](https://img.shields.io/badge/Valkey-FF4438?style=flat&logo=redis&logoColor=white)

---

## GitHub Stats

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=aru-shiru&theme=github_dark" />
</p>
<p align="center">
  <img src="https://ghchart.rshah.org/aru-shiru" alt="Contribution Graph" />
</p>

---

## Experience

**Technical Lead & Senior Full-Stack Engineer** — PT Lamacca Kreatif Solusi *(2018 – Present)*  
Software consultancy delivering custom digital products for Indonesian enterprises and government clients. Led engineering across 30+ projects — setting architecture standards, conducting code reviews, and contributing hands-on across mobile, web, backend, and infrastructure.

**Co-Founder & Full-Stack Engineer** — Belliki *(2016 – 2018)*  
Online marketplace for custom-designed apparel — customers design clothing using an interactive canvas tool (Fabric.js) or upload design files directly (CorelDraw, Photoshop), then choose their preferred printing vendor. Built the entire platform from scratch including the garment designer, marketplace, and vendor-side order and inventory management system.  
`Vue.js` `Node.js` `Fabric.js`

---

## Education

**Associate Degree in Information Processing**  
Seifu Institute of Technology, Osaka  
*Graduation project sCalendar (voice-recognition scheduler, UWP) recognised as one of two outstanding projects by Microsoft Japan representative.*

**Osaka Japanese Language Education Center** *(2013 – 2014)*

---

## Selected Projects

### e-Partai — Political Party Management System
> Full-stack platform for party membership, candidate management, and volunteer coordination — member registration, digital membership cards, and field volunteer trees.

- **1.4M** members in production · **50K+** Play Store installs
- Nx monorepo with 17 domain API modules and 8 apps (API, admin dashboard, mobile PWA, native mobile, CLI, migration tools, E2E suites)
- Functional error handling via `neverthrow` (Result types, zero try-catch) with concern-split repositories (Query / Mutation / List / Creator)
- CASL authorization + SuperTokens auth + Zod validation + event-driven audit logging via NestJS EventEmitter
- AI-powered analytics chatbot using Google Gemini with function-calling for natural-language queries on candidate and volunteer data
- Full-text search across members and volunteers, with voter registry lookup via a separate search API
- Queue-based async exports with XLSX generation and distributed locking via Valkey
- Migrated two legacy Firebase systems (simPAN + pantau-relawan) into this unified platform

`TypeScript` `NestJS` `PostgreSQL` `Drizzle ORM` `React` `TanStack Router` `Expo` `React Native` `Meilisearch` `Valkey` `SuperTokens` `CASL` `Nx`

---

### Narrative Phone — Healthcare Video Calling App
> Native iOS and Android video calling app for healthcare professionals and patients — enabling phone-style video calls integrated with the [ナラティブブック](https://www.narrativebook.jp) health communication platform.

- Led a team of two native developers (Kotlin + Swift); hands-on on both platforms, then owned both apps after they left
- Custom Zoom Video SDK meeting UI built with UIKit on iOS — replacing the default Zoom UI with a tailored in-call experience for healthcare use cases
- SwiftUI-based iOS app with UIKit integration for Zoom video components; Kotlin Android app with the equivalent feature set
- Contact management, call history, and integration with ナラティブブック's existing account and contact system
- REST API integration with client-provided Ruby on Rails backend

`SwiftUI` `UIKit` `Kotlin` `XML` `Zoom Video SDK` `Ruby on Rails`

---

### Pantau Relawan — Electoral Volunteer Management & Real-Time Vote Monitoring
> SaaS platform for political campaign volunteer management and real-time election monitoring, serving 20+ candidate organizations with dedicated apps and a shared basic plan.

- Nx monorepo (29 apps, 7 shared libraries) spanning Flutter mobile, React PWA, Vue.js admin dashboards, and Firebase Cloud Functions — with shared TypeScript/Dart library layer for cross-platform code reuse
- Single-handedly built and maintained the Flutter mobile app: Riverpod state management, offline-first architecture (SQLite + Firestore sync), go_router navigation
- Serverless backend with 25+ domain-driven Cloud Functions modules: auth, real-time vote counting, voter database management, survey analytics, and scheduled batch jobs
- Multi-candidate architecture with dynamic theming and tenant-scoped data isolation on a single Firestore instance

`Flutter` `Dart` `React` `Vue` `TypeScript` `Firebase` `Riverpod` `Zustand` `Pinia` `Nx` `SQLite`

---

### e-Watch LSI — Political Fieldwork Monitoring Platform
> Real-time field operations monitoring for a political survey/consulting firm — tracking canvassing activities, geotagged evidence, and survey responses across Indonesian election campaigns.

- **~500K** field submissions in the system · used by ~100 concurrent internal users
- Real-time election monitoring dashboard (Nuxt) with regional progress tracking, daily stats charts, and questionnaire response analytics
- Automated report generation pipeline: reverse-geocoding GPS coordinates via Google Maps API, static map snapshots, and field photo compositing (Puppeteer + Sharp)
- Custom auth issuing Firebase custom tokens with role-based claims — enabling field volunteers to log in without email accounts
- Real-time stats aggregation via Firestore triggers: every submission auto-updates per-user, per-region, and per-date counters with daily reset via Cloud Scheduler

**Flutter mobile app (field worker companion):**
- **Offline-first draft queue**: SQLite (`sqflite`) persists pending submissions with compressed image preview blobs; a reactive `QueueService` watches connectivity × auth × tenant providers and auto-resumes uploads to Firebase Storage + Firestore on reconnect — survives app restarts and process death
- Riverpod feature-sliced architecture across login, home, dropping, persuasi, and draft domains — one notifier per concern, cross-provider reactivity, with custom-token auth via Cloud Functions letting field workers log in with username/password (no email required)
- Multi-tenant single APK: same binary serves multiple client organizations; feature modules and dynamic questionnaires loaded per-tenant from Firestore, with dual-resolution image pipeline streamed through a `FormStatus` state machine

`Nuxt` `Vue` `TypeScript` `Firebase` `Google Maps API` `Puppeteer` `Sharp` `Nx` `Flutter` `Dart` `Riverpod` `SQLite` `sqflite` `Geolocator`

---

### SDS — Building Services Management Platform
> Full-stack facility management platform digitizing attendance, cleaning operations, recruitment, inventory, and ticketing across mobile and web.

- **2,000+** field employees using the app daily
- Sole engineer across mobile, web admin, backend, database design, and IoT device integration
- Cross-platform mobile app (React Native/Expo) with GPS-geofenced attendance check-in, camera capture, shift management, cleaning task tracking, and inventory transfers
- Supabase (PostgreSQL) with Row-Level Security policies, custom JWT hooks, and Edge Functions (Deno)
- Integrated physical fingerprint scanners by implementing the iClock protocol — bridging ZKTeco biometric devices to the cloud via Express/SQLite on Fly.io
- Nuxt Layers architecture for modular feature domains: attendance, employee management, recruitment pipeline, building management, and ticketing

`React Native` `Expo` `Nuxt` `Vue` `TypeScript` `Supabase` `PostgreSQL` `Firebase Cloud Functions` `CASL` `Zod` `Mapbox` `Fly.io` `Turborepo`

---

### SimplePol — Health Check Management System
> Full-stack web application managing health check workflows for Indonesian driving license applicants.

- Replacing a legacy system with **1.5M Play Store installs** and **~200K monthly health checks**
- Passwordless authentication via magic link flow (Laravel Fortify) — no traditional password storage
- AI-powered KTP (national ID card) OCR and fraud detection using Google Gemini API
- Role-based access for doctors, health workers, registration agents, police officers, and administrators
- Spec-driven development with comprehensive Pest test coverage (feature + browser tests via Playwright)
- Change history auditing, soft-delete policies, and strict relational integrity on PostgreSQL

`Laravel` `Livewire` `PHP` `PostgreSQL` `Tailwind CSS` `Google Gemini API` `Pest` `Docker`

---

### ADV Live — Agricultural Sales Force Automation
> Sales force automation platform for an agribusiness in Indonesia and Malaysia — managing field sales operations, supply chain tracking, and farmer engagement.

- Indonesia live since 2021: **50K+** sales records · **~100K** tracked field activities · 100+ internal users
- Adopted by Malaysia HQ on the same product, with local geography, catalog, and language
- Led a team across the full stack: architecture decisions, code reviews, and hands-on contribution across mobile, admin dashboard, backend, and infrastructure
- Offline-first React Native mobile app (Expo) with GPS-stamped field logging, fake location detection, and background sync queues for low-connectivity rural areas
- Supply chain management with distributor/retailer stock tracking and automated inventory deductions linked to sales transactions

`React Native` `Expo` `Nuxt` `TypeScript` `NestJS` `PostgreSQL` `Firebase` `Google Maps API` `TanStack Query` `CASL` `Turborepo`

---
