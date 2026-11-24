# scoop-bucket

Personal [Scoop](https://scoop.sh) bucket maintained by [@doubyoungle](https://github.com/doubyoungle).

[![Tests](https://github.com/doubyoungle/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/doubyoungle/scoop-bucket/actions/workflows/ci.yml)
[![Excavator](https://github.com/doubyoungle/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/doubyoungle/scoop-bucket/actions/workflows/excavator.yml)

## Install this bucket

```pwsh
scoop bucket add doubyoungle https://github.com/doubyoungle/scoop-bucket
```

## Available manifests

| Manifest | Description |
| --- | --- |
| [misterdownloadmanager](bucket/misterdownloadmanager.json) | Fast, resumable download manager with browser integration, video/torrent support, and an MCP server |

```pwsh
scoop install doubyoungle/misterdownloadmanager
```

## Automation

- The **Excavator** workflow runs every 4 hours and automatically updates manifests to the latest upstream versions (`checkver` + `autoupdate`).
- The **CI** workflow runs Scoop's manifest tests on every push and pull request.

To make new manifests, copy `bucket/app-name.json.template` to `bucket/<app-name>.json` and follow the [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md) and the [App Manifests wiki](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests).
