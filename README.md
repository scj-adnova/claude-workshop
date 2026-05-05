# Claude Code Workshop

Willkommen zum Claude Code Workshop. Dieses Repository enthält alle Materialien die du für den Workshop benötigst.

## Struktur

```
workshop/
  claude-workshop/          ← dieses Repo (Aufgaben & Materialien)
  calculator-java/          ← Calculator Repo (Java / Spring Boot)
  calculator-angular/       ← Calculator Repo (Typescript / Angular)
  calculator-c/             ← Calculator Repo (C CLI)
  calculator-go/            ← Calculator Repo (Go)
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
git clone https://github.com/scj-adnova/calculator-go
git clone https://github.com/scj-adnova/team-marketplace
```

### 2. Claude Code installieren

> Anthropic empfiehlt den **Native Installer**. Er braucht kein Node.js und aktualisiert sich automatisch im Hintergrund.

**Variante A – Native Installer (empfohlen):**

```bash
# macOS, Linux, WSL
curl -fsSL https://claude.ai/install.sh | bash
```

```powershell
# Windows PowerShell
irm https://claude.ai/install.ps1 | iex
```

**Variante B – Paketmanager (falls "curl | bash" durch eure Firmen-Policy blockiert ist):**

```bash
brew install --cask claude-code              # macOS (Homebrew)
winget install Anthropic.ClaudeCode          # Windows (WinGet)
sudo apt install claude-code                 # Debian / Ubuntu (Repo siehe Doku)
```

**Variante C – npm (für Node.js-Nutzer, kein sudo!):**

```bash
node --version                                # muss >= 18.0.0 sein
npm install -g @anthropic-ai/claude-code
```

### 3. Calculator-Repo starten

Wähle das Repo für deine Programmiersprache und folge der README im jeweiligen Repo.

## Workshop-Materialien

| Datei | Inhalt |
|---|---|
| [praxisaufgaben.md](./praxisaufgaben.md) | Alle Hands-on Aufgaben |

## Team-Marketplace

Das [team-marketplace](https://github.com/scj-adnova/team-marketplace)-Repo enthält fertige Skills, Agents, Hooks und Commands die in Kapitel 8 eingebunden werden. Struktur und Einrichtung sind in den Praxisaufgaben beschrieben.

## Voraussetzungen

- Node.js >= 18
- Git
- Claude.ai Pro/Max/Team/Enterprise Account
