# FPS Prototype 1

A first-person shooter prototype built in Unity.

## About

Multiplayer FPS prototype using Unity NetCode and Unity Gaming Services. Host or join sessions from the main menu, pick a character, and play a networked match. Currently at prototype stage — core movement, shooting, and client/server connectivity are in place.

## Getting Started

### Requirements( Must haves to run or test this)
- Unity Hub
- Unity editor version: `6000.5.6f1` (Unity 6)
- Git

### Setup
1. Clone the repo:
   ```bash
   git clone https://github.com/Jatin2705/FPS_Prototype1.git
   ```
2. Open Unity Hub → **Add** → select the `fps game` folder (not the repo root — that's where the actual Unity project lives).
3. Let Unity import/re-resolve packages (first open can take a few minutes).
4. Open the main scene: `Assets/Scenes/MainMenu.unity` (gameplay lives in `Assets/Scenes/GameScene.unity`).
5. Press Play.

## Project Structure

```
FPS_Prototype1/           <- repo root
├── README.md
├── CONTRIBUTING.md
└── fps game/              <- actual Unity project (open THIS in Unity Hub)
    ├── Assets/
    │   ├── Scripts/
    │   ├── Scenes/
    │   ├── Prefabs/
    │   └── ...
    ├── Packages/
    ├── ProjectSettings/
    └── .gitignore
```

## Contributing

Friends and outside contributors welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for branch naming, commit conventions, and how to submit a PR.

## License

_(Add a license if you want others to know what they're allowed to do with the code — MIT is common for small game prototypes. See https://choosealicense.com)_
