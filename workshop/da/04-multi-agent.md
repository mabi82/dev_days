<!-- l10n-sync: source-file="workshop/04-multi-agent.md" -->
# Del 4: Multi-Agent Development

[🎮 Live Demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) • [📚 Lab Guide](GUIDE.md) • [← Del 3](03-quiz-master.md)

---

> ⏱️ **Tid:** ~20 minutter

Byg nye features med specialiserede agents: TDD agents til robust kode og design agents til poleret UI.

---

## 🧪 Opgave 1: Scavenger Hunt mode (TDD-drevet)

Custom agents med handoffs opdeler komplekse workflows i mindre trin og holder dig i kontrol.

### Hvad vi bygger

En ny **Scavenger Hunt** mode:
- Samme spørgsmål som bingo
- Vist som enkel tjekliste
- Progress meter i toppen
- Klik for at markere færdig

### Trin

#### Fase 1: Plan

1. Start ny Chat i **Plan Mode**
2. Indtast:
   ```
   Add a new Scavenger Hunt mode: same questions, but shown as a
   simple list with checkboxes and a progress meter
   ```
3. **Iterer planen** - tjek at den:
   - ✅ Tilføjer mode på startskærmen
   - ✅ Opretter ny komponent til liste-visning
   - ✅ Indeholder progress indikator
   - ❌ Ikke overbygger med for mange features

#### Fase 2: TDD Red (skriv fejlede tests)

1. Vælg **TDD Red** agent
2. Klik **Start**
3. Se den skrive tests for:
   - Komponent-rendering
   - Checkbox-interaktioner
   - Progress-beregning
   - State-handsamling

4. Tjek **Test Explorer** for fejlede tests

#### Fase 3: TDD Green (faa tests til at passe)

1. Når Red er færdig, vælg **TDD Green**
2. Se den:
   - Implementere minimum-kode
   - Køre tests efter hver ændring
   - Iterere til alle tests er grøn

#### Fase 4: Refactor (ryd op)

1. Vælg **TDD Refactor**
2. Lad den forbedre kodekvaliteten uden at bryde tests

### Checkpoint recovery

Hvis noget går galt:
1. Brug Chat **Checkpoints** til rollback
2. Gå tilbage til før "TDD Red"
3. Prøv igen med justerede prompts

> 💡 **Bonus:** Proev **TDD Supervisor** for fuldautomatisk TDD-flow.

✅ **Resultat:** Fuldt testet Scavenger Hunt-feature bygget med disciplineret TDD.

---

## 🎴 Opgave 2: Card Deck mode (design-drevet)

Brug **Pixel Jam** agenten til UI-iteration mens du bygger nye features.

### Hvad vi bygger

En ny **Card Deck Shuffle** mode:
- Spilleren åbner spillet
- Trykker for at få et tilfældigt kort
- Kortet flipper med animation
- Viser et spørgsmål at tale om

### Trin

1. Start ny Chat
2. Vælg **Pixel Jam** agent
3. Indtast:
   ```
   New mode: Card Deck Shuffle. Every player opens the game,
   taps, and gets a random card with a question
   ```
4. Se den iterere på UI
5. Følg op for forbedringer:
   ```
   Add a cool 3D flip animation when revealing the card
   ```
   ```
   Make the card styling match the cyberpunk theme
   ```
6. **Commit** når du er tilfreds

### Hvad Pixel Jam gør anderledes

- Fokus på **visuelt design** først
- Itererer **UI/UX** før logik
- Bruger frontend design-instruktioner
- Skaber polerede, animerede interfaces

---

## 🔍 Opgave 3: UX review agent

Kombiner MCP tools, custom workflows og subagent isolation for kraftfulde reviews.

### Trin

1. Start ny Chat med **Pixel Jam**
2. Indtast:
   ```
   Run review
   ```
3. Når du bliver spurgt, klik **Allow for this Workspace** for Playwright-adgang
4. Se den:
   - Tage screenshots af hver side
   - Analysere usability-problemer
   - Tjekke accessibility
   - Reviewe visuel konsistens

### Hvad der reviewes

| Kategori | Tjek |
|----------|------|
| **Usability** | Navigation flow, knap-tydelighed, feedback |
| **Accessibility** | Farvekontrast, keyboard navigation, screen readers |
| **Visual** | Konsistens, spacing, alignment |
| **Interaction** | Touch targets, hover states, animationer |

### Opfølgning

Efter review:
```
File the critical findings as GitHub issues
```
```
Fix the accessibility issues you found
```
```
Assign the navigation bug to a background agent
```

✅ **Resultat:** Omfattende UX review med handlingsklare fund.

---

## 🎯 Bonus-udfordringer

| Udfordring | Fremgangsmaade |
|-----------|----------------|
| Fix UX issues | Deleger til background eller cloud agent |
| Flere temaer | Tilføj theme picker på startskærmen |
| Social deling | Tilføj share-knap i win-state |
| Leaderboard | Track og vis highscores |
| Lydeffekter | Tilføj audio feedback for interaktioner |

---

## ✅ Del 4 færdig

Du har lært at:
- Bruge TDD agents til testdrevet udvikling
- Bygge features med Red-Green-Refactor
- Bruge designfokuserede agents som Pixel Jam
- Køre omfattende UX reviews
- Kombinere flere agents i komplekse workflows

---

## 🎉 Workshop færdig

Tillykke - du har gennemført VS Code GitHub Copilot Agent Lab.

### Hvad du byggede

- ✅ En fuldt redesignet Social Bingo app
- ✅ Custom quiz-temaer
- ✅ Scavenger Hunt mode (TDD-bygget)
- ✅ Card Deck Shuffle mode (design-drevet)

### Hvad du lærte

1. **Context Engineering** - lær AI om din kodebase
2. **Agentic Primitives** - background, cloud og custom agents
3. **Design-First Development** - UI-iteration med AI-assistance
4. **Test-Driven Development** - pålidelig kode med TDD agents

### Fortsæt

- 📺 [VS Code on YouTube](https://www.youtube.com/code)
- 📖 [VS Code Copilot Docs](https://code.visualstudio.com/docs/copilot/overview)
- 🌟 [Awesome Copilot](https://github.com/github/awesome-copilot)
