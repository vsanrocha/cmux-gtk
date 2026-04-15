---
name: ghosttyuitests
description: "Skill for the GhosttyUITests area of cmux-gtk. 37 symbols across 6 files."
---

# GhosttyUITests

37 symbols | 6 files | Cohesion: 88%

## When to Use

- Working with code in `ghostty/`
- Understanding how testWindowCascading, testDragSplitWindowPosition, testDragSplitWindowPositionWithFixedSize work
- Modifying ghosttyuitests-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | testWindowCascading, testDragSplitWindowPosition, testDragSplitWindowPositionWithFixedSize, testConfigOverridesCachedPositionAndSize, testSizeOnlyConfigPreservesPosition (+6) |
| `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | assertTitlebarAppearance, testIssue8282, testLightTransparentWindowThemeWithDarkTerminal, testLightNativeWindowThemeWithDarkTerminal, testReloadingLightTransparentWindowTheme (+6) |
| `ghostty/macos/GhosttyUITests/GhosttyTitlebarTabsUITests.swift` | setUp, testCustomTitlebar, GhosttyTitlebarTabsUITests, testTabsGeometryInNormalWindow, testTabsGeometryInFullscreen (+3) |
| `ghostty/macos/GhosttyUITests/GhosttyTitleUITests.swift` | setUp, testTitle, GhosttyTitleUITests |
| `ghostty/macos/GhosttyUITests/GhosttyCustomConfigCase.swift` | updateConfig, ghosttyApplication, GhosttyCustomConfigCase |
| `ghostty/macos/GhosttyUITests/AppKitExtensions.swift` | colorAt |

## Entry Points

Start here when exploring this area:

- **`testWindowCascading`** (Function) — `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift:14`
- **`testDragSplitWindowPosition`** (Function) — `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift:75`
- **`testDragSplitWindowPositionWithFixedSize`** (Function) — `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift:130`
- **`testConfigOverridesCachedPositionAndSize`** (Function) — `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift:187`
- **`testSizeOnlyConfigPreservesPosition`** (Function) — `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift:235`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `GhosttyWindowPositionUITests` | Class | `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | 9 |
| `GhosttyTitlebarTabsUITests` | Class | `ghostty/macos/GhosttyUITests/GhosttyTitlebarTabsUITests.swift` | 9 |
| `GhosttyTitleUITests` | Class | `ghostty/macos/GhosttyUITests/GhosttyTitleUITests.swift` | 9 |
| `GhosttyThemeTests` | Class | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 10 |
| `GhosttyCustomConfigCase` | Class | `ghostty/macos/GhosttyUITests/GhosttyCustomConfigCase.swift` | 9 |
| `testWindowCascading` | Function | `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | 14 |
| `testDragSplitWindowPosition` | Function | `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | 75 |
| `testDragSplitWindowPositionWithFixedSize` | Function | `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | 130 |
| `testConfigOverridesCachedPositionAndSize` | Function | `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | 187 |
| `testSizeOnlyConfigPreservesPosition` | Function | `ghostty/macos/GhosttyUITests/GhosttyWindowPositionUITests.swift` | 235 |
| `setUp` | Function | `ghostty/macos/GhosttyUITests/GhosttyTitlebarTabsUITests.swift` | 10 |
| `testCustomTitlebar` | Function | `ghostty/macos/GhosttyUITests/GhosttyTitlebarTabsUITests.swift` | 21 |
| `setUp` | Function | `ghostty/macos/GhosttyUITests/GhosttyTitleUITests.swift` | 10 |
| `testTitle` | Function | `ghostty/macos/GhosttyUITests/GhosttyTitleUITests.swift` | 15 |
| `assertTitlebarAppearance` | Function | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 12 |
| `testIssue8282` | Function | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 38 |
| `testLightTransparentWindowThemeWithDarkTerminal` | Function | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 56 |
| `testLightNativeWindowThemeWithDarkTerminal` | Function | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 65 |
| `testReloadingLightTransparentWindowTheme` | Function | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 73 |
| `testSwitchingSystemTheme` | Function | `ghostty/macos/GhosttyUITests/GhosttyThemeTests.swift` | 87 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Extensions | 1 calls |

## How to Explore

1. `gitnexus_context({name: "testWindowCascading"})` — see callers and callees
2. `gitnexus_query({query: "ghosttyuitests"})` — find related execution flows
3. Read key files listed above for implementation details
