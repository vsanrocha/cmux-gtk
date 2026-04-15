---
name: ghostty
description: "Skill for the Ghostty area of cmux-gtk. 140 symbols across 19 files."
---

# Ghostty

140 symbols | 19 files | Cohesion: 92%

## When to Use

- Working with code in `ghostty/`
- Understanding how ghostty_app_userdata, ghostty_surface_app, ghostty_surface_inherited_config work
- Modifying ghostty-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | openConfig, newTab, newWindow, toggleFullscreen, action (+65) |
| `ghostty/macos/Tests/Ghostty/ConfigTests.swift` | initialWindowDefaultsToTrue, initialWindowSetToFalse, quitAfterLastWindowClosedDefaultsToFalse, quitAfterLastWindowClosedSetToTrue, windowStepResizeDefaultsToFalse (+31) |
| `ghostty/include/ghostty.h` | ghostty_app_userdata, ghostty_surface_app, ghostty_surface_inherited_config, ghostty_surface_key_is_binding, ghostty_app_set_focus (+1) |
| `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | windowDidBecomeKey, syncFloatOnTopMenu, userNotificationCenter, findSurface, AppDelegate |
| `ghostty/macos/Sources/Ghostty/Ghostty.Surface.swift` | sendKeyEvent, keyIsBinding, sendText, sendMouseButton |
| `ghostty/macos/Sources/Ghostty/GhosttyPackage.swift` | AllocatedString, from, toNative |
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_AppKit.swift` | setCursorShape, setCursorVisibility |
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView.swift` | dotOpacity, SearchState |
| `ghostty/macos/Sources/Ghostty/Ghostty.Input.swift` | withCValue, Key |
| `ghostty/macos/Sources/Helpers/Extensions/Double+Extension.swift` | Double |

## Entry Points

Start here when exploring this area:

- **`ghostty_app_userdata`** (Function) — `ghostty/include/ghostty.h:1068`
- **`ghostty_surface_app`** (Function) — `ghostty/include/ghostty.h:1085`
- **`ghostty_surface_inherited_config`** (Function) — `ghostty/include/ghostty.h:1086`
- **`from`** (Function) — `ghostty/macos/Sources/Ghostty/GhosttyPackage.swift:92`
- **`action`** (Function) — `ghostty/macos/Sources/Ghostty/Ghostty.App.swift:266`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `AllocatedString` | Class | `ghostty/macos/Sources/Ghostty/GhosttyPackage.swift` | 67 |
| `Double` | Class | `ghostty/macos/Sources/Helpers/Extensions/Double+Extension.swift` | 0 |
| `SearchState` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView.swift` | 1270 |
| `TemporaryConfig` | Class | `ghostty/macos/Tests/Ghostty/ConfigTests.swift` | 218 |
| `Key` | Class | `ghostty/macos/Sources/Ghostty/Ghostty.Input.swift` | 1175 |
| `AppDelegate` | Class | `ghostty/macos/Sources/App/macOS/AppDelegate+Ghostty.swift` | 6 |
| `AppDelegate` | Class | `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | 7 |
| `ghostty_app_userdata` | Function | `ghostty/include/ghostty.h` | 1068 |
| `ghostty_surface_app` | Function | `ghostty/include/ghostty.h` | 1085 |
| `ghostty_surface_inherited_config` | Function | `ghostty/include/ghostty.h` | 1086 |
| `from` | Function | `ghostty/macos/Sources/Ghostty/GhosttyPackage.swift` | 92 |
| `action` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 266 |
| `appState` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 455 |
| `surfaceView` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 467 |
| `quit` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 678 |
| `checkForUpdates` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 693 |
| `openURL` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 701 |
| `undo` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 742 |
| `redo` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 763 |
| `newSplit` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | 845 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Perform → StoredPermission` | cross_community | 6 |
| `Simulate → Double` | cross_community | 6 |
| `GhosttySurfaceDragEndedNoTarget → Double` | cross_community | 5 |
| `Action → Ghostty_surface_userdata` | cross_community | 4 |
| `Action → Ghostty_surface_app` | intra_community | 4 |
| `Action → Ghostty_app_userdata` | intra_community | 4 |
| `Perform → GetStoredResult` | cross_community | 4 |
| `Perform → FormatRememberText` | cross_community | 4 |
| `HandleSplit → Ghostty_surface_userdata` | cross_community | 4 |
| `GotoSplit → Dimensions` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Extensions | 7 calls |
| Surface View | 7 calls |
| Terminal | 3 calls |
| AppleScript | 3 calls |
| Include | 2 calls |
| Tests | 1 calls |
| Splits | 1 calls |
| MacOS | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ghostty_app_userdata"})` — see callers and callees
2. `gitnexus_query({query: "ghostty"})` — find related execution flows
3. Read key files listed above for implementation details
