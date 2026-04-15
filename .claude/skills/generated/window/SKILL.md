---
name: window
description: "Skill for the Window area of cmux-gtk. 33 symbols across 16 files."
---

# Window

33 symbols | 16 files | Cohesion: 54%

## When to Use

- Working with code in `cmux/`
- Understanding how binding_action, set_title, prune_terminal_cache work
- Modifying window-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/ui/search_overlay.rs` | create_search_overlay, do_search_action, do_search_needle, trigger_find_next, trigger_find_prev |
| `cmux/src/app.rs` | prune_terminal_cache, push_closed_browser_url, cleanup_stale_remote_sessions, open_window |
| `cmux/src/ui/window/mod.rs` | create_window, rebuild_content, refresh_ui, bind_sidebar_selection |
| `cmux/src/model/tab_manager.rs` | add_workspace_at_top, add_workspace_after_current, add_workspace_with_placement |
| `cmux/src/ui/window/event_handler.rs` | select_workspace_by_index, select_latest_unread, mark_workspace_read |
| `ghostty-gtk/src/surface.rs` | binding_action, set_title |
| `cmux/src/ui/window/dialogs.rs` | show_rename_dialog, show_ssh_dialog |
| `cmux/src/ui/browser_panel/registry.rs` | stop_all_webviews, toggle_console |
| `cmux/src/ui/welcome.rs` | should_show_welcome |
| `cmux/src/ui/sidebar.rs` | create_sidebar |

## Entry Points

Start here when exploring this area:

- **`binding_action`** (Function) — `ghostty-gtk/src/surface.rs:889`
- **`set_title`** (Function) — `ghostty-gtk/src/surface.rs:1308`
- **`prune_terminal_cache`** (Function) — `cmux/src/app.rs:178`
- **`push_closed_browser_url`** (Function) — `cmux/src/app.rs:378`
- **`cleanup_stale_remote_sessions`** (Function) — `cmux/src/app.rs:397`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `binding_action` | Function | `ghostty-gtk/src/surface.rs` | 889 |
| `set_title` | Function | `ghostty-gtk/src/surface.rs` | 1308 |
| `prune_terminal_cache` | Function | `cmux/src/app.rs` | 178 |
| `push_closed_browser_url` | Function | `cmux/src/app.rs` | 378 |
| `cleanup_stale_remote_sessions` | Function | `cmux/src/app.rs` | 397 |
| `open_window` | Function | `cmux/src/app.rs` | 576 |
| `should_show_welcome` | Function | `cmux/src/ui/welcome.rs` | 6 |
| `create_sidebar` | Function | `cmux/src/ui/sidebar.rs` | 21 |
| `show_settings` | Function | `cmux/src/ui/settings.rs` | 13 |
| `create_search_overlay` | Function | `cmux/src/ui/search_overlay.rs` | 26 |
| `trigger_find_next` | Function | `cmux/src/ui/search_overlay.rs` | 202 |
| `trigger_find_prev` | Function | `cmux/src/ui/search_overlay.rs` | 210 |
| `session_file_exists` | Function | `cmux/src/session/store.rs` | 24 |
| `clear_attention` | Function | `cmux/src/model/workspace.rs` | 621 |
| `add_workspace_at_top` | Function | `cmux/src/model/tab_manager.rs` | 137 |
| `add_workspace_after_current` | Function | `cmux/src/model/tab_manager.rs` | 146 |
| `add_workspace_with_placement` | Function | `cmux/src/model/tab_manager.rs` | 155 |
| `text` | Function | `ghostty/macos/Sources/Ghostty/GhosttyPackage.swift` | 260 |
| `install_css` | Function | `cmux/src/ui/window/styling.rs` | 4 |
| `setup_shortcuts` | Function | `cmux/src/ui/window/shortcuts.rs` | 15 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Create_window → RpcError` | cross_community | 6 |
| `Create_window → Display_title` | cross_community | 5 |
| `Create_window → Lock_or_recover` | cross_community | 5 |
| `Create_window → Get_mut` | cross_community | 5 |
| `Bind_shared_state_updates → Config_dir` | cross_community | 4 |
| `Setup_shortcuts → All_panel_ids` | cross_community | 4 |
| `Create_browser_widget_with_profile → Text` | cross_community | 4 |
| `Create_window → Error` | cross_community | 4 |
| `Create_window → Selected_index` | cross_community | 4 |
| `Bind_shared_state_updates → Set_title` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| V2 | 45 calls |
| Model | 11 calls |
| Ui | 10 calls |
| Settings | 2 calls |
| Include | 1 calls |
| Surface View | 1 calls |
| Cluster_7 | 1 calls |
| Remote | 1 calls |

## How to Explore

1. `gitnexus_context({name: "binding_action"})` — see callers and callees
2. `gitnexus_query({query: "window"})` — find related execution flows
3. Read key files listed above for implementation details
