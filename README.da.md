<!-- l10n-sync: source-file="README.md" -->
🌐 [English](README.md) | [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

Gør ethvert meetup til et energifyldt socialt spil.

**Soc Ops** er en hurtig social bingo-app til fysiske events, hvor spillere finder personer, der matcher felterne på kortet, og konkurrerer om at få fem på stribe.

[Spil spillet](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) | [Se lab-guiden](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) | [Workshop-filer](workshop/)

---

## Hvorfor dette projekt

- Bygget som en praktisk workshop i udvikling med AI coding agents.
- Viser en ren Blazor WebAssembly-arkitektur med tydelige servicegrænser.
- Giver dig en sjov, reel app, som du hurtigt kan tilpasse, shippe og demonstrere.

## Hvad du kan gøre

- Starte et spil og generere et dynamisk bingo-kort.
- Markere felter, når du finder en matchende person.
- Detektere bingo-linjer og vise spillets progression.
- Eksperimentere med AI-assisteret design og feature-iteration i en struktureret workshop.

## Hurtig start

### Forudsætning

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) eller nyere

### Kør lokalt

```bash
cd SocOps
dotnet run
```

### Build

```bash
cd SocOps
dotnet build
```

### Valgfrit: Åbn i GitHub Codespaces

Når du har oprettet dit eget repo fra denne template:

1. Åbn dit repository på GitHub.
2. Vælg **Code** -> **Codespaces** -> **Create codespace on main**.
3. Vent til dev container-setup er færdigt.
4. Kør:

```bash
cd SocOps
dotnet run
```

---

## Workshop-sti

Brug workshoppen som en guidet build-rejse:

| Del | Emne |
|------|-------|
| [00](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overblik og tjekliste |
| [01](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup og context engineering |
| [02](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-first frontend |
| [03](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [04](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-agent udvikling |
| [05](workshop/05-complete.md) | Komplet løsningsreview |

Du kan også læse hele workshoppen offline i [workshop/da/](workshop/da/).

---

## Projektstruktur

- `SocOps/Components/`: Genbrugelige UI-komponenter (board, modal, screens).
- `SocOps/Pages/Home.razor`: Hovedflow og state-drevet side-rendering.
- `SocOps/Services/BingoGameService.cs`: Orkestrering af game state.
- `SocOps/Services/BingoLogicService.cs`: Ren bingo-logik.
- `SocOps/Data/Questions.cs`: Datakilde for prompts/spørgsmål.

## Deployment

Appen deployer automatisk til GitHub Pages ved push til `main`.

## Bidrag

Bidrag er velkomne. Start med:

- [CONTRIBUTING.md](CONTRIBUTING.md)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- [SECURITY.md](SECURITY.md)
