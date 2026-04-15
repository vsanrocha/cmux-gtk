---
name: model
description: "Skill for the Model area of cmux-gtk. 74 symbols across 7 files."
---

# Model

74 symbols | 7 files | Cohesion: 68%

## When to Use

- Working with code in `cmux/`
- Understanding how to_layout, new, empty work
- Modifying model-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/model/tab_manager.rs` | new, empty, select, add_workspace, close_below (+19) |
| `cmux/src/model/panel.rs` | new_terminal, all_panel_ids, remove_panel, set_divider_position_for_split, resize_panel (+19) |
| `cmux/src/model/workspace.rs` | new, split, set_status, record_notification, notification_summary (+15) |
| `cmux/src/app.rs` | cleanup_scrollback_temp_files, restore_session |
| `cmux/src/ui/split_view.rs` | build_layout, build_split |
| `cmux/src/session/snapshot.rs` | to_layout |
| `cmux/src/ui/command_palette.rs` | execute_action |

## Entry Points

Start here when exploring this area:

- **`to_layout`** (Function) — `cmux/src/session/snapshot.rs:184`
- **`new`** (Function) — `cmux/src/model/tab_manager.rs:17`
- **`empty`** (Function) — `cmux/src/model/tab_manager.rs:26`
- **`select`** (Function) — `cmux/src/model/tab_manager.rs:64`
- **`add_workspace`** (Function) — `cmux/src/model/tab_manager.rs:129`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `to_layout` | Function | `cmux/src/session/snapshot.rs` | 184 |
| `new` | Function | `cmux/src/model/tab_manager.rs` | 17 |
| `empty` | Function | `cmux/src/model/tab_manager.rs` | 26 |
| `select` | Function | `cmux/src/model/tab_manager.rs` | 64 |
| `add_workspace` | Function | `cmux/src/model/tab_manager.rs` | 129 |
| `close_below` | Function | `cmux/src/model/tab_manager.rs` | 323 |
| `new` | Function | `cmux/src/model/workspace.rs` | 153 |
| `split` | Function | `cmux/src/model/workspace.rs` | 209 |
| `set_status` | Function | `cmux/src/model/workspace.rs` | 398 |
| `record_notification` | Function | `cmux/src/model/workspace.rs` | 603 |
| `new_terminal` | Function | `cmux/src/model/panel.rs` | 47 |
| `build_layout` | Function | `cmux/src/ui/split_view.rs` | 31 |
| `remove_panel` | Function | `cmux/src/model/workspace.rs` | 252 |
| `detach_panel` | Function | `cmux/src/model/workspace.rs` | 269 |
| `drag_to_split` | Function | `cmux/src/model/workspace.rs` | 327 |
| `all_panel_ids` | Function | `cmux/src/model/panel.rs` | 211 |
| `remove_panel` | Function | `cmux/src/model/panel.rs` | 276 |
| `set_divider_position_for_split` | Function | `cmux/src/model/panel.rs` | 308 |
| `resize_panel` | Function | `cmux/src/model/panel.rs` | 344 |
| `prev_panel_id` | Function | `cmux/src/model/panel.rs` | 384 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Simulate → New` | cross_community | 5 |
| `Handle_workspace_create_ssh → New_terminal` | cross_community | 5 |
| `Handle_workspace_create_ssh → Single_pane` | cross_community | 5 |
| `Handle_workspace_create_ssh → Get` | cross_community | 5 |
| `Setup_shortcuts → All_panel_ids` | cross_community | 4 |
| `Handle_tab_action → Get` | cross_community | 4 |
| `Handle_surface_move → Get` | cross_community | 4 |
| `Handle_pane_break → Get` | cross_community | 4 |
| `Handle_pane_join → Get` | cross_community | 4 |
| `Handle_surface_action → Get` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| V2 | 24 calls |
| Session | 1 calls |
| Cluster_7 | 1 calls |
| Ui | 1 calls |
| Window | 1 calls |

## How to Explore

1. `gitnexus_context({name: "to_layout"})` — see callers and callees
2. `gitnexus_query({query: "model"})` — find related execution flows
3. Read key files listed above for implementation details
