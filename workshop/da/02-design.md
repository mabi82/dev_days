<!-- l10n-sync: source-file="workshop/02-design.md" -->
# Del 2: Design-First Frontend

[🎮 Live Demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) • [📚 Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) • [← Del 1](01-setup.md)

---

> ⏱️ **Tid:** ~15 minutter

Nu hvor repo-context er på plads, er det tid til kreativitet. Du redesigner hele UI med AI-assisteret udvikling.

---

## 🎨 Opgave 1: Giv appen dit eget udtryk

Brug **Plan Mode** til større opgaver. Iterer planen (2+ gange) med præciseringer.

### Trin

1. Skift til **Plan Mode** i Chat
2. Indtast din vision:
   ```
   Let's do a full redesign. Make it [YOUR THEME]
   ```
3. Gennemgå den genererede plan
4. Bed om justeringer til du er tilfreds
5. Klik **Implement**

### 🎭 Temaideer

| Kategori | Temaer |
|----------|--------|
| **Minimal** | Minimalist Mono, Scandinavian Calm, Desert Sand Minimal |
| **Retro** | Retro Terminal Green, Pixel Arcade Style, Vaporwave Sunset |
| **Dark** | Cyberpunk Neon, Dark Mode Noir, Space Galaxy Glow |
| **Playful** | Playful Candy Pop, Toybox Primary Colors, Anime Bubble |
| **Professional** | Corporate Clean Blue, Gradient Glass UI, Metallic Chrome |
| **Creative** | Brutalist Blocks, Geometric Memphis, Bold Constructivist |
| **Cozy** | Cozy Coffee Shop, Soft Pastel Clouds, Notebook Doodle |
| **Unique** | Skeuomorphic Stickers, Paper Card Cutouts, Chalkboard |

✅ **Resultat:** Frontend- og CSS-instruktioner kombineres til et gennemført design.

---

## 📝 Opgave 2: Hold instruktioner opdateret

Ved større ændringer i arkitektur, design eller dependencies skal instruktionerne opdateres.

### Trin

1. Efter redesign, følg op med:
   ```
   Add a design guide section to copilot-instructions.md
   ```
2. Gennemgå ændringerne
3. **Commit og push**

> 💡 Tjek at GitHub Pages opdaterer med dit nye design.

---

## 🚀 Opgave 3: Skalering med cloud agents

Generer flere designvariationer parallelt med cloud agents.

### Trin

1. Start en **ny Chat** i Plan Mode
2. Indtast:
   ```
   Redesign the start screen as a more engaging landing page
   ```
3. Noter variationer i planen
4. Kør exploration-prompten:
   ```
   /cloud-explore design variations
   ```
   📄 Se `.github/prompts/cloud-explore.prompt.md`

5. Tjek **Agent Sessions** for de 3 nye cloud agents
6. Åbn en session for status eller web-visning

### Hvad der sker

Prompten starter **3 parallelle cloud agents**, hver med sin designretning. De vil:
- Oprette branches
- Implementere variationer
- Tage screenshots
- Åbne PR'er til review

✅ **Resultat:** 3 designforslag at sammenligne, kørende parallelt.

> ⏰ Det tager nogle minutter. Fortsæt med Del 3, mens de kører.

---

## 🖼️ Design showcase

Eksempel på **Cyberpunk Neon** tema:

```
┌─────────────────────────────────────────────┐
│  ╔═══════════════════════════════════════╗  │
│  ║     🎮 SOC OPS - SOCIAL BINGO 🎮      ║  │
│  ╚═══════════════════════════════════════╝  │
│                                             │
│  ┌─────┬─────┬─────┬─────┬─────┐          │
│  │ ▓▓▓ │ ░░░ │ ▓▓▓ │ ░░░ │ ▓▓▓ │          │
│  ├─────┼─────┼─────┼─────┼─────┤          │
│  │ ░░░ │ ▓▓▓ │ ░░░ │ ▓▓▓ │ ░░░ │  NEON   │
│  ├─────┼─────┼─────┼─────┼─────┤  GLOW   │
│  │ ▓▓▓ │ ░░░ │ ★★★ │ ░░░ │ ▓▓▓ │          │
│  ├─────┼─────┼─────┼─────┼─────┤          │
│  │ ░░░ │ ▓▓▓ │ ░░░ │ ▓▓▓ │ ░░░ │          │
│  ├─────┼─────┼─────┼─────┼─────┤          │
│  │ ▓▓▓ │ ░░░ │ ▓▓▓ │ ░░░ │ ▓▓▓ │          │
│  └─────┴─────┴─────┴─────┴─────┘          │
│                                             │
│         [ 🔄 NEW GAME ]  [ 🎯 BINGO! ]      │
└─────────────────────────────────────────────┘
```

---

## ✅ Del 2 færdig

Du har lært at:
- Bruge Plan Mode til komplekse design-opgaver
- Iterere planer før implementering
- Opdatere instruktioner efter ændringer
- Skalere udforskning med parallelle cloud agents
