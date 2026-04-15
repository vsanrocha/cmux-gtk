---
name: cmuxd-remote
description: "Skill for the Cmuxd-remote area of cmux-gtk. 126 symbols across 5 files."
---

# Cmuxd-remote

126 symbols | 5 files | Cohesion: 64%

## When to Use

- Working with code in `daemon/`
- Understanding how TestCLIPingV1OverAuthenticatedTCPWithEnv, TestCLIPingV1OverAuthenticatedTCPWithRelayFile, TestCLIUnknownCommand work
- Modifying cmuxd-remote-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `daemon/remote/cmd/cmuxd-remote/cli_test.go` | TestCLIPingV1OverAuthenticatedTCPWithEnv, TestCLIPingV1OverAuthenticatedTCPWithRelayFile, TestCLIUnknownCommand, TestCLINoSocket, TestCLINoArgs (+36) |
| `daemon/remote/cmd/cmuxd-remote/main.go` | main, shouldRunCLIForInvocation, isDaemonEntryCommand, run, usage (+28) |
| `daemon/remote/cmd/cmuxd-remote/main_test.go` | TestProxyStreamRoundTrip, TestProxyOpenInvalidParams, TestSessionResizeCoordinator, TestSessionInvalidParamsAndNotFound, assertAttachmentCount (+24) |
| `daemon/remote/cmd/cmuxd-remote/cli.go` | runCLI, runRPC, readSocketAddrFile, cliUsage, readRelayAuthFile (+17) |
| `ghostty/macos/Sources/Helpers/Extensions/Duration+Extension.swift` | Duration |

## Entry Points

Start here when exploring this area:

- **`TestCLIPingV1OverAuthenticatedTCPWithEnv`** (Function) — `daemon/remote/cmd/cmuxd-remote/cli_test.go:395`
- **`TestCLIPingV1OverAuthenticatedTCPWithRelayFile`** (Function) — `daemon/remote/cmd/cmuxd-remote/cli_test.go:408`
- **`TestCLIUnknownCommand`** (Function) — `daemon/remote/cmd/cmuxd-remote/cli_test.go:578`
- **`TestCLINoSocket`** (Function) — `daemon/remote/cmd/cmuxd-remote/cli_test.go:585`
- **`TestCLINoArgs`** (Function) — `daemon/remote/cmd/cmuxd-remote/cli_test.go:803`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `Duration` | Class | `ghostty/macos/Sources/Helpers/Extensions/Duration+Extension.swift` | 2 |
| `TestCLIPingV1OverAuthenticatedTCPWithEnv` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 395 |
| `TestCLIPingV1OverAuthenticatedTCPWithRelayFile` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 408 |
| `TestCLIUnknownCommand` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 578 |
| `TestCLINoSocket` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 585 |
| `TestCLINoArgs` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 803 |
| `TestCLIHelpFlag` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 810 |
| `TestCLIHelpCommand` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 817 |
| `TestProxyStreamRoundTrip` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 257 |
| `TestProxyOpenInvalidParams` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 530 |
| `TestSessionResizeCoordinator` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 556 |
| `TestSessionInvalidParamsAndNotFound` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 646 |
| `TestProxyOpenBlockedLoopback` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 810 |
| `TestProxyOpenBlockedMetadata` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 829 |
| `TestProxyOpenAllowPrivateEnvOverride` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 849 |
| `TestDialSocketRefreshesToUpdatedTCPAddressWithoutPolling` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 309 |
| `TestDialSocketFailsFastWhenTCPAddressStaysStale` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 353 |
| `TestDialSocketDetection` | Function | `daemon/remote/cmd/cmuxd-remote/cli_test.go` | 436 |
| `TestRunVersion` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 78 |
| `TestRunStdioHelloAndPing` | Function | `daemon/remote/cmd/cmuxd-remote/main_test.go` | 129 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Run → ParsedFlags` | cross_community | 5 |
| `Main → ParsedFlags` | cross_community | 5 |
| `Run → Close` | cross_community | 4 |
| `Run → DiscardUntilNewline` | cross_community | 4 |
| `Run → FlagToParamKey` | cross_community | 4 |
| `Run → ApplyWorkspaceEnvFallback` | cross_community | 4 |
| `Run → ApplySurfaceEnvFallback` | cross_community | 4 |
| `Main → FlagToParamKey` | cross_community | 4 |
| `Main → ApplyWorkspaceEnvFallback` | cross_community | 4 |
| `Main → ApplySurfaceEnvFallback` | cross_community | 4 |

## How to Explore

1. `gitnexus_context({name: "TestCLIPingV1OverAuthenticatedTCPWithEnv"})` — see callers and callees
2. `gitnexus_query({query: "cmuxd-remote"})` — find related execution flows
3. Read key files listed above for implementation details
