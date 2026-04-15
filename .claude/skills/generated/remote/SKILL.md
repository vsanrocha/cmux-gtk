---
name: remote
description: "Skill for the Remote area of cmux-gtk. 51 symbols across 8 files."
---

# Remote

51 symbols | 8 files | Cohesion: 83%

## When to Use

- Working with code in `cmux/`
- Understanding how is_alive, call, proxy_open work
- Modifying remote-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `cmux/src/remote/bootstrap.rs` | probe_platform, remote_daemon_path, check_remote_binary, upload_daemon, bootstrap_daemon (+6) |
| `cmux/src/remote/session.rs` | daemon_path, new, start, ssh_args, config (+5) |
| `cmux/src/remote/rpc.rs` | is_alive, call, proxy_open, proxy_write, proxy_close (+4) |
| `cmux/src/remote/relay.rs` | start, handle_relay_connection, read_limited_line, forward_to_socket, start_reverse_tunnel (+4) |
| `cmux/src/remote/proxy.rs` | handle_proxy_connection, handle_socks5, handle_http_connect, relay_streams, start (+3) |
| `cmux/src/socket/server.rs` | socket_path, cleanup |
| `cmux/src/socket/auth.rs` | hex_decode |
| `ghostty/macos/Sources/Ghostty/Ghostty.Shell.swift` | escape |

## Entry Points

Start here when exploring this area:

- **`is_alive`** (Function) — `cmux/src/remote/rpc.rs:240`
- **`call`** (Function) — `cmux/src/remote/rpc.rs:245`
- **`proxy_open`** (Function) — `cmux/src/remote/rpc.rs:330`
- **`proxy_write`** (Function) — `cmux/src/remote/rpc.rs:342`
- **`proxy_close`** (Function) — `cmux/src/remote/rpc.rs:352`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `is_alive` | Function | `cmux/src/remote/rpc.rs` | 240 |
| `call` | Function | `cmux/src/remote/rpc.rs` | 245 |
| `proxy_open` | Function | `cmux/src/remote/rpc.rs` | 330 |
| `proxy_write` | Function | `cmux/src/remote/rpc.rs` | 342 |
| `proxy_close` | Function | `cmux/src/remote/rpc.rs` | 352 |
| `proxy_subscribe` | Function | `cmux/src/remote/rpc.rs` | 363 |
| `hex_decode` | Function | `cmux/src/socket/auth.rs` | 107 |
| `start` | Function | `cmux/src/remote/relay.rs` | 32 |
| `start` | Function | `cmux/src/remote/proxy.rs` | 24 |
| `port` | Function | `cmux/src/remote/proxy.rs` | 101 |
| `probe_platform` | Function | `cmux/src/remote/bootstrap.rs` | 23 |
| `remote_daemon_path` | Function | `cmux/src/remote/bootstrap.rs` | 63 |
| `check_remote_binary` | Function | `cmux/src/remote/bootstrap.rs` | 71 |
| `upload_daemon` | Function | `cmux/src/remote/bootstrap.rs` | 127 |
| `bootstrap_daemon` | Function | `cmux/src/remote/bootstrap.rs` | 205 |
| `socket_path` | Function | `cmux/src/socket/server.rs` | 29 |
| `cleanup` | Function | `cmux/src/socket/server.rs` | 268 |
| `daemon_path` | Function | `cmux/src/remote/session.rs` | 71 |
| `new` | Function | `cmux/src/remote/session.rs` | 107 |
| `start` | Function | `cmux/src/remote/session.rs` | 121 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `ApplicationDidFinishLaunching → RemotePlatform` | cross_community | 6 |
| `ApplicationDidFinishLaunching → Daemon_version` | cross_community | 5 |
| `ApplicationDidFinishLaunching → Remote_daemon_path` | cross_community | 5 |
| `ApplicationDidFinishLaunching → Check_remote_binary` | cross_community | 5 |
| `ApplicationDidFinishLaunching → Ssh_args` | cross_community | 4 |
| `ApplicationDidFinishLaunching → Daemon_path` | cross_community | 4 |
| `ApplicationDidFinishLaunching → Error` | cross_community | 4 |
| `Main → Socket_path` | cross_community | 4 |
| `Start → Compute_hmac_sha256` | cross_community | 4 |
| `Start → Hex_encode` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Socket | 2 calls |
| Session | 1 calls |

## How to Explore

1. `gitnexus_context({name: "is_alive"})` — see callers and callees
2. `gitnexus_query({query: "remote"})` — find related execution flows
3. Read key files listed above for implementation details
