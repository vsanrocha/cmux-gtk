---
name: v2
description: "Skill for the V2 area of cmux-gtk. 192 symbols across 31 files."
---

# V2

192 symbols | 31 files | Cohesion: 77%

## When to Use

- Working with code in `cmux/`
- Understanding how set_close_handler, clear, entry_count work
- Modifying v2-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/socket/v2/workspace.rs` | handle_workspace_list, handle_workspace_new, handle_workspace_create, create_workspace, handle_workspace_create_ssh (+37) |
| `cmux/src/model/tab_manager.rs` | selected_index, selected, selected_id, selected_mut, select_by_id (+11) |
| `cmux/src/socket/v2/surface.rs` | handle_surface_send_input, handle_surface_list, handle_surface_current, handle_surface_focus, handle_surface_send_key (+11) |
| `cmux/src/model/workspace.rs` | truncate_str, insert_panel, panel, panel_mut, panel_ids (+8) |
| `cmux/src/socket/browser/queries.rs` | find_by_selector, handle_find, handle_find_all, handle_find_by_text, handle_find_by_role (+8) |
| `cmux/src/socket/v2/pane.rs` | handle_pane_new, handle_pane_list, handle_pane_focus, handle_pane_close, handle_pane_last (+7) |
| `cmux/src/socket/v2/mod.rs` | success, error, dispatch, test_notification_create_updates_workspace_attention, test_workspace_latest_unread_selects_newest_workspace (+5) |
| `cmux/src/app.rs` | lock_or_recover, send_input_to_panel, close_panel, install_ui_event_sender, remove_ui_event_sender (+4) |
| `cmux/src/model/panel.rs` | new_browser, new_markdown, find_pane_with_panel, find_pane_with_panel_readonly, select_panel (+4) |
| `cmux/src/ui/sidebar.rs` | refresh_sidebar, setup_row_drag_drop, setup_row_context_menu, show_custom_color_picker, show_rename_for_index (+2) |

## Entry Points

Start here when exploring this area:

- **`set_close_handler`** (Function) — `ghostty-gtk/src/surface.rs:1153`
- **`clear`** (Function) — `cmux/src/notifications.rs:117`
- **`entry_count`** (Function) — `cmux/src/browser_history.rs:260`
- **`lock_or_recover`** (Function) — `cmux/src/app.rs:16`
- **`send_input_to_panel`** (Function) — `cmux/src/app.rs:137`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `set_close_handler` | Function | `ghostty-gtk/src/surface.rs` | 1153 |
| `clear` | Function | `cmux/src/notifications.rs` | 117 |
| `entry_count` | Function | `cmux/src/browser_history.rs` | 260 |
| `lock_or_recover` | Function | `cmux/src/app.rs` | 16 |
| `send_input_to_panel` | Function | `cmux/src/app.rs` | 137 |
| `close_panel` | Function | `cmux/src/app.rs` | 160 |
| `install_ui_event_sender` | Function | `cmux/src/app.rs` | 343 |
| `remove_ui_event_sender` | Function | `cmux/src/app.rs` | 347 |
| `window_ids` | Function | `cmux/src/app.rs` | 352 |
| `send_ui_event` | Function | `cmux/src/app.rs` | 361 |
| `send_ui_event_to` | Function | `cmux/src/app.rs` | 367 |
| `notify_ui_refresh` | Function | `cmux/src/app.rs` | 373 |
| `refresh_sidebar` | Function | `cmux/src/ui/sidebar.rs` | 160 |
| `create_notifications_panel` | Function | `cmux/src/ui/notifications_panel.rs` | 16 |
| `show_all_surfaces_search` | Function | `cmux/src/ui/all_surfaces_search.rs` | 25 |
| `truncate_str` | Function | `cmux/src/model/workspace.rs` | 139 |
| `insert_panel` | Function | `cmux/src/model/workspace.rs` | 289 |
| `panel` | Function | `cmux/src/model/workspace.rs` | 372 |
| `panel_mut` | Function | `cmux/src/model/workspace.rs` | 378 |
| `panel_ids` | Function | `cmux/src/model/workspace.rs` | 383 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Create_window → RpcError` | cross_community | 6 |
| `Dispatch → ErrorInfo` | cross_community | 5 |
| `Create_window → Display_title` | cross_community | 5 |
| `Create_window → Lock_or_recover` | cross_community | 5 |
| `Create_window → Get_mut` | cross_community | 5 |
| `Handle_workspace_create_ssh → New_terminal` | cross_community | 5 |
| `Handle_workspace_create_ssh → Single_pane` | cross_community | 5 |
| `Handle_workspace_create_ssh → Get` | cross_community | 5 |
| `Dispatch → Is_null` | cross_community | 4 |
| `Dispatch → Lock_or_recover` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Model | 24 calls |
| Ui | 15 calls |
| Include | 7 calls |
| Window | 5 calls |
| Cluster_7 | 2 calls |
| Browser | 2 calls |
| Cluster_6 | 1 calls |
| Surface View | 1 calls |

## How to Explore

1. `gitnexus_context({name: "set_close_handler"})` — see callers and callees
2. `gitnexus_query({query: "v2"})` — find related execution flows
3. Read key files listed above for implementation details
