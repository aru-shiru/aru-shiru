# Muhammad Dzul Arsyil

**Senior Full-Stack Engineer** — 9+ years building and leading production software across mobile, web, backend, and infrastructure.

Based in Indonesia. Associate degree in Information Processing, Seifu Institute of Technology, Osaka.

Most repositories are private (client work). The projects below represent a selection of production systems I've architected and shipped.

---

## What I Do

I lead small teams and build complex, multi-platform systems end-to-end — from database schema and backend architecture to mobile apps and admin dashboards. I've shipped 30+ projects across agriculture, facility management, government, political consulting, and civic tech in Indonesia.

**Mobile** — Flutter, React Native / Expo  
**Frontend** — React, Next.js, Vue, Nuxt, TanStack Router/Query  
**Backend** — NestJS, Laravel, Firebase Cloud Functions, Supabase Edge Functions  
**Databases** — PostgreSQL (Drizzle ORM, Supabase), Firestore, SQLite  
**Infra & Tooling** — Nx, Turborepo, Meilisearch, Valkey, S3/GCS/MinIO, Fly.io, Docker  
**Auth & Access** — CASL, SuperTokens, Firebase Auth, Laravel Fortify  

---

## Selected Projects

### e-Partai — Political Party Management System
> Full-stack platform managing the complete Indonesian election lifecycle — member registration, candidate management, volunteer coordination, polling station observer placement, and real-time vote tabulation.

- **1.6M** registered members and volunteers · **50K+** Play Store installs · **~1–2K** daily active users
- Nx monorepo with 15 domain API modules and 8 apps (API, admin dashboard, mobile PWA, native mobile, CLI, migration tools, E2E suites)
- Functional error handling via `neverthrow` (Result types, zero try-catch) with concern-split repositories (Query / Mutation / List / Creator)
- CASL authorization + SuperTokens auth + Zod validation + event-driven audit logging via NestJS EventEmitter
- AI-powered analytics chatbot using Google Gemini with function-calling for natural-language queries on candidate and volunteer data
- Dual Meilisearch instances for full-text search across user and voter registry (DPT) data
- Queue-based async exports with PostgreSQL-backed job queue, XLSX generation, and distributed locking via Valkey
- Migrated two legacy Firebase systems (simPAN + pantau-relawan) into this unified platform

`TypeScript` `NestJS` `PostgreSQL` `Drizzle ORM` `React` `TanStack Router` `Expo` `React Native` `Meilisearch` `Valkey` `SuperTokens` `CASL` `Nx`

---

### Pantau Relawan — Electoral Volunteer Management & Real-Time Vote Monitoring
> SaaS platform for political campaign volunteer management and real-time election monitoring, serving 18+ candidate organizations simultaneously with per-candidate isolated deployments.

- **~300K** registered volunteers · **40** concurrent client organizations across dedicated apps and PWAs
- Nx monorepo (29 apps, 7 shared libraries) spanning Flutter mobile, React PWA, Vue.js admin dashboards, and Firebase Cloud Functions — with shared TypeScript/Dart library layer for cross-platform code reuse
- Single-handedly built and maintained the Flutter mobile app: Riverpod state management, offline-first architecture (SQLite + Firestore sync), go_router navigation
- Serverless backend with 25+ domain-driven Cloud Functions modules: auth, real-time vote counting, voter database management, survey analytics, and scheduled batch jobs
- Multi-candidate architecture with dynamic theming and tenant-scoped data isolation on a single Firestore instance (30+ collections, 8,800+ composite indexes)

`Flutter` `Dart` `React` `Vue` `TypeScript` `Firebase` `Riverpod` `Zustand` `Pinia` `Nx` `SQLite`

---

### e-Watch LSI — Political Fieldwork Monitoring Platform
> Real-time field operations monitoring for a political survey/consulting firm — tracking canvassing activities, geotagged evidence, and survey responses across Indonesian election campaigns.

- **~500K** field submissions in the system · used by ~100 concurrent internal users
- Real-time election monitoring dashboard (Nuxt) with regional progress tracking, daily stats charts, and questionnaire response analytics
- Automated report generation pipeline: reverse-geocoding GPS coordinates via Google Maps API, static map snapshots, and field photo compositing (Puppeteer + Sharp)
- Custom auth issuing Firebase custom tokens with role-based claims — enabling field volunteers to log in without email accounts
- Real-time stats aggregation via Firestore triggers: every submission auto-updates per-user, per-region, and per-date counters with daily reset via Cloud Scheduler

`Nuxt` `Vue` `TypeScript` `Firebase` `Mapbox GL` `Google Maps API` `Puppeteer` `Sharp` `Turborepo`

---

