# Scoop Bucket — Dever Labs

This is the official [Scoop](https://scoop.sh) bucket for [Dever Labs](https://github.com/dever-labs) apps.

## Usage

Add the bucket, then install:

```powershell
scoop bucket add dever-labs https://github.com/dever-labs/scoop-bucket
scoop install dever-labs/devx
scoop install dever-labs/resctl
scoop install dever-labs/mockly
scoop install dever-labs/postly
```

## Available Apps

| App | Description | Architectures |
|---|---|---|
| [`devx`](bucket/devx.json) | Tool to help speed up local development and keep it consistent across a team | 64bit, arm64 |
| [`resctl`](bucket/resctl.json) | Minimal CLI to get, set and toggle display resolution | 64bit |
| [`mockly`](bucket/mockly.json) | Mock server for HTTP, gRPC, Redis, Kafka, and 17 other protocols | 64bit |
| [`postly`](bucket/postly.json) | Desktop API client for teams — REST, GraphQL, gRPC, WebSocket & MQTT (portable build) | 64bit |

## About

Each manifest pins the Windows asset of the app's latest GitHub release, with
`checkver: github` and an `autoupdate` block (hashes come from the release's
`checksums.txt` where one is published).

- [`mockly`](bucket/mockly.json) is also updated automatically by [goreleaser's `scoops`](https://github.com/dever-labs/mockly/blob/main/.goreleaser.yaml) as part of the [mockly release workflow](https://github.com/dever-labs/mockly/blob/main/.github/workflows/ci.yml); its next release overwrites this manifest.
- The others are updated by running Scoop's `checkver.ps1 -Update` against `bucket/` (an excavator workflow is not set up yet).
