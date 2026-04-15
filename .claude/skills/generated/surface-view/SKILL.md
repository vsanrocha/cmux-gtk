---
name: surface-view
description: "Skill for the Surface View area of cmux-gtk. 180 symbols across 34 files."
---

# Surface View

180 symbols | 34 files | Cohesion: 74%

## When to Use

- Working with code in `ghostty/`
- Understanding how surface_size, ghostty_surface_set_content_scale, ghostty_surface_set_size work
- Modifying surface view-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_AppKit.swift` | sizeDidChange, setSurfaceSize, windowDidChangeScreen, viewDidChangeBackingProperties, selectedRange (+60) |
| `ghostty/include/ghostty.h` | ghostty_surface_set_content_scale, ghostty_surface_set_size, ghostty_surface_size, ghostty_surface_set_display_id, ghostty_surface_ime_point (+18) |
| `ghostty/macos/Sources/Ghostty/Surface View/InspectorView.swift` | mouseDown, mouseUp, rightMouseDown, rightMouseUp, keyDown (+9) |
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceScrollView.swift` | SurfaceScrollView, layout, synchronizeSurfaceView, synchronizeCoreSurface, synchronizeScrollView (+5) |
| `ghostty-gtk/src/surface.rs` | resize, schedule_resize_focus_restore, surface_size, read_screen_text, read_scrollback_text (+4) |
| `ghostty/macos/Sources/Helpers/TabTitleEditor.swift` | beginEditing, tabTitleEditorFrame, sourceTabTitleLabel, applyTextStyle, hide (+2) |
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | ghosttyDidFocusSplit, ghosttyDidToggleSplitZoom, ghosttyDidPresentTerminal, performAction, localEventHandler (+1) |
| `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView.swift` | updateOSView, makeOSView, moveFocus, makeBody, backgroundColor |
| `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | addWindowButtonsBackdrop, addWindowDragHandle, WindowDragView, WindowButtonsBackdropView |
| `ghostty/macos/Sources/Ghostty/Ghostty.Inspector.swift` | mouseButton, key, setFocus, mousePos |

## Entry Points

Start here when exploring this area:

- **`surface_size`** (Function) — `ghostty-gtk/src/surface.rs:1343`
- **`ghostty_surface_set_content_scale`** (Function) — `ghostty/include/ghostty.h:1092`
- **`ghostty_surface_set_size`** (Function) — `ghostty/include/ghostty.h:1095`
- **`ghostty_surface_size`** (Function) — `ghostty/include/ghostty.h:1096`
- **`ghostty_surface_set_display_id`** (Function) — `ghostty/include/ghostty.h:1144`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `NSView` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSView+Extension.swift` | 3 |
| `SurfaceScrollView` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceScrollView.swift` | 14 |
| `SurfaceDragSourceView` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceDragSource.swift` | 81 |
| `WindowDragView` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 505 |
| `WindowButtonsBackdropView` | Class | `ghostty/macos/Sources/Features/Terminal/Window Styles/TitlebarTabsVenturaTerminalWindow.swift` | 534 |
| `NSMenu` | Class | `ghostty/macos/Sources/Helpers/Extensions/NSMenu+Extension.swift` | 2 |
| `Array` | Class | `ghostty/macos/Sources/Helpers/Extensions/Array+Extension.swift` | 0 |
| `MouseButton` | Class | `ghostty/macos/Sources/Ghostty/Ghostty.Input.swift` | 419 |
| `Transferable` | Class | `ghostty/macos/Sources/Helpers/Extensions/Transferable+Extension.swift` | 4 |
| `Ghostty` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView+Transferable.swift` | 7 |
| `SurfaceView` | Class | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView+Transferable.swift` | 7 |
| `InspectorView` | Class | `ghostty/macos/Sources/Ghostty/Surface View/InspectorView.swift` | 93 |
| `surface_size` | Function | `ghostty-gtk/src/surface.rs` | 1343 |
| `ghostty_surface_set_content_scale` | Function | `ghostty/include/ghostty.h` | 1092 |
| `ghostty_surface_set_size` | Function | `ghostty/include/ghostty.h` | 1095 |
| `ghostty_surface_size` | Function | `ghostty/include/ghostty.h` | 1096 |
| `ghostty_surface_set_display_id` | Function | `ghostty/include/ghostty.h` | 1144 |
| `sizeDidChange` | Function | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_UIKit.swift` | 105 |
| `didMoveToWindow` | Function | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_UIKit.swift` | 127 |
| `sizeDidChange` | Function | `ghostty/macos/Sources/Ghostty/Surface View/SurfaceView_AppKit.swift` | 477 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `HandleFocus → Apply` | cross_community | 7 |
| `Perform → Apply` | cross_community | 7 |
| `Perform → StoredPermission` | cross_community | 6 |
| `HandleFocus → Ghostty_surface_set_focus` | cross_community | 6 |
| `HandleFocus → ObjectIdentifier` | cross_community | 6 |
| `HandleFocus → Array` | cross_community | 6 |
| `Perform → Ghostty_surface_set_focus` | cross_community | 6 |
| `Perform → ObjectIdentifier` | cross_community | 6 |
| `Perform → Array` | cross_community | 6 |
| `LocalEventHandler → ModifierFlags` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Extensions | 8 calls |
| Include | 7 calls |
| Ghostty | 4 calls |
| Splits | 3 calls |
| Terminal | 2 calls |
| Cluster_6 | 2 calls |
| AppleScript | 2 calls |
| Cluster_2 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "surface_size"})` — see callers and callees
2. `gitnexus_query({query: "surface view"})` — find related execution flows
3. Read key files listed above for implementation details
