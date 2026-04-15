---
name: splits
description: "Skill for the Splits area of cmux-gtk. 116 symbols across 14 files."
---

# Splits

116 symbols | 14 files | Cohesion: 75%

## When to Use

- Working with code in `ghostty/`
- Understanding how topEdge, bottomEdge, leftEdge work
- Modifying splits-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Tests/Splits/SplitTreeTests.swift` | MockView, nonEmptyTreeIsNotEmpty, isNotSplit, treeContainsView, treeDoesNotContainView (+41) |
| `ghostty/macos/Sources/Features/Splits/SplitTree.swift` | doesBorder, contains, replacing, encode, path (+24) |
| `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | topEdge, bottomEdge, leftEdge, rightEdge, topLeftCornerSelectsLeft (+15) |
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | ghosttyDidResizeSplit, performSplitAction, splitDidResize, findNextFocusTargetAfterClosing, ghosttyDidEqualizeSplits |
| `ghostty/macos/Sources/Features/Services/ServiceProvider.swift` | openTab, openWindow, openTerminal |
| `ghostty/macos/Sources/Features/Splits/TerminalSplitTreeView.swift` | performDrop, calculate |
| `ghostty/macos/Sources/Helpers/TabGroupCloseCoordinator.swift` | windowShouldClose, trigger |
| `ghostty/macos/Sources/Features/AppleScript/ScriptWindow.swift` | stableID, valueInTerminals |
| `ghostty/macos/Sources/Features/AppleScript/ScriptTab.swift` | stableID, valueInTerminals |
| `ghostty/macos/Sources/Features/App Intents/NewTerminalIntent.swift` | perform |

## Entry Points

Start here when exploring this area:

- **`topEdge`** (Function) — `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift:9`
- **`bottomEdge`** (Function) — `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift:14`
- **`leftEdge`** (Function) — `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift:19`
- **`rightEdge`** (Function) — `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift:24`
- **`topLeftCornerSelectsLeft`** (Function) — `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift:33`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `MockView` | Class | `ghostty/macos/Tests/Splits/SplitTreeTests.swift` | 4 |
| `ObjectIdentifier` | Class | `ghostty/macos/Sources/Helpers/Extensions/ObjectIdentifier+Extension.swift` | 2 |
| `topEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 9 |
| `bottomEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 14 |
| `leftEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 19 |
| `rightEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 24 |
| `topLeftCornerSelectsLeft` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 33 |
| `topRightCornerSelectsRight` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 38 |
| `bottomLeftCornerSelectsLeft` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 43 |
| `bottomRightCornerSelectsRight` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 48 |
| `centerSelectsLeft` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 55 |
| `rectangularViewTopEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 62 |
| `rectangularViewLeftEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 68 |
| `tallRectangleTopEdge` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 74 |
| `pointLeftOfViewSelectsLeft` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 82 |
| `pointAboveViewSelectsTop` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 87 |
| `pointRightOfViewSelectsRight` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 92 |
| `pointBelowViewSelectsBottom` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 97 |
| `upperLeftTriangleSelectsLeft` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 104 |
| `upperRightTriangleSelectsRight` | Function | `ghostty/macos/Tests/Splits/TerminalSplitDropZoneTests.swift` | 110 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `OpenTab → ModifierFlags` | cross_community | 7 |
| `OpenWindow → ModifierFlags` | cross_community | 7 |
| `Perform → StoredPermission` | cross_community | 6 |
| `Perform → StoredPermission` | cross_community | 6 |
| `HandleFocus → ObjectIdentifier` | cross_community | 6 |
| `Perform → ObjectIdentifier` | cross_community | 6 |
| `OpenTab → SetFrame` | cross_community | 6 |
| `OpenTab → KeyEquivalent` | cross_community | 6 |
| `OpenTab → KeyboardShortcut` | cross_community | 6 |
| `OpenTab → EventModifiers` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ghostty | 4 calls |
| Terminal | 3 calls |
| App Intents | 2 calls |
| Tests | 1 calls |
| Surface View | 1 calls |
| QuickTerminal | 1 calls |

## How to Explore

1. `gitnexus_context({name: "topEdge"})` — see callers and callees
2. `gitnexus_query({query: "splits"})` — find related execution flows
3. Read key files listed above for implementation details
