# inertia-native-android

> Inertia Native Android (Kotlin/AndroidX) library: single shared WebView across fragment destinations, AndroidX Navigation, path config, bridge components.

📋 **Part of the [Inertia Native](https://github.com/users/SteveCrickmar/projects/4) project** — an open-source toolkit for shipping native iOS & Android apps powered by an existing Laravel + Inertia.js application, modelled on (but not depending on) Hotwire Native. Track the cross-repo roadmap on the **[project board](https://github.com/users/SteveCrickmar/projects/4)**.

### Repositories in the Inertia Native project
- **[inp-protocol](https://github.com/SteveCrickmar/inp-protocol)** — spec, JSON Schemas, conformance fixtures, ADRs, and the M0 spike. Coordination point for all Inertia Native repos
- **[inertia-native-adapter](https://github.com/SteveCrickmar/inertia-native-adapter)** — visit interception, screen page-cache & restore, lifecycle reporting, bridge transport
- **[inertia-native-ios](https://github.com/SteveCrickmar/inertia-native-ios)** — Navigator, shared WKWebView + snapshot cache, path configuration, bridge components, native error/auth/recovery. Models Hotwire Native iOS; zero Turbo dependency
- **inertia-native-android** ⬅ _this repo_
- **[inertia-native-laravel](https://github.com/SteveCrickmar/inertia-native-laravel)** — native detection & macros, shared props, signal routes & helpers, path-config authoring/serving, scaffolding & test helpers
- **[inertia-native-demo](https://github.com/SteveCrickmar/inertia-native-demo)** — one Laravel 12 app with switchable React & Vue front ends exercising every feature; error-injection harness; doubles as docs example and UI-test target
- **[inertia-native-docs](https://github.com/SteveCrickmar/inertia-native-docs)** — quick start, navigation, path configuration, signals, bridge components, native screens, auth, protocol reference

## Project documents
- [PRD](https://github.com/SteveCrickmar/inp-protocol/blob/main/docs/01-prd-inertia-native.md)
- [Technical Specification](https://github.com/SteveCrickmar/inp-protocol/blob/main/docs/02-technical-spec-inertia-native.md) (normative)
- [Task Breakdown](https://github.com/SteveCrickmar/inp-protocol/blob/main/docs/03-task-breakdown.md)

## Toolchain baseline (OC-8)
AGP current LTS, Kotlin 2.x, minSdk 26, JUnit5 + Robolectric + Espresso, ktlint.

## Working conventions
- **OC-1:** one task → one branch (`task/<ID>-slug`) → one PR; no task touches more than one repo.
- **OC-3:** the [protocol spec](https://github.com/SteveCrickmar/inp-protocol) is law. Conformance fixtures are vendored read-only at the ref in `INP_SPEC_REF`.
- See the [task breakdown](https://github.com/SteveCrickmar/inp-protocol/blob/main/docs/03-task-breakdown.md) §0 for the full operating conventions and Definition of Done (OC-2).

## Tasks tracked in this repo
- **N7.1** — Repo scaffold
- **N7.2** — Session & channel
- **N7.3** — ScreenFragment, re-parenting, SnapshotCache
- **N7.4** — Navigator, back handling, modal model
- **N7.5** — PathConfig, policy layer, errors & recovery
- **N7.6** — Bridge registry + reference components
- **N7.7** — Conformance + Espresso suite
- **N7.8** — Scaffolding (android) + beta train
- **X1-android** — Debug overlay (message inspector) toggle in Harness apps

## Status
Pre-alpha. Names are placeholders pending a trademark check (OC-6). Licensed MIT (proposed).
