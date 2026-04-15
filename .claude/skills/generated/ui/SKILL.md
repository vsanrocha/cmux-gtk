---
name: ui
description: "Skill for the Ui area of cmux-gtk. 49 symbols across 18 files."
---

# Ui

49 symbols | 18 files | Cohesion: 54%

## When to Use

- Working with code in `cmux/`
- Understanding how build_welcome, build_omnibar, build_omnibar_full work
- Modifying ui-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/ui/omnibar.rs` | is_externally_suppressed, build_omnibar, build_omnibar_full, populate_suggestions, build_search_suggestion_row (+4) |
| `cmux/src/ui/command_palette.rs` | show_command_palette, populate_list, fuzzy_match, shortcut_for_action, build_actions (+1) |
| `cmux/src/ui/terminal_panel.rs` | show_vim_badge, hide_vim_badge, create_panel_widget, create_browser_widget, create_markdown_widget |
| `cmux/src/model/workspace.rs` | with_directory, test_with_directory_updates_initial_terminal_panel, display_title, sidebar_status_label |
| `cmux/src/ui/markdown_panel.rs` | create_markdown_widget, load_markdown_file, render_markdown |
| `cmux/src/app.rs` | pop_closed_browser_url, get_cached_browser, cache_browser |
| `cmux/src/notifications.rs` | all, mark_read, test_unread_count |
| `cmux/src/ui/sidebar.rs` | create_workspace_row, workspace_meta_text, compact_path |
| `ghostty-gtk/src/surface.rs` | raw_surface, refresh |
| `cmux/src/ui/notifications_panel.rs` | refresh, format_timestamp |

## Entry Points

Start here when exploring this area:

- **`build_welcome`** (Function) — `cmux/src/ui/welcome.rs:13`
- **`build_omnibar`** (Function) — `cmux/src/ui/omnibar.rs:47`
- **`build_omnibar_full`** (Function) — `cmux/src/ui/omnibar.rs:55`
- **`create_markdown_widget`** (Function) — `cmux/src/ui/markdown_panel.rs:16`
- **`show_command_palette`** (Function) — `cmux/src/ui/command_palette.rs:24`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `build_welcome` | Function | `cmux/src/ui/welcome.rs` | 13 |
| `build_omnibar` | Function | `cmux/src/ui/omnibar.rs` | 47 |
| `build_omnibar_full` | Function | `cmux/src/ui/omnibar.rs` | 55 |
| `create_markdown_widget` | Function | `cmux/src/ui/markdown_panel.rs` | 16 |
| `show_command_palette` | Function | `cmux/src/ui/command_palette.rs` | 24 |
| `new` | Function | `cmux/src/remote/rpc.rs` | 71 |
| `raw_surface` | Function | `ghostty-gtk/src/surface.rs` | 845 |
| `refresh` | Function | `ghostty-gtk/src/surface.rs` | 850 |
| `pop_closed_browser_url` | Function | `cmux/src/app.rs` | 387 |
| `ghostty_surface_refresh` | Function | `ghostty/include/ghostty.h` | 1090 |
| `should_open_externally` | Function | `cmux/src/settings/mod.rs` | 502 |
| `show_vim_badge` | Function | `cmux/src/ui/terminal_panel.rs` | 26 |
| `hide_vim_badge` | Function | `cmux/src/ui/terminal_panel.rs` | 35 |
| `with_directory` | Function | `cmux/src/model/workspace.rs` | 192 |
| `detect_git_branch` | Function | `cmux/src/ui/window/styling.rs` | 430 |
| `bind_shared_state_updates` | Function | `cmux/src/ui/window/event_handler.rs` | 12 |
| `get_cached_browser` | Function | `cmux/src/app.rs` | 197 |
| `cache_browser` | Function | `cmux/src/app.rs` | 202 |
| `create_panel_widget` | Function | `cmux/src/ui/terminal_panel.rs` | 52 |
| `build_zoomed` | Function | `cmux/src/ui/split_view.rs` | 15 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Create_window → RpcError` | cross_community | 6 |
| `Create_browser_widget_with_profile → RpcError` | cross_community | 5 |
| `Create_browser_widget_with_profile → Error` | cross_community | 5 |
| `Create_window → Display_title` | cross_community | 5 |
| `Handle_workspace_create_ssh → New_terminal` | cross_community | 5 |
| `Handle_workspace_create_ssh → Single_pane` | cross_community | 5 |
| `GhosttyConfigDidChange → Display` | cross_community | 4 |
| `Bind_shared_state_updates → New` | cross_community | 4 |
| `Bind_shared_state_updates → Background_hex` | cross_community | 4 |
| `Bind_shared_state_updates → Config_dir` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| V2 | 24 calls |
| Window | 8 calls |
| Model | 5 calls |
| Surface View | 3 calls |
| Cluster_33 | 2 calls |
| Settings | 2 calls |
| Browser_panel | 2 calls |
| Cluster_26 | 2 calls |

## How to Explore

1. `gitnexus_context({name: "build_welcome"})` — see callers and callees
2. `gitnexus_query({query: "ui"})` — find related execution flows
3. Read key files listed above for implementation details
