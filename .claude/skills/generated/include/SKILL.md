---
name: include
description: "Skill for the Include area of cmux-gtk. 92 symbols across 15 files."
---

# Include

92 symbols | 15 files | Cohesion: 74%

## When to Use

- Working with code in `ghostty/`
- Understanding how process_exited, get_config_color, get_config_f64 work
- Modifying include-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/include/ghostty.h` | ghostty_config_get, ghostty_surface_new, ghostty_surface_free, ghostty_surface_process_exited, ghostty_surface_draw (+28) |
| `ghostty-gtk/src/callbacks.rs` | write_clipboard_trampoline, c_string, handler_from_userdata, wakeup_trampoline, action_trampoline (+6) |
| `ghostty-gtk/src/surface.rs` | dispose, realize, render, create_surface, flush_pending_text (+5) |
| `ghostty-gtk/src/app.rs` | get_config_color, get_config_f64, tick, reload_config, needs_confirm_quit (+4) |
| `ghostty/macos/Sources/Ghostty/Ghostty.Inspector.swift` | setContentScale, setSize, metalRender, mouseScroll, metalInit |
| `ghostty/macos/Sources/Ghostty/Surface View/InspectorView.swift` | updateSize, viewDidChangeBackingProperties, draw, scrollWheel, surfaceViewDidChange |
| `ghostty/macos/Sources/Ghostty/Ghostty.App.swift` | appTick, wakeup, requestClose, splitEqualize, keyboardSelectionDidChange |
| `cmux/src/app.rs` | is_null, on_wakeup, get, on_action |
| `ghostty/macos/Sources/Features/Terminal/BaseTerminalController.swift` | close, equalizeSplits, windowDidChangeOcclusionState |
| `ghostty/macos/Sources/Ghostty/Ghostty.Config.swift` | loadConfig, keyboardShortcut |

## Entry Points

Start here when exploring this area:

- **`process_exited`** (Function) — `ghostty-gtk/src/surface.rs:1329`
- **`get_config_color`** (Function) — `ghostty-gtk/src/app.rs:170`
- **`get_config_f64`** (Function) — `ghostty-gtk/src/app.rs:198`
- **`ghostty_config_get`** (Function) — `ghostty/include/ghostty.h:1056`
- **`ghostty_surface_new`** (Function) — `ghostty/include/ghostty.h:1081`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `process_exited` | Function | `ghostty-gtk/src/surface.rs` | 1329 |
| `get_config_color` | Function | `ghostty-gtk/src/app.rs` | 170 |
| `get_config_f64` | Function | `ghostty-gtk/src/app.rs` | 198 |
| `ghostty_config_get` | Function | `ghostty/include/ghostty.h` | 1056 |
| `ghostty_surface_new` | Function | `ghostty/include/ghostty.h` | 1081 |
| `ghostty_surface_free` | Function | `ghostty/include/ghostty.h` | 1083 |
| `ghostty_surface_process_exited` | Function | `ghostty/include/ghostty.h` | 1089 |
| `ghostty_surface_draw` | Function | `ghostty/include/ghostty.h` | 1091 |
| `ghostty_inspector_set_content_scale` | Function | `ghostty/include/ghostty.h` | 1152 |
| `ghostty_inspector_set_size` | Function | `ghostty/include/ghostty.h` | 1153 |
| `ghostty_inspector_metal_render` | Function | `ghostty/include/ghostty.h` | 1171 |
| `setContentScale` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.Inspector.swift` | 28 |
| `setSize` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.Inspector.swift` | 34 |
| `metalRender` | Function | `ghostty/macos/Sources/Ghostty/Ghostty.Inspector.swift` | 87 |
| `updateSize` | Function | `ghostty/macos/Sources/Ghostty/Surface View/InspectorView.swift` | 165 |
| `viewDidChangeBackingProperties` | Function | `ghostty/macos/Sources/Ghostty/Surface View/InspectorView.swift` | 221 |
| `draw` | Function | `ghostty/macos/Sources/Ghostty/Surface View/InspectorView.swift` | 416 |
| `tick` | Function | `ghostty-gtk/src/app.rs` | 101 |
| `ghostty_app_tick` | Function | `ghostty/include/ghostty.h` | 1067 |
| `reload_config` | Function | `ghostty-gtk/src/app.rs` | 133 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Action → Ghostty_surface_userdata` | cross_community | 4 |
| `Dispatch → Is_null` | cross_community | 4 |
| `HandleSplit → Ghostty_surface_userdata` | cross_community | 4 |
| `Show_all_surfaces_search → Is_null` | cross_community | 4 |
| `Wakeup → Ghostty_app_tick` | cross_community | 3 |
| `Bind_shared_state_updates → Is_null` | cross_community | 3 |
| `ReadClipboard → Ghostty_surface_complete_clipboard_request` | cross_community | 3 |
| `Handle_notification_create → Is_null` | cross_community | 3 |
| `Handle_workspace_action → Is_null` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cluster_20 | 2 calls |
| Surface View | 1 calls |
| Cluster_2 | 1 calls |
| Ghostty | 1 calls |
| Cluster_6 | 1 calls |
| Terminal | 1 calls |
| V2 | 1 calls |
| Cluster_7 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "process_exited"})` — see callers and callees
2. `gitnexus_query({query: "include"})` — find related execution flows
3. Read key files listed above for implementation details