### Advansia — Agricultural Sales Force Automation
> Sales force automation platform for an Indonesian agribusiness company — managing field sales operations, supply chain tracking, and farmer engagement.

- **50K+** sales records · **~100K** tracked field activities · 100+ internal users
- Led a team across the full stack: architecture decisions, code reviews, and hands-on contribution across mobile, admin dashboard, backend, and infrastructure
- Offline-first React Native mobile app (Expo) with GPS-stamped field logging, fake location detection, and background sync queues for low-connectivity rural areas
- 17 independent Firebase Cloud Functions microservices: transactions, inventory, employee management, reporting, and data exports
- Supply chain management with distributor/retailer stock tracking and automated inventory deductions linked to sales transactions

`React Native` `Expo` `Next.js` `TypeScript` `Firebase` `Google Maps API` `TanStack Query` `CASL` `Turborepo`

---

### SDS — Building Services Management Platform
> Full-stack facility management platform digitizing attendance, cleaning operations, recruitment, inventory, and ticketing across mobile and web.

- **1,000+** field employees using the app daily
- Led a team across mobile, web admin, backend, database design, and IoT device integration
- Cross-platform mobile app (React Native/Expo) with GPS-geofenced attendance check-in, camera capture, shift management, cleaning task tracking, and inventory transfers
- Supabase (PostgreSQL) with 80+ migrations, Row-Level Security policies, custom JWT hooks, and Edge Functions (Deno)
- Integrated physical fingerprint scanners by implementing the iClock protocol — bridging ZKTeco biometric devices to the cloud via Express/SQLite on Fly.io
- Nuxt Layers architecture for modular feature domains: attendance, employee management, recruitment pipeline, building management, real-time ticketing

`React Native` `Expo` `Nuxt` `Vue` `TypeScript` `Supabase` `PostgreSQL` `Firebase Cloud Functions` `CASL` `Zod` `Mapbox` `Fly.io` `Turborepo`

---

### SimplePol — Health Check Management System
> Full-stack web application managing health check workflows for Indonesian driving license applicants.

- Replacing a legacy system with **1.5M Play Store installs** and **~200K monthly health checks**
- Passwordless authentication via magic link flow (Laravel Fortify) — no traditional password storage
- AI-powered KTP (national ID card) OCR and fraud detection using Google Gemini API
- Role-based multi-tenant architecture supporting 5 distinct user roles with dedicated dashboards and middleware-enforced access control
- Spec-driven development with comprehensive Pest test coverage (feature + browser tests via Playwright)
- 24 Eloquent models with soft-delete policies, change history auditing, and strict relational integrity

`Laravel` `Livewire` `PHP` `Tailwind CSS` `Google Gemini API` `SQLite` `Pest` `Docker`

---

### e-Hibah Polri — Grant Management System, Indonesian National Police
> Full-stack grant lifecycle platform for the Indonesian National Police managing proposals, agreements, budget planning, fund withdrawals, and document workflows across a three-tier organizational hierarchy.

- Multi-level approval workflows with TOTP 2FA and granular authorization policies per organizational tier
- Comprehensive audit trail: change history tracking, activity logging, and soft-delete policies aligned to data retention requirements
- Led full platform rewrite from Laravel 11 + Inertia.js + React to a Livewire-based architecture, eliminating the JS build pipeline for most features while preserving UI interactivity

`Laravel` `Livewire` `PHP` `PostgreSQL` `Tailwind CSS` `Alpine.js` `Laravel Fortify` `Pest` `Docker`

---

### ナラティブフォン — Healthcare Video Calling App
> Native iOS and Android video calling app for healthcare professionals and patients — enabling phone-style video calls integrated with the [ナラティブブック](https://www.narrativebook.jp) health communication platform.

- Led a team of two native developers (Kotlin + Swift); responsible for code reviews on both platforms and hands-on contribution on the iOS app
- Custom Zoom Video SDK meeting UI built with UIKit on iOS — replacing the default Zoom UI with a tailored in-call experience for healthcare use cases
- SwiftUI-based iOS app with UIKit integration for Zoom video components; Kotlin/XML-based Android app with equivalent feature set
- Contact management with QR code exchange, call history, and integration with ナラティブブック's existing account and contact system
- REST API integration with client-provided Ruby on Rails backend

`SwiftUI` `UIKit` `Kotlin` `XML` `Zoom Video SDK` `Ruby on Rails`

---

## Experience

**Technical Lead & Senior Full-Stack Engineer** — PT Lamacca Kreatif Solusi *(2018 – Present)*  
Led a team of developers across 30+ client projects over 9+ years. Responsible for architecture decisions, technical standards, code reviews, and hands-on contribution across mobile, web, backend, database, and infrastructure.

---

## Education

**Associate Degree in Information Processing**  
Seifu Institute of Technology, Osaka

---
