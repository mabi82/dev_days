🌐 [Danish](README.da.md) | [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

Turn any meetup into a high-energy social game.

**Soc Ops** is a fast, in-person social bingo app where players find people who match prompts on their board and race to complete a line.

[Play the Game](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) | [View Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) | [Workshop Files](workshop/)

---

## Why This Project

- Built as a practical workshop for building with AI coding agents.
- Demonstrates a clean Blazor WebAssembly architecture with clear service boundaries.
- Gives you a fun, real app to customize, ship, and demo quickly.

## What You Can Do

- Start a game and generate a dynamic bingo board.
- Mark squares as players find matching people.
- Detect bingo lines and show game progression.
- Experiment with AI-assisted design and feature iteration in a structured lab.

## Quick Start

### Prerequisite

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

### Run Locally

```bash
cd SocOps
dotnet run
```

### Build

```bash
cd SocOps
dotnet build
```

### Optional: Open in GitHub Codespaces

After creating your own repo from this template:

1. Open your repository on GitHub.
2. Select **Code** -> **Codespaces** -> **Create codespace on main**.
3. Wait for the dev container to finish setup.
4. Run:

```bash
cd SocOps
dotnet run
```

---

## Workshop Path

Use the workshop as a guided build journey:

| Part | Topic |
|------|-------|
| [00](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview and checklist |
| [01](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup and context engineering |
| [02](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-first frontend |
| [03](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [04](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-agent development |
| [05](workshop/05-complete.md) | Complete solution review |

You can also read the full workshop offline in [workshop/](workshop/).

---

## Project Structure

- `SocOps/Components/`: Reusable UI components (board, modal, screens).
- `SocOps/Pages/Home.razor`: Main game flow and state-driven page rendering.
- `SocOps/Services/BingoGameService.cs`: Game state orchestration.
- `SocOps/Services/BingoLogicService.cs`: Core bingo logic.
- `SocOps/Data/Questions.cs`: Prompt/question source data.

## Deployment

The app deploys automatically to GitHub Pages on push to `main`.

## Contributing

Contributions are welcome. Start with:

- [CONTRIBUTING.md](CONTRIBUTING.md)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- [SECURITY.md](SECURITY.md)

