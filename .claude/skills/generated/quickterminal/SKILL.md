---
name: quickterminal
description: "Skill for the QuickTerminal area of cmux-gtk. 41 symbols across 9 files."
---

# QuickTerminal

41 symbols | 9 files | Cohesion: 67%

## When to Use

- Working with code in `ghostty/`
- Understanding how ghostty_surface_set_color_scheme, updateColorSchemeForSurfaceTree, setLoaded work
- Modifying quickterminal-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | windowDidLoad, syncAppearance, ghosttyConfigDidChange, saveScreenState, animateWindowOut (+15) |
| `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | setLoaded, setFinal, configuredFrameSize, finalOrigin, setInitial (+4) |
| `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalScreenStateCache.swift` | frame, onScreensChanged, pruneCapacity, isValid, save |
| `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalSize.swift` | toPixels, calculate |
| `ghostty/include/ghostty.h` | ghostty_surface_set_color_scheme |
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | updateColorSchemeForSurfaceTree |
| `ghostty/macos/Sources/Helpers/Extensions/View+Extension.swift` | innerShadow |
| `ghostty/macos/Sources/Features/Splits/TerminalSplitTreeView.swift` | overlay |
| `ghostty/macos/Sources/Helpers/Private/CGS.swift` | active |

## Entry Points

Start here when exploring this area:

- **`ghostty_surface_set_color_scheme`** (Function) — `ghostty/include/ghostty.h:1097`
- **`updateColorSchemeForSurfaceTree`** (Function) — `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift:1470`
- **`setLoaded`** (Function) — `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift:11`
- **`windowDidLoad`** (Function) — `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift:110`
- **`syncAppearance`** (Function) — `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift:599`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ghostty_surface_set_color_scheme` | Function | `ghostty/include/ghostty.h` | 1097 |
| `updateColorSchemeForSurfaceTree` | Function | `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | 1470 |
| `setLoaded` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | 11 |
| `windowDidLoad` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | 110 |
| `syncAppearance` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | 599 |
| `ghosttyConfigDidChange` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | 698 |
| `innerShadow` | Function | `ghostty/macos/Sources/Helpers/Extensions/View+Extension.swift` | 3 |
| `overlay` | Function | `ghostty/macos/Sources/Features/Splits/TerminalSplitTreeView.swift` | 221 |
| `frame` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalScreenStateCache.swift` | 49 |
| `onScreensChanged` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalScreenStateCache.swift` | 63 |
| `pruneCapacity` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalScreenStateCache.swift` | 91 |
| `isValid` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalScreenStateCache.swift` | 110 |
| `toPixels` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalSize.swift` | 40 |
| `calculate` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalSize.swift` | 51 |
| `setFinal` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | 40 |
| `configuredFrameSize` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | 59 |
| `finalOrigin` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | 93 |
| `save` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalScreenStateCache.swift` | 36 |
| `setInitial` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | 21 |
| `initialOrigin` | Function | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalPosition.swift` | 65 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `ApplicationDidFinishLaunching → SetFrame` | cross_community | 8 |
| `ToggleQuickTerminal → ToPixels` | cross_community | 8 |
| `ToggleQuickTerminal → DisplayEntry` | cross_community | 7 |
| `ToggleQuickTerminal → PruneCapacity` | cross_community | 7 |
| `ApplicationDidFinishLaunching → Active` | cross_community | 6 |
| `ApplicationDidFinishLaunching → MakeWindowKey` | cross_community | 6 |
| `ApplicationDidFinishLaunching → SurfaceConfiguration` | cross_community | 6 |
| `ApplicationDidFinishLaunching → SurfaceView` | cross_community | 6 |
| `ToggleQuickTerminal → SetFrame` | cross_community | 6 |
| `ToggleQuickTerminal → InitialOrigin` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Terminal | 8 calls |
| Window Styles | 2 calls |
| Surface View | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ghostty_surface_set_color_scheme"})` — see callers and callees
2. `gitnexus_query({query: "quickterminal"})` — find related execution flows
3. Read key files listed above for implementation details
