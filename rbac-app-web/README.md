# 🛡️ RBAC App
<p align="center">
  <img src="https://angular.io/assets/images/logos/angular/angular.svg" alt="Angular Logo" width="180">
  <br />
  <img src="https://img.shields.io/badge/version-0.0.1-5c5c5c.svg?style=flat" alt="version">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Angular-DD0031?style=flat&logo=angular&logoColor=white" alt="Angular" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/NgRx-BA2BD2?style=flat&logo=ngrx&logoColor=white" alt="NgRx" />
  <img src="https://img.shields.io/badge/RxJS-B7178C?style=flat&logo=reactivex&logoColor=white" alt="RxJS" />
  <img src="https://img.shields.io/badge/Husky-42b983?style=flat&logo=npm&logoColor=white" alt="Husky" />
  <img src="https://img.shields.io/badge/Jasmine-8A4182?style=flat&logo=jasmine&logoColor=white" alt="Jasmine" />
</p>

> The core enterprise frontend application for the Role-Based Access Control (RBAC) System, built with strict reactive architecture principles.

---

## 🔗 📋 Table of Contents

*   🌟 [Features & Modules](#-features--modules)
*   🏗️ [Architecture Guidelines](#️-architecture-guidelines)
*   🚀 [Quick Start](#-quick-start)
*   🛠️ [Tech Stack](#️-tech-stack)
*   🧪 [Testing](#-testing)
*   🐳 [Docker Management](#-docker-management)
*   📄 [License](#-license)

---

## 🌟 Features & Modules

The application is structured into discrete **Feature Modules**:

| Module | Description |
| :--- | :--- |
| **Users** | Core domain managing user lifecycle, identity, and role assignment. |
| **Roles** | Complex logic for role hierarchies and assignment strategies. |
| **Permissions** | Management of distinct system capabilities and precise access control rules. |
| **Applications** | Configuration for third-party systems relying on our RBAC ecosystem. |
| **Actions** | Definition and management of distinct actionable operations within the system. |


---

## 🏗️ Architecture Guidelines

We enforce a strict **Component-Driven** approach with total separation of concerns, heavily influenced by modern Angular scalable architectures and unidirectional data flow.

*   **Core Module**: Singleton services, interceptors, guards, and app-wide dependencies.
*   **Shared Module**: Reusable dumb components, pipes, directives, and UI layouts.
*   **Feature Modules**: Lazy-loaded modules containing smart components and isolated NgRx state.



---

## 🚀 Quick Start

**Prerequisites**

*   **Node.js**: (LTS recommended)
*   **npm/pnpm**: Package manager.

<br>

**1. Installation**

```bash
$ npm install
```

**2. Environment Setup**

Copy the development environment file:

```bash
$ cp src/environments/environment.development.ts src/environments/environment.ts
```

**3. Run Application**

```bash
# Watch mode (Development)
$ npm start

# Production build
$ npm run build
```

---

## 🛠️ Tech Stack

*   **Framework**: [Angular 19](https://angular.dev/)
*   **Language**: [TypeScript](https://www.typescriptlang.org/)
*   **State Management**: [NgRx](https://ngrx.io) Store, Effects, & Entity
*   **Git Hooks**: [Husky](https://typicode.github.io/husky/) and Lint-Staged
*   **Testing**: Jasmine & Karma

---

## 🧪 Testing

We prioritize testing at multiple levels:

```bash
# Unit Tests
$ npm run test

# E2E Tests
$ npm run e2e

# Test Coverage
$ npm run test -- --code-coverage
```

---

## 🐳 Docker Management

Helper scripts for managing local containers (e.g., SSR or backend API dependencies):

```bash
$ npm run d:up:dev      # Start Services
$ npm run d:down:dev    # Stop Services
$ npm run d:reset:dev   # Reset Services (⚠️ Wipes Data)
```

---
