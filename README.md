# Scoop Bucket — Dever Labs

This is the official [Scoop](https://scoop.sh) bucket for [Dever Labs](https://github.com/dever-labs) apps.

## Usage

Add the bucket, then install:

```powershell
scoop bucket add dever-labs https://github.com/dever-labs/scoop-bucket
scoop install mockly
```

## Available Apps

| App | Description |
|---|---|
| [`mockly`](bucket/mockly.json) | Mock server for HTTP, gRPC, Redis, Kafka, and 17 other protocols |

## About

Manifests in this bucket are updated automatically whenever a new version is published:

- [`mockly`](bucket/mockly.json) — by [goreleaser's `scoops`](https://github.com/dever-labs/mockly/blob/main/.goreleaser.yaml) as part of the [mockly release workflow](https://github.com/dever-labs/mockly/blob/main/.github/workflows/ci.yml)
