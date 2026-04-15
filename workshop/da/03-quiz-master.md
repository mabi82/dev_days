<!-- l10n-sync: source-file="workshop/03-quiz-master.md" -->
# Del 3: Custom Quiz Master

[🎮 Live Demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) • [📚 Lab Guide](GUIDE.md) • [← Del 2](02-design.md)

---

> ⏱️ **Tid:** ~10 minutter

Lav dine egne specialiserede quiz-temaer med custom agents - workflows, der går ud over generiske prompts.

---

## 🎲 Forstå custom agents

Custom agents er defineret i `.github/agents/` og giver:
- **Specialiseret viden** til konkrete opgaver
- **Konsistente workflows** til gentagelige processer
- **Fokuseret context**, der forbedrer output-kvalitet

📄 Se: `.github/agents/quiz-master.agent.md`

---

## 🎯 Opgave: Din egen Quiz Master

### Trin

1. Start en **ny Chat**
2. Vælg **Quiz Master** som custom agent
3. Indtast dit tema:
   ```
   Update questions to [YOUR THEME]
   ```
   Eller:
   ```
   Update quiz
   ```

4. Gennemgå de genererede spørgsmål
5. Følg op for mere kreativitet:
   ```
   Make them more chaotic and unexpected!
   ```

### 🎭 Temaideer

| Kategori | Temaer |
|----------|--------|
| **Professional** | Skill Bingo, Team Bingo, Work Culture Bingo |
| **Personal** | Personality Bingo, Lifestyle Bingo, Travel Bingo |
| **Tech** | Tech Life Bingo, Fandom Bingo, Dev Memes Bingo |
| **Interactive** | Secret Challenge Bingo, Micro-Challenge Bingo, Mystery Bingo |
| **Fun** | Office Humor Bingo, Chaos Bingo, Opposites Bingo |
| **Deep** | Deep Chat Bingo, Creative Bingo, Reflective Bingo |

### Tema-beskrivelser

- **Skill Bingo** - Arbejds- eller tekniske skills i stedet for personlige facts
- **Personality Bingo** - Præferencer, særlige vaner og sjove træk
- **Secret Challenge Bingo** - Korte mikro-opgaver med nye mennesker
- **Team Bingo** - Kategorier efter afdeling eller team
- **Tech Life Bingo** - Sprog, shortcuts, frameworks og dev-memes
- **Chaos Bingo** - Overraskende og uforudsigelige prompts
- **Opposites Bingo** - Find personer, der er din modsatte profil

---

## ☁️ Opgave: Quiz-generering i cloud

Kør Quiz Master som cloud agent til asynkron generering.

### Trin

1. Skift **Session target** til `Cloud`
2. Vælg **Quiz Master**
3. Indtast et andet tema:
   ```
   Create a Tech Life Bingo with questions about
   coding habits, IDE preferences, and developer culture
   ```
4. Lad den køre i baggrunden
5. Review PR'en, når den er klar

✅ **Resultat:** Custom agent laver kreative, tematiserede spørgsmål, mens du fortsætter arbejdet.

---

## 📝 Eksempeloutput: Tech Life Bingo

```
┌────────────────────────────────────────────────┐
│  Uses dark mode     │  Has 50+ browser tabs   │
│  for everything     │  open right now         │
├────────────────────────────────────────────────┤
│  Knows vim          │  Has a mechanical       │
│  keybindings        │  keyboard               │
├────────────────────────────────────────────────┤
│  Prefers tabs       │  Has strong opinions    │
│  over spaces        │  about semicolons       │
├────────────────────────────────────────────────┤
│  Uses AI to write   │  Has a dotfiles         │
│  commit messages    │  repository             │
└────────────────────────────────────────────────┘
```

---

## 💡 Pro tips

1. **Vær specifik** - konkrete temaer giver bedre resultater
2. **Iterer** - følg op for tone og kreativitet
3. **Mix temaer** - fx "Tech Life + Chaos Bingo"
4. **Test lokalt** - se hvordan prompts passer på bingo-grid

---

## ✅ Del 3 færdig

Du har lært at:
- Bruge custom agents til specialiserede workflows
- Generere tematiserede quiz-spørgsmål
- Køre custom agents i cloud
- Iterere output til bedre kvalitet
