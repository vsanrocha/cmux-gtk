---
name: window-styles
description: "Skill for the Window Styles area of cmux-gtk. 91 symbols across 19 files."
---

# Window Styles

91 symbols | 19 files | Cohesion: 79%

## When to Use

- Working with code in `ghostty/`
- Understanding how descendants, update, hideEffectView work
- Modifying window styles-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | layoutIfNeeded, update, updateConstraintsIfNeeded, updateNewTabButtonImage, updateTabsForVeryDarkBackgrounds (+19) |
| `ghostty/macos/Sources/Features/Terminal/Window Styles/TerminalWindow.swift` | isTabBar, syncAppearance, updateColorSchemeForSurfaceTree, generateResetZoomButton, awakeFromNib (+12) |
| `ghostty/macos/Sources/Features/Terminal/Window Styles/TransparentTitlebarTerminalWindow.swift` | update, hideEffectView, awakeFromNib, syncAppearance, syncAppearanceTahoe (+6) |
| `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsTahoeTerminalWindow.swift` | removeTitlebarAccessoryViewController, removeTabBar, awakeFromNib, TitlebarTabsTahoeTerminalWindow, becomeMain (+4) |
| `ghostty/macos/Sources/Helpers/Fullscreen.swift` | exit, exit, unhideDock, unhideMenu, Name |
| `ghostty/macos/Sources/Features/Terminal/Window Styles/HiddenTitlebarTerminalWindow.swift` | awakeFromNib, reapplyHiddenStyle, fullscreenDidExit, HiddenTitlebarTerminalWindow |
| `ghostty/macos/Sources/Helpers/Extensions/NSView+Extension.swift` | descendants, screenshot, firstSuperview |
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceScrollView.swift` | synchronizeAppearance, handleConfigChange, updateTrackingAreas |
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | splitZoom, promptTabTitle, changeTabTitle |
| `ghostty/macos/Sources/Helpers/Extensions/NSWindow+Extension.swift` | addTabbedWindowSafely, NSWindow |

## Entry Points

Start here when exploring this area:

- **`descendants`** (Function) — `ghostty/macos/Sources/Helpers/Extensions/NSView+Extension.swift:98`
- **`update`** (Function) — `ghostty/macos/Sources/Features/Terminal/Window Styles/TransparentTitlebarTerminalWindow.swift:45`
- **`hideEffectView`** (Function) — `ghostty/macos/Sources/Features/Terminal/Window Styles/TransparentTitlebarTerminalWindow.swift:192`
- **`layoutIfNeeded`** (Function) — `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift:71`
- **`update`** (Function) — `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift:81`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `TerminalToolbar` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 587 |
| `NSAppearance` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSAppearance+Extension.swift` | 2 |
| `NSImage` | Class | `ghostty/macos/GhosttyUITests/AppKitExtensions.swift` | 26 |
| `NonDraggableHostingView` | Class | `ghostty/macos/Sources/Helpers/NonDraggableHostingView.swift` | 10 |
| `Name` | Class | `ghostty/macos/Sources/Helpers/Fullscreen.swift` | 454 |
| `NSWindow` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSWindow+Extension.swift` | 2 |
| `TransparentTitlebarTerminalWindow` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TransparentTitlebarTerminalWindow.swift` | 4 |
| `TitlebarTabsVenturaTerminalWindow` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 3 |
| `TitlebarTabsTahoeTerminalWindow` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsTahoeTerminalWindow.swift` | 7 |
| `TerminalWindow` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TerminalWindow.swift` | 6 |
| `HiddenTitlebarTerminalWindow` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/HiddenTitlebarTerminalWindow.swift` | 2 |
| `NSToolbarItem` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 709 |
| `NSToolbarItem` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsTahoeTerminalWindow.swift` | 305 |
| `descendants` | Function | `ghostty/macos/Sources/Helpers/Extensions/NSView+Extension.swift` | 98 |
| `update` | Function | `ghostty/macos/Sources/Features/Terminal/Window Styles/TransparentTitlebarTerminalWindow.swift` | 45 |
| `hideEffectView` | Function | `ghostty/macos/Sources/Features/Terminal/Window Styles/TransparentTitlebarTerminalWindow.swift` | 192 |
| `layoutIfNeeded` | Function | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 71 |
| `update` | Function | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 81 |
| `updateConstraintsIfNeeded` | Function | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 120 |
| `updateNewTabButtonImage` | Function | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 207 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `ConfigureTabContextMenuIfNeeded → SetFrame` | cross_community | 9 |
| `CloseAllWindows → SetFrame` | cross_community | 8 |
| `ConfigureTabContextMenuIfNeeded → SetInitialWindowPosition` | cross_community | 8 |
| `CloseAllWindows → SetInitialWindowPosition` | cross_community | 7 |
| `HandleCloseTab → SetFrame` | cross_community | 7 |
| `ConfigureTabContextMenuIfNeeded → TerminalController` | cross_community | 7 |
| `ConfigureTabContextMenuIfNeeded → AddTabbedWindowSafely` | cross_community | 7 |
| `CloseAllWindows → TerminalController` | cross_community | 6 |
| `CloseAllWindows → AddTabbedWindowSafely` | cross_community | 6 |
| `HandleCloseWindow → SetFrame` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Terminal | 5 calls |
| Surface View | 4 calls |
| Extensions | 3 calls |
| Cluster_195 | 1 calls |
| Tests | 1 calls |

## How to Explore

1. `gitnexus_context({name: "descendants"})` — see callers and callees
2. `gitnexus_query({query: "window styles"})` — find related execution flows
3. Read key files listed above for implementation details
