---
name: update
description: "Skill for the Update area of cmux-gtk. 34 symbols across 6 files."
---

# Update

34 symbols | 6 files | Cohesion: 92%

## When to Use

- Working with code in `ghostty/`
- Understanding how testIdleText, testPermissionRequestText, testCheckingText work
- Modifying update-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | simulate, simulateHappyPath, simulateNotFound, simulateError, simulateSlowDownload (+9) |
| `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | testIdleText, testPermissionRequestText, testCheckingText, testDownloadingTextWithKnownLength, testDownloadingTextWithUnknownLength (+8) |
| `ghostty/macos/Sources/Features/Update/UpdateViewModel.swift` | UpdateViewModel, cancel, confirm |
| `ghostty/macos/Sources/Features/Update/UpdateController.swift` | checkForUpdates, installUpdate |
| `ghostty/macos/Sources/Features/Update/UpdateDriver.swift` | handleTerminalWindowWillClose |
| `ghostty/macos/Sources/App/macOS/AppDelegate.swift` | checkForUpdates |

## Entry Points

Start here when exploring this area:

- **`testIdleText`** (Function) — `ghostty/macos/Tests/Update/UpdateViewModelTests.swift:9`
- **`testPermissionRequestText`** (Function) — `ghostty/macos/Tests/Update/UpdateViewModelTests.swift:15`
- **`testCheckingText`** (Function) — `ghostty/macos/Tests/Update/UpdateViewModelTests.swift:22`
- **`testDownloadingTextWithKnownLength`** (Function) — `ghostty/macos/Tests/Update/UpdateViewModelTests.swift:28`
- **`testDownloadingTextWithUnknownLength`** (Function) — `ghostty/macos/Tests/Update/UpdateViewModelTests.swift:34`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `UpdateViewModel` | Class | `ghostty/macos/Sources/Features/Update/UpdateViewModel.swift` | 4 |
| `testIdleText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 9 |
| `testPermissionRequestText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 15 |
| `testCheckingText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 22 |
| `testDownloadingTextWithKnownLength` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 28 |
| `testDownloadingTextWithUnknownLength` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 34 |
| `testDownloadingTextWithZeroExpectedLength` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 40 |
| `testExtractingText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 46 |
| `testInstallingText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 52 |
| `testNotFoundText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 60 |
| `testErrorText` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 66 |
| `testMaxWidthTextForDownloading` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 75 |
| `testMaxWidthTextForExtracting` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 81 |
| `testMaxWidthTextForNonProgressState` | Function | `ghostty/macos/Tests/Update/UpdateViewModelTests.swift` | 87 |
| `simulate` | Function | `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | 36 |
| `simulateHappyPath` | Function | `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | 59 |
| `simulateNotFound` | Function | `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | 78 |
| `simulateError` | Function | `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | 94 |
| `simulateSlowDownload` | Function | `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | 114 |
| `simulateSlowDownloadProgress` | Function | `ghostty/macos/Sources/Features/Update/UpdateSimulator.swift` | 133 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Simulate → Double` | cross_community | 6 |
| `Simulate → SimulateInstalling` | intra_community | 6 |
| `Simulate → New` | cross_community | 5 |
| `Simulate → Downloading` | intra_community | 5 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Model | 3 calls |
| Ghostty | 1 calls |

## How to Explore

1. `gitnexus_context({name: "testIdleText"})` — see callers and callees
2. `gitnexus_query({query: "update"})` — find related execution flows
3. Read key files listed above for implementation details
