# ⌚ FiTagotchi

> *How can we motivate a gamer to adopt a healthy lifestyle?*
> By turning daily physical activity into an adventure on the wrist.

FiTagotchi is an **Apple Watch** game built around a virtual pet that lives on your activity. Move more, and your FiTagotchi thrives; stay still, and it gets tired — or worse.

## ✨ Features

- **HealthKit integration** — reads steps, active calories and other activity data in real time.
- **Reward loop** — activity is converted into coins, spent on items that keep the pet healthy.
- **Reactive avatar** — SpriteKit animations change with the pet's state: happy, tired, sleeping, or "dead".
- **Long-term goal** — reaching milestones lets the pet rebuild its spaceship and fly back to its home planet.
- **Watch-face widget** (WidgetKit) showing the pet's mood at a glance.

## 🛠️ Tech stack

| | |
|---|---|
| Language | Swift |
| UI | SwiftUI, SpriteKit |
| Frameworks | HealthKit, HealthKitUI, WidgetKit, AppIntents, WatchConnectivity |
| Platform | watchOS |

## 🧩 Architecture overview

```
FiTagotchi Watch App/
├── GameView.swift              # main game scene and pet state machine
├── Scenes/                     # SpriteKit scenes & animations
├── BackEnd/                    # HealthKit queries and data management
├── MenuOptions/                # shop, stats, settings
├── RocketProgressView.swift    # spaceship-rebuild progress
└── StatisticCircleView.swift   # activity rings / stats
ExpressionWidgetExtension/      # watch-face widget
```

## 🚀 Getting started

1. Download the repo, unzip `Salute/FiTagotchi.zip` and open `FiTagotchi.xcodeproj` in Xcode 15+.
2. Select the *FiTagotchi Watch App* scheme and a watchOS simulator or paired Apple Watch.
3. Grant HealthKit permissions on first launch.

## 📄 License

See [LICENSE](LICENSE).
