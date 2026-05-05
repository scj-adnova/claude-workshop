# Claude Code Workshop

Willkommen zum Claude Code Workshop. Dieses Repository enthält alle Materialien die du für den Workshop benötigst.

## Struktur

```
workshop/
  claude-workshop/          ← dieses Repo (Aufgaben & Materialien)
  calculator-java/          ← Calculator Repo (Java / Spring Boot)
  calculator-angular/       ← Calculator Repo (Angular)
  calculator-c/             ← Calculator Repo (C CLI)
  team-marketplace/         ← Team-Marketplace Plugin-Repo
```

Alle Repos müssen auf **gleicher Ebene** liegen damit der Team-Marketplace korrekt eingebunden werden kann.

## Setup

### 1. Alle Repos klonen

```bash
mkdir workshop && cd workshop

git clone https://github.com/scj-adnova/claude-workshop
git clone https://github.com/scj-adnova/calculator-java       # oder deine Sprache
git clone https://github.com/scj-adnova/calculator-angular
git clone https://github.com/scj-adnova/calculator-c
git clone https://github.com/scj-adnova/team-marketplace
```

### 2. Claude Code installieren

```bash
node --version          # muss >= 18.0.0 sein
npm install -g @anthropic-ai/claude-code
claude --version
claude                  # Login im Browser
```

### 3. Calculator-Repo starten

Wähle das Repo für deine Programmiersprache und folge der README im jeweiligen Repo.

## Workshop-Materialien

| Datei | Inhalt |
|---|---|
| [praxisaufgaben.md](./praxisaufgaben.md) | Alle Hands-on Aufgaben (Kapitel 1–13) |

## Calculator-Repos

Jedes Calculator-Repo enthält eine kleine Taschenrechner-App mit absichtlichen Bugs – die Grundlage für alle Debugging-, Testing- und Sicherheits-Aufgaben im Workshop.

| Repo | Stack | Starten mit |
|---|---|---|
| [calculator-java](https://github.com/scj-adnova/calculator-java) | Spring Boot 3.2, Java 17 | `mvn spring-boot:run` |
| [calculator-angular](https://github.com/scj-adnova/calculator-angular) | Angular 17 Standalone | `npm install && npm start` |
| [calculator-c](https://github.com/scj-adnova/calculator-c) | C CLI | `make && ./calculator 10 + 5` |

## Team-Marketplace

Das [team-marketplace](https://github.com/scj-adnova/team-marketplace)-Repo enthält fertige Skills, Agents, Hooks und Commands die in Kapitel 8 eingebunden werden. Struktur und Einrichtung sind in den Praxisaufgaben beschrieben.

## Voraussetzungen

- Node.js >= 18
- Git
- Claude.ai Pro/Max/Team/Enterprise Account
