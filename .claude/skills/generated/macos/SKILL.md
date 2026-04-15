---
name: macos
description: "Skill for the MacOS area of cmux-gtk. 40 symbols across 10 files."
---

# MacOS

40 symbols | 10 files | Cohesion: 80%

## When to Use

- Working with code in `ghostty/`
- Understanding how ghostty_app_has_global_keybinds, enable, disable work
- Modifying macos-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | ghosttyConfigDidChange, terminalWindowHasBell, syncDockBadge, setDockBadge, syncAppearance (+20) |
| `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift` | enable, disable, tryEnable, cgEventFlagsChangedHandler |
| `ghostty/include/ghostty.h` | ghostty_app_has_global_keybinds, ghostty_app_set_color_scheme, ghostty_app_key |
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | ghosttyCommandPaletteDidToggle, toggleCommandPalette |
| `ghostty-gtk/src/app.rs` | set_color_scheme |
| `ghostty/macos/Sources/Features/Update/UpdateController.swift` | startUpdater |
| `ghostty/macos/Sources/Features/Services/ServiceProvider.swift` | ServiceProvider |
| `ghostty/macos/Sources/Ghostty/NSEvent+Extension.swift` | ghosttyKeyEvent |
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_AppKit.swift` | performKeyEquivalent |
| `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | toggle |

## Entry Points

Start here when exploring this area:

- **`ghostty_app_has_global_keybinds`** (Function) — `ghostty/include/ghostty.h:1076`
- **`enable`** (Function) — `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift:34`
- **`disable`** (Function) — `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift:59`
- **`tryEnable`** (Function) — `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift:75`
- **`ghosttyConfigDidChange`** (Function) — `ghostty/macos/Sources/App/macOS/AppDelegate.swift:644`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ServiceProvider` | Class | `ghostty/macos/Sources/Features/Services/ServiceProvider.swift` | 3 |
| `ghostty_app_has_global_keybinds` | Function | `ghostty/include/ghostty.h` | 1076 |
| `enable` | Function | `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift` | 34 |
| `disable` | Function | `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift` | 59 |
| `tryEnable` | Function | `ghostty/macos/Sources/Features/Global Keybinds/GlobalEventTap.swift` | 75 |
| `ghosttyConfigDidChange` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 644 |
| `terminalWindowHasBell` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 675 |
| `syncDockBadge` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 680 |
| `setDockBadge` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 739 |
| `syncAppearance` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 838 |
| `updateAppIcon` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 842 |
| `set_color_scheme` | Function | `ghostty-gtk/src/app.rs` | 124 |
| `ghostty_app_set_color_scheme` | Function | `ghostty/include/ghostty.h` | 1077 |
| `startUpdater` | Function | `ghostty/macos/Sources/Features/Update/UpdateController.swift` | 45 |
| `applicationDidFinishLaunching` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 202 |
| `applicationDidBecomeActive` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 346 |
| `setupSignals` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 534 |
| `ghosttyBellDidRing` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 656 |
| `ghosttyNewWindow` | Function | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 719 |
| `ghostty_app_key` | Function | `ghostty/include/ghostty.h` | 1070 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `ApplicationDidFinishLaunching → SetFrame` | cross_community | 8 |
| `ToggleQuickTerminal → ToPixels` | cross_community | 8 |
| `ToggleQuickTerminal → DisplayEntry` | cross_community | 7 |
| `ToggleQuickTerminal → PruneCapacity` | cross_community | 7 |
| `GhosttyConfigDidChange → ModifierFlags` | cross_community | 6 |
| `ApplicationDidFinishLaunching → Active` | cross_community | 6 |
| `ApplicationDidFinishLaunching → MakeWindowKey` | cross_community | 6 |
| `ApplicationDidFinishLaunching → SurfaceConfiguration` | cross_community | 6 |
| `ApplicationDidFinishLaunching → SurfaceView` | cross_community | 6 |
| `ApplicationDidFinishLaunching → RemotePlatform` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Extensions | 4 calls |
| Terminal | 3 calls |
| Surface View | 2 calls |
| QuickTerminal | 2 calls |
| Remote | 1 calls |
| Ui | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ghostty_app_has_global_keybinds"})` — see callers and callees
2. `gitnexus_query({query: "macos"})` — find related execution flows
3. Read key files listed above for implementation details
