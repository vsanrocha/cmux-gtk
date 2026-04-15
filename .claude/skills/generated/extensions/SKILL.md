---
name: extensions
description: "Skill for the Extensions area of cmux-gtk. 60 symbols across 29 files."
---

# Extensions

60 symbols | 29 files | Cohesion: 73%

## When to Use

- Working with code in `ghostty/`
- Understanding how didEnterFullScreenNotification, didExitFullScreenNotification, enter work
- Modifying extensions-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Helpers/Fullscreen.swift` | enter, fullscreenDidChange, didEnterFullScreenNotification, didExitFullScreenNotification, enter (+4) |
| `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | reloadDockMenu, setupMenuImages, syncMenuShortcuts, syncMenuShortcut |
| `ghostty/macos/Sources/Features/Terminal/Window Styles/TerminalWindow.swift` | configureTabContextMenuIfNeeded, isTabContextMenu, appendTabModifierSection, sendEvent |
| `ghostty/macos/Sources/Helpers/Extensions/NSImage+Extension.swift` | NSImage, combine, gradient, tint |
| `ghostty/macos/Tests/Helpers/TransferablePasteboardTests.swift` | pasteboardItemIsCreated, pasteboardItemProvidesCorrectData, multipleTypesProvideCorrectData |
| `ghostty/macos/Sources/Helpers/Extensions/NSWindow+Extension.swift` | tabButtonsInVisualOrder, tabButtonHit, tabIndex |
| `ghostty/macos/Sources/Helpers/Extensions/NSMenuItem+Extension.swift` | NSMenuItem, setImageIfDesired |
| `ghostty/macos/Sources/Helpers/Extensions/NSMenu+Extension.swift` | insertItem, removeItems |
| `ghostty/include/ghostty.h` | ghostty_surface_config_new, ghostty_inspector_text |
| `ghostty/macos/Sources/Helpers/Extensions/Array+Extension.swift` | withCStrings, helper |

## Entry Points

Start here when exploring this area:

- **`didEnterFullScreenNotification`** (Function) — `ghostty/macos/Sources/Helpers/Fullscreen.swift:76`
- **`didExitFullScreenNotification`** (Function) — `ghostty/macos/Sources/Helpers/Fullscreen.swift:81`
- **`enter`** (Function) — `ghostty/macos/Sources/Helpers/Fullscreen.swift:100`
- **`fullscreenFrame`** (Function) — `ghostty/macos/Sources/Helpers/Fullscreen.swift:323`
- **`hideDock`** (Function) — `ghostty/macos/Sources/Helpers/Fullscreen.swift:372`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `SavedState` | Class | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 391 |
| `NSMenuItem` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSMenuItem+Extension.swift` | 2 |
| `KeyboardShortcut` | Class | `ghostty/macos/Sources/Helpers/Extensions/KeyboardShortcut+Extension.swift` | 2 |
| `KeyEquivalent` | Class | `ghostty/macos/Sources/Helpers/Extensions/KeyboardShortcut+Extension.swift` | 48 |
| `EventModifiers` | Class | `ghostty/macos/Sources/Helpers/Extensions/EventModifiers+Extension.swift` | 4 |
| `ModifierFlags` | Class | `ghostty/macos/Sources/Helpers/Extensions/EventModifiers+Extension.swift` | 18 |
| `TransferableDataProvider` | Class | `ghostty/macos/Sources/Helpers/Extensions/Transferable+Extension.swift` | 24 |
| `UTType` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView+Transferable.swift` | 46 |
| `UUID` | Class | `ghostty/macos/Sources/Helpers/Extensions/UUID+Extension.swift` | 2 |
| `NSPasteboard` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSPasteboard+Extension.swift` | 4 |
| `NSImage` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSImage+Extension.swift` | 2 |
| `ExpiringUndoManager` | Class | `ghostty/macos/Sources/Helpers/ExpiringUndoManager.swift` | 13 |
| `UndoManager` | Class | `ghostty/macos/Sources/Helpers/Extensions/UndoManager+Extension.swift` | 2 |
| `OSColor` | Class | `ghostty/macos/Sources/Helpers/Extensions/OSColor+Extension.swift` | 5 |
| `didEnterFullScreenNotification` | Function | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 76 |
| `didExitFullScreenNotification` | Function | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 81 |
| `enter` | Function | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 100 |
| `fullscreenFrame` | Function | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 323 |
| `hideDock` | Function | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 372 |
| `hideMenu` | Function | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 382 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `ConfigureTabContextMenuIfNeeded → SetFrame` | cross_community | 9 |
| `ConfigureTabContextMenuIfNeeded → SetInitialWindowPosition` | cross_community | 8 |
| `OpenTab → ModifierFlags` | cross_community | 7 |
| `OpenWindow → ModifierFlags` | cross_community | 7 |
| `ConfigureTabContextMenuIfNeeded → TerminalController` | cross_community | 7 |
| `ConfigureTabContextMenuIfNeeded → AddTabbedWindowSafely` | cross_community | 7 |
| `GhosttyConfigDidChange → ModifierFlags` | cross_community | 6 |
| `HandleNewTabScriptCommand → ModifierFlags` | cross_community | 6 |
| `Application → ModifierFlags` | cross_community | 6 |
| `NewTab → ModifierFlags` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Surface View | 4 calls |
| Window Styles | 4 calls |
| Tests | 3 calls |
| Terminal | 3 calls |
| Update | 1 calls |
| Custom App Icon | 1 calls |

## How to Explore

1. `gitnexus_context({name: "didEnterFullScreenNotification"})` — see callers and callees
2. `gitnexus_query({query: "extensions"})` — find related execution flows
3. Read key files listed above for implementation details
