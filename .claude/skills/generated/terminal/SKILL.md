---
name: terminal
description: "Skill for the Terminal area of cmux-gtk. 163 symbols across 32 files."
---

# Terminal

163 symbols | 32 files | Cohesion: 79%

## When to Use

- Working with code in `ghostty/`
- Understanding how treeDoesNotContainRemovedView, removingNonexistentNodeLeavesTreeUnchanged, newSplit work
- Modifying terminal-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | newSplit, closeSurface, removeSurfaceNode, replaceSurfaceTree, ghosttyDidNewSplit (+41) |
| `ghostty/macos/Sources/Features/Terminal/TerminalController.swift` | applyCascade, newWindow, newTab, showWindow, replaceSurfaceTree (+40) |
| `ghostty/macos/Sources/Features/Terminal/TerminalViewContainer.swift` | TerminalViewContainer, viewDidMoveToWindow, layout, TerminalGlassView, updateTopInset (+8) |
| `ghostty/macos/Sources/Features/Terminal/TerminalRestorable.swift` | TerminalRestorable, encode, TerminalRestorableState, restoreWindow, restoreFocus |
| `ghostty/include/ghostty.h` | ghostty_app_update_config, ghostty_surface_update_config, ghostty_surface_set_focus, ghostty_surface_split_resize |
| `ghostty/macos/Tests/Terminal/TerminalViewContainerTests.swift` | MockTerminalViewContainer, MockConfig, glassAvailability, configChangeUpdatesGlass |
| `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | reloadConfig, splitResize, changeFontSize, completeClipboardRequest |
| `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | QuickTerminalController, windowDidBecomeKey, hide, toggleGhosttyFullScreen |
| `ghostty/macos/Sources/Features/Splits/SplitTree.swift` | inserting, removing, valuesPublisher |
| `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | ghosttyNewTab, newTab, closeAllWindows |

## Entry Points

Start here when exploring this area:

- **`treeDoesNotContainRemovedView`** (Function) — `ghostty/macos/Tests/Splits/SplitTreeTests.swift:90`
- **`removingNonexistentNodeLeavesTreeUnchanged`** (Function) — `ghostty/macos/Tests/Splits/SplitTreeTests.swift:97`
- **`newSplit`** (Function) — `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift:234`
- **`closeSurface`** (Function) — `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift:389`
- **`removeSurfaceNode`** (Function) — `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift:449`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `SurfaceView` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_UIKit.swift` | 5 |
| `MockTerminalViewContainer` | Class | `ghostty/macos/Tests/Terminal/TerminalViewContainerTests.swift` | 11 |
| `MockConfig` | Class | `ghostty/macos/Tests/Terminal/TerminalViewContainerTests.swift` | 22 |
| `Config` | Class | `ghostty/macos/Sources/Ghostty/Ghostty.Config.swift` | 740 |
| `TerminalViewContainer` | Class | `ghostty/macos/Sources/Features/Terminal/TerminalViewContainer.swift` | 5 |
| `CodableBridge` | Class | `ghostty/macos/Sources/Helpers/CodableBridge.swift` | 3 |
| `TerminalRestorableState` | Class | `ghostty/macos/Sources/Features/Terminal/TerminalRestorable.swift` | 42 |
| `TerminalGlassView` | Class | `ghostty/macos/Sources/Features/Terminal/TerminalViewContainer.swift` | 97 |
| `TabGroupCloseCoordinator` | Class | `ghostty/macos/Sources/Helpers/TabGroupCloseCoordinator.swift` | 8 |
| `BaseTerminalController` | Class | `ghostty/macos/Sources/Features/Terminal/TerminalViewContainer.swift` | 86 |
| `TerminalController` | Class | `ghostty/macos/Sources/Features/Terminal/TerminalController.swift` | 7 |
| `QuickTerminalController` | Class | `ghostty/macos/Sources/Features/QuickTerminal/QuickTerminalController.swift` | 6 |
| `BaseTerminalController` | Class | `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | 28 |
| `NSColor` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSColor+Extension.swift` | 2 |
| `ClipboardConfirmationController` | Class | `ghostty/macos/Sources/Features/ClipboardConfirmation/ClipboardConfirmationController.swift` | 8 |
| `treeDoesNotContainRemovedView` | Function | `ghostty/macos/Tests/Splits/SplitTreeTests.swift` | 90 |
| `removingNonexistentNodeLeavesTreeUnchanged` | Function | `ghostty/macos/Tests/Splits/SplitTreeTests.swift` | 97 |
| `newSplit` | Function | `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | 234 |
| `closeSurface` | Function | `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | 389 |
| `removeSurfaceNode` | Function | `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | 449 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `ConfigureTabContextMenuIfNeeded → SetFrame` | cross_community | 9 |
| `ApplicationDidFinishLaunching → SetFrame` | cross_community | 8 |
| `CloseAllWindows → SetFrame` | cross_community | 8 |
| `ConfigureTabContextMenuIfNeeded → SetInitialWindowPosition` | cross_community | 8 |
| `CloseAllWindows → SetInitialWindowPosition` | cross_community | 7 |
| `HandleCloseTab → SetFrame` | cross_community | 7 |
| `OpenTab → ModifierFlags` | cross_community | 7 |
| `OpenWindow → ModifierFlags` | cross_community | 7 |
| `ConfigureTabContextMenuIfNeeded → TerminalController` | cross_community | 7 |
| `ConfigureTabContextMenuIfNeeded → AddTabbedWindowSafely` | cross_community | 7 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Splits | 7 calls |
| Window Styles | 4 calls |
| Extensions | 4 calls |
| Include | 2 calls |
| Surface View | 2 calls |
| Cluster_208 | 2 calls |
| AppleScript | 2 calls |
| Cluster_8 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "treeDoesNotContainRemovedView"})` — see callers and callees
2. `gitnexus_query({query: "terminal"})` — find related execution flows
3. Read key files listed above for implementation details
