<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=220&section=header&text=Vastavik&fontSize=80&fontColor=ffffff&fontAlignY=35&desc=One%20Product.%20Every%20Platform.%20Built%20by%20Parth.&descSize=20&descAlignY=55&descColor=ffffff" width="100%"/>

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&pause=1000&color=00D9FF&center=true&vCenter=true&width=600&lines=Flutter+%7C+Electron+%7C+Web+%7C+Android;Cross-platform+%E2%9A%A1+Single+Codebase+%F0%9F%9A%80;Built+with+%E2%9D%A4%EF%B8%8F+by+Parth+Vastavik)](https://github.com/parthasdey2304)

<p align="center">
  <a href="https://github.com/parthasdey2304"><img src="https://img.shields.io/badge/Maintained%20by-Parth%20Vastavik-00D9FF?style=for-the-badge&logo=github&logoColor=white" alt="Maintainer"/></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-7C3AED?style=for-the-badge&logo=open-source-initiative&logoColor=white" alt="License"/></a>
  <a href="#-platforms"><img src="https://img.shields.io/badge/Platforms-5-10B981?style=for-the-badge&logo=android&logoColor=white" alt="Platforms"/></a>
  <a href="#-tech-stack"><img src="https://img.shields.io/badge/Tech-6+-F59E0B?style=for-the-badge&logo=flutter&logoColor=white" alt="Tech"/></a>
</p>

<p align="center">
  <a href="https://instagram.com/vastavik_parth"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://linkedin.com/in/sarathiparth"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://twitter.com/vastavik__parth"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/></a>
  <a href="https://100-days-of-code-git-main-parthasarathidey.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white"/></a>
</p>

</div>

---

## ✨ Overview

**Vastavik** is a unified, cross-platform application suite that delivers a single product experience across **iOS, Android, Web, macOS, Windows, and Linux**. Built with a focus on performance, design consistency, and developer experience, Vastavik is engineered so that the same product, the same code philosophy, and the same user journey work everywhere.

> *"One codebase. Five platforms. Zero compromise."*

This repository is the home of the **Vastavik** organisation — the umbrella under which all client applications live and evolve together.

---

## 📱 Supported Platforms

<div align="center">

| Platform | Stack | Target |
|:---:|:---:|:---:|
| 📱 **iOS** | Flutter | iPhone & iPad |
| 📱 **Android** | Kotlin | Android Phone and Tablet |
| 🌐 **Web** | Modern Web (React/Next.js) | All Browsers |
| 🖥️ **Desktop** | Electron.js | macOS · Windows · Linux |

</div>

---

## 🧩 Applications

### 🍎 iOS App — Flutter
A native-feeling **iOS application** built with **Flutter**, delivering smooth animations, pixel-perfect UI, and full access to the Apple ecosystem.

- Built with **Dart + Flutter SDK**
- Optimised for iPhone and iPad
- Cupertino-styled components where it matters
- Offline-first architecture
- Push notifications & deep linking ready

### 🤖 Android App — Kotlin
A **native Android application** built with **Kotlin**, bringing the Vastavik experience to the world's most widely-used mobile platform with a true Material You feel.

- Built with **Kotlin** on **Android Studio**
- Targets **Android Phones and Tablets** (phones & form-factor tablets)
- **Material 3** design with dynamic colour theming
- **Jetpack Compose** UI for modern, declarative rendering
- **Kotlin Coroutines + Flow** for reactive async work
- **Room / DataStore** for offline-first persistence
- **Hilt** for dependency injection
- **Retrofit + OkHttp** for networking
- Adapts seamlessly across phone, foldables, and tablets

### 🌐 Web App
A blazing-fast, SEO-friendly **web application** that mirrors the mobile experience on the open web.

- Responsive design — mobile, tablet, desktop
- PWA-ready for installable experiences
- Server-side rendering for performance
- Accessible (WCAG-conscious) markup

### ⚛️ Desktop App — Electron.js
A **cross-platform desktop application** built with **Electron.js**, distributing native binaries for **macOS, Windows, and Linux** from a single codebase.

- Single codebase, three operating systems
- Auto-updates out of the box
- Native menus, tray icons, and OS-level integrations
- Signed installers for every platform

### 🐱 Catalan (CataLà)
The **Catalan-language** variant of the product — a first-class citizen, not an afterthought. This module ships locale-specific resources, translations, and culturally appropriate UX for Catalan speakers.

- `ca-ES` locale bundle
- Catalan-first copy and content
- Region-aware date, number, and currency formatting
- Maintained alongside the primary language tracks

---

## 🏗️ Architecture

```
┌──────────────────────────────────────────────────────────────────┐
│                       VASTAVIK  PLATFORM                         │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│   ┌──────────────┐  ┌──────────────┐  ┌──────────────┐           │
│   │  Flutter App │  │ Kotlin App   │  │   Web App    │           │
│   │    (iOS)     │  │  (Android)   │  │  (Browser)   │           │
│   └──────┬───────┘  └──────┬───────┘  └──────┬───────┘           │
│          │                 │                 │                   │
│          │          ┌──────┴───────┐         │                   │
│          │          │ Electron App │         │                   │
│          │          │ mac/Win/Lin  │         │                   │
│          │          └──────┬───────┘         │                   │
│          │                 │                 │                   │
│          └─────────────────┼─────────────────┘                   │
│                            ▼                                     │
│                  ┌────────────────────┐                          │
│                  │   Shared Core API  │                          │
│                  │   + Design System  │                          │
│                  └─────────┬──────────┘                          │
│                            ▼                                     │
│                  ┌────────────────────┐                          │
│                  │  Backend Services  │                          │
│                  └────────────────────┘                          │
│                                                                  │
│   ┌────────────────────────────────────────────────────┐         │
│   │  Locales:  en · ca (Català) · es · +more            │         │
│   └────────────────────────────────────────────────────┘         │
└──────────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|:---|:---|
| 📱 iOS Mobile | Flutter · Dart |
| 🤖 Android Mobile | Kotlin · Jetpack Compose · Coroutines |
| 🌐 Web | React / Next.js · TypeScript |
| 🖥️ Desktop | Electron.js · Node.js |
| 🎨 Design | Figma · Material 3 · Cupertino |
| 🌍 i18n | Flutter intl · i18next · Android string resources |
| ⚙️ Build | Vite · Webpack · electron-builder · Gradle |
| 🧪 Testing | Jest · Flutter Test · Playwright · JUnit · Espresso |
| 📦 CI/CD | GitHub Actions |

</div>

---

## 🚀 Getting Started

### Prerequisites
- **Node.js** ≥ 18
- **Flutter** ≥ 3.16
- **JDK** ≥ 17 (for Android / Kotlin builds)
- **Android Studio** (with Android SDK & emulator)
- **Git**

### Clone
```bash
git clone https://github.com/parthasdey2304/vastavikCodingStuff.git
cd vastavikCodingStuff
```

### Run the Web App
```bash
cd web
npm install
npm run dev
```

### Run the iOS App (Flutter)
```bash
cd mobile
flutter pub get
flutter run
```

### Run the Android App (Kotlin)
```bash
cd android-app
./gradlew assembleDebug          # build a debug APK
./gradlew installDebug           # install to a connected device/emulator
# Or open the android-app/ folder in Android Studio and hit ▶ Run
```

### Run the Desktop App (Electron)
```bash
cd desktop
npm install
npm run dev
```

---

## 📂 Repository Layout

```
vastavikCodingStuff/
├── 📱 mobile/        # Flutter app (iOS)
├── 🤖 android-app/   # Kotlin app (Android Phones & Tablets)
├── 🌐 web/           # Web application
├── 🖥️ desktop/      # Electron desktop app
├── 🐱 catalan/       # Catalan locale & resources
├── 🎨 design/        # Design tokens, assets, Figma exports
├── 📦 shared/        # Shared types, API client, utils
└── 📄 docs/          # Architecture & contribution docs
```

---

## 🤝 Contributing

Contributions are welcome! Please read our contributing guide, open an issue, or submit a pull request.

1. Fork the repository
2. Create your feature branch — `git checkout -b feature/amazing-feature`
3. Commit your changes — `git commit -m 'Add amazing feature'`
4. Push to the branch — `git push origin feature/amazing-feature`
5. Open a Pull Request

---

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for the full text.

---

## 💫 Author

<div align="center">

**Parth Vastavik** — *Full Stack Developer · Machine Learning Enthusiast*

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/parthasdey2304)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/sarathiparth)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram)](https://instagram.com/vastavik_parth)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x)](https://twitter.com/vastavik__parth)

<sub>⭐ Star this repo if you like the work — it helps a lot!</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=120&section=footer" width="100%"/>

</div>
