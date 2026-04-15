---
name: browser
description: "Skill for the Browser area of cmux-gtk. 87 symbols across 7 files."
---

# Browser

87 symbols | 7 files | Cohesion: 70%

## When to Use

- Working with code in `cmux/`
- Understanding how handle_viewport_set, handle_download_wait, handle_open_split work
- Modifying browser-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/socket/browser/queries.rs` | handle_get_html, handle_get_value, handle_get_attribute, handle_get_property, handle_get_bounding_box (+24) |
| `cmux/src/socket/browser/interaction.rs` | handle_click, handle_dblclick, handle_hover, handle_type, handle_fill (+16) |
| `cmux/src/socket/browser/tabs.rs` | handle_viewport_set, handle_download_wait, handle_open_split, handle_focus_webview, handle_is_webview_focused (+12) |
| `cmux/src/socket/browser/navigation.rs` | handle_wait_for_selector, handle_execute_js, handle_get_url, handle_get_text, handle_screenshot (+8) |
| `cmux/src/socket/browser/helpers.rs` | send_eval_action, require_selector, recv_with_timeout, send_action_with_reply, send_action |
| `cmux/src/socket/browser/mod.rs` | dispatch |
| `cmux/src/ui/browser_panel/registry.rs` | resolve_selector |

## Entry Points

Start here when exploring this area:

- **`handle_viewport_set`** (Function) — `cmux/src/socket/browser/tabs.rs:128`
- **`handle_download_wait`** (Function) — `cmux/src/socket/browser/tabs.rs:151`
- **`handle_open_split`** (Function) — `cmux/src/socket/browser/tabs.rs:194`
- **`handle_focus_webview`** (Function) — `cmux/src/socket/browser/tabs.rs:200`
- **`handle_is_webview_focused`** (Function) — `cmux/src/socket/browser/tabs.rs:210`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `handle_viewport_set` | Function | `cmux/src/socket/browser/tabs.rs` | 128 |
| `handle_download_wait` | Function | `cmux/src/socket/browser/tabs.rs` | 151 |
| `handle_open_split` | Function | `cmux/src/socket/browser/tabs.rs` | 194 |
| `handle_focus_webview` | Function | `cmux/src/socket/browser/tabs.rs` | 200 |
| `handle_is_webview_focused` | Function | `cmux/src/socket/browser/tabs.rs` | 210 |
| `handle_state_save` | Function | `cmux/src/socket/browser/tabs.rs` | 224 |
| `handle_state_load` | Function | `cmux/src/socket/browser/tabs.rs` | 237 |
| `handle_network_route` | Function | `cmux/src/socket/browser/tabs.rs` | 274 |
| `handle_network_unroute` | Function | `cmux/src/socket/browser/tabs.rs` | 286 |
| `handle_network_requests` | Function | `cmux/src/socket/browser/tabs.rs` | 295 |
| `handle_trace_start` | Function | `cmux/src/socket/browser/tabs.rs` | 308 |
| `handle_trace_stop` | Function | `cmux/src/socket/browser/tabs.rs` | 320 |
| `handle_screencast_start` | Function | `cmux/src/socket/browser/tabs.rs` | 325 |
| `handle_screencast_stop` | Function | `cmux/src/socket/browser/tabs.rs` | 337 |
| `handle_frame_select` | Function | `cmux/src/socket/browser/tabs.rs` | 350 |
| `handle_frame_main` | Function | `cmux/src/socket/browser/tabs.rs` | 366 |
| `handle_get_html` | Function | `cmux/src/socket/browser/queries.rs` | 52 |
| `handle_get_value` | Function | `cmux/src/socket/browser/queries.rs` | 70 |
| `handle_get_attribute` | Function | `cmux/src/socket/browser/queries.rs` | 82 |
| `handle_get_property` | Function | `cmux/src/socket/browser/queries.rs` | 102 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Dispatch → ErrorInfo` | cross_community | 5 |
| `Dispatch → Is_null` | cross_community | 4 |
| `Dispatch → Lock_or_recover` | cross_community | 4 |
| `Dispatch → Recv_with_timeout` | cross_community | 4 |
| `Dispatch → Success` | cross_community | 4 |
| `Handle_find → ErrorInfo` | cross_community | 4 |
| `Handle_find_all → ErrorInfo` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| V2 | 61 calls |

## How to Explore

1. `gitnexus_context({name: "handle_viewport_set"})` — see callers and callees
2. `gitnexus_query({query: "browser"})` — find related execution flows
3. Read key files listed above for implementation details
