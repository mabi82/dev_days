<!-- l10n-sync: source-file="workshop/01-setup.md" -->
# Del 1: Setup og Context Engineering

[🎮 Live Demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) • [📚 Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) • [← Overblik](00-overview.md)

---

> ⏱️ **Tid:** ~15 minutter

I denne del sætter du udviklingsmiljøet op og lærer GitHub Copilot om din kodebase.

---

## 🔧 Initial setup

### Trin 1: Opret dit repository

1. Åbn [github.com/copilot-dev-days/agent-lab-dotnet](https://github.com/copilot-dev-days/agent-lab-dotnet)
2. Klik **Use this template** -> **Create a new repository**
   - Navn: `my-soc-ops-csharp`
   - Synlighed: **Public**
3. ✅ Dit eget Soc Ops repo er klart

### Trin 2: Aktiver GitHub Pages

1. Gå til repoets **Settings** -> **Pages**
2. Under "Build and deployment", vælg **GitHub Actions**
3. ✅ Hvert commit publicerer nu til: `https://{username}.github.io/{repo-name}`

### Trin 3: Vælg udviklingsmiljø

#### Option A: GitHub Codespaces (hurtigst)

1. Åbn dit nye repository på GitHub
2. Klik **Code** -> **Codespaces** -> **Create codespace on main**
3. Vent til devcontainer-setup er færdigt

#### Option B: Lokal VS Code

1. Åbn VS Code
2. Kør kommando: `Git: Clone` -> `Clone from GitHub`
3. Vælg dit nye repository
4. Installer **recommended extensions**, når du bliver spurgt

### Trin 4: Kør setup-agent

I Chat-panelet:

```
/setup
```

Agenten vil:
- Detektere dit miljø
- Installere manglende dependencies
- Starte development server

✅ **Succes:** Appen kører i browseren

---

## 📚 Forstå context engineering

Context engineering er måden, du lærer AI om din specifikke kodebase. Det giver mere præcise og relevante forslag fra Copilot.

### Opgave 1: Generer workspace-instruktioner

Instruktioner guider alle agent-interaktioner og gør dem mere stabile.

**Trin:**

1. Kør kommando: `Chat: Generate Agent Instructions`
2. Vent på, at agenten analyserer kodebasen
3. Gennemgå de genererede instruktioner
4. Følg op med:
   ```
   Compress down by half and add a mandatory development checklist
   (lint, build, test) to the top
   ```
5. **Commit** instruktion-filen

✅ **Resultat:** Fremtidige requests har et klart workspace-kort.

---

### Opgave 2: Background agents til parallelle opgaver

Background agents kører i isolerede git worktrees - perfekt til opgaver uden håndholding.

**Trin:**

1. I Chat input, skift **Session target** dropdown fra `Local` til `Copilot CLI`
2. Indtast:
   ```
   Add linting rules for unused vars and async/await usage; fix any errors
   ```
3. Lad den køre, og **Review** og **Apply** ændringerne
4. Højreklik på sessionen og slet den, når du er færdig

**Prøv også en cloud agent:**

1. Skift **Session target** til `Cloud`
2. Indtast:
   ```
   Make the README more engaging as a landing page to the project
   ```

✅ **Resultat:** Lint-regler, fejlrettelser og README-forbedringer merged tilbage til main.

---

### Opgave 3: Udforsk eksisterende instruktioner

Repoet har prækonfigurerede instruktioner, der hjælper AI med at forstå projektet.

#### CSS utility-instruktioner

📄 Se `.github/instructions/css-utilities.instructions.md`

De dokumenterer custom Tailwind-lignende CSS-klasser i dette Blazor-projekt.

> 💡 **Valgfrit:** Slet hovedteksten og kør prompten igen for at se ny generering.

#### Frontend design-instruktioner

📄 Se `.github/instructions/frontend-design.instructions.md`

"No purple gradients"-instruktionen udfordrer agenten til at tænke som en designer.

> 💡 **Tænk over:** Hvilke andre AI-biases kan du udfordre og styre?

---

## ✅ Del 1 færdig

Du har lært at:
- Sætte udviklingsmiljø op
- Generere og forbedre workspace-instruktioner
- Bruge background og cloud agents parallelt
- Forstå eksisterende instruktionsfiler
