# Project Guidelines

## Mandatory Development Checklist
- Lint: run `dotnet format --verify-no-changes` (or equivalent lint check used in your branch).
- Build: run `dotnet build SocOps/SocOps.csproj`.
- Test: run `dotnet test` when a test project exists.

## Code and Architecture
- Stack: Blazor WebAssembly on .NET 10 (`SocOps/SocOps.csproj`); DI and startup in `SocOps/Program.cs`.
- App flow: `SocOps/Pages/Home.razor` switches UI by `BingoGameService.CurrentGameState`.
- Boundaries: UI in `SocOps/Components/`, models in `SocOps/Models/`, state orchestration in `SocOps/Services/BingoGameService.cs`, pure bingo logic in `SocOps/Services/BingoLogicService.cs`, content in `SocOps/Data/Questions.cs`.
- Style: standard C# naming conventions, nullable reference types, and composable Blazor components using `[Parameter]` and `EventCallback`.
- Frontend styling: follow utilities in `SocOps/wwwroot/css/app.css` and scoped instructions in `.github/instructions/css-utilities.instructions.md` and `.github/instructions/frontend-design.instructions.md`.

## Conventions
- Keep game-state changes centralized in `BingoGameService`; do not mutate board state directly in UI components.
- Maintain lifecycle hygiene: subscribe/unsubscribe state change handlers (see `SocOps/Pages/Home.razor`).
- Keep localStorage compatibility stable in `BingoGameService` unless migration is intentional.
- Do not edit `.solutions/` unless explicitly requested.

## Docs
- Project overview: `README.md`
- Workshop guide: `workshop/GUIDE.md`
- Contribution and policy docs: `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`
