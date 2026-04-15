---
name: socket
description: "Skill for the Socket area of cmux-gtk. 30 symbols across 3 files."
---

# Socket

30 symbols | 3 files | Cohesion: 90%

## When to Use

- Working with code in `cmux/`
- Understanding how dispatch, verify_hmac, compute_hmac_sha256 work
- Modifying socket-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/socket/auth.rs` | verify_hmac, compute_hmac_sha256, hex_encode, verify_hmac_raw, hmac_known_vector (+9) |
| `cmux/src/socket/v1.rs` | target, dispatch, parse_args, test_parse_args, test_parse_quoted_args (+7) |
| `cmux/src/socket/server.rs` | run_socket_server, handle_client, is_stale_socket, write_pid_file |

## Entry Points

Start here when exploring this area:

- **`dispatch`** (Function) — `cmux/src/socket/v1.rs:31`
- **`verify_hmac`** (Function) — `cmux/src/socket/auth.rs:67`
- **`compute_hmac_sha256`** (Function) — `cmux/src/socket/auth.rs:91`
- **`hex_encode`** (Function) — `cmux/src/socket/auth.rs:102`
- **`verify_hmac_raw`** (Function) — `cmux/src/socket/auth.rs:125`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `dispatch` | Function | `cmux/src/socket/v1.rs` | 31 |
| `verify_hmac` | Function | `cmux/src/socket/auth.rs` | 67 |
| `compute_hmac_sha256` | Function | `cmux/src/socket/auth.rs` | 91 |
| `hex_encode` | Function | `cmux/src/socket/auth.rs` | 102 |
| `verify_hmac_raw` | Function | `cmux/src/socket/auth.rs` | 125 |
| `is_v1` | Function | `cmux/src/socket/v1.rs` | 25 |
| `run_socket_server` | Function | `cmux/src/socket/server.rs` | 57 |
| `authenticate_peer` | Function | `cmux/src/socket/auth.rs` | 17 |
| `from_env` | Function | `cmux/src/socket/auth.rs` | 52 |
| `is_same_user` | Function | `cmux/src/socket/auth.rs` | 28 |
| `is_authorized` | Function | `cmux/src/socket/auth.rs` | 140 |
| `target` | Function | `cmux/src/socket/v1.rs` | 15 |
| `parse_args` | Function | `cmux/src/socket/v1.rs` | 776 |
| `test_parse_args` | Function | `cmux/src/socket/v1.rs` | 840 |
| `test_parse_quoted_args` | Function | `cmux/src/socket/v1.rs` | 848 |
| `test_git_branch_dirty_star` | Function | `cmux/src/socket/v1.rs` | 855 |
| `test_git_branch_clean` | Function | `cmux/src/socket/v1.rs` | 870 |
| `test_git_branch_dirty_flag` | Function | `cmux/src/socket/v1.rs` | 883 |
| `test_git_branch_with_panel` | Function | `cmux/src/socket/v1.rs` | 895 |
| `test_pr_checks_parse` | Function | `cmux/src/socket/v1.rs` | 902 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Main → From_env` | cross_community | 4 |
| `Main → Socket_path` | cross_community | 4 |
| `Main → Is_stale_socket` | cross_community | 4 |
| `Main → Write_pid_file` | cross_community | 4 |
| `Start → Compute_hmac_sha256` | cross_community | 4 |
| `Start → Hex_encode` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Remote | 1 calls |
| V2 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "dispatch"})` — see callers and callees
2. `gitnexus_query({query: "socket"})` — find related execution flows
3. Read key files listed above for implementation details
