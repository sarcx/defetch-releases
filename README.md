# defetch

Serverless peer-to-peer file sharing for the terminal. No tracker, no central
server — peers gossip to discover each other and move files directly in 1 MiB,
SHA-256-verified chunks. Peers behind NAT tunnel through a public-IP peer.

Runs on macOS, Linux, Windows, and Android TV. This repository hosts the release binaries;
grab the asset for your platform from the
[latest release](https://github.com/sarcx/defetch-releases/releases/latest).

**Latest release: v0.20.0**

## Download

| Asset | Platform |
| --- | --- |
| `defetch-win32-x64.exe` | Windows x86_64 |
| `defetch-darwin-arm64` | Apple Silicon macOS |
| `defetch-linux-x64` | Linux x86_64 |
| `defetch.mjs` | single-file bundle (any OS with Node ≥ 18) |
| `defetch-tv.apk` | Android TV app, a Stremio add-on for the swarm's films |

The standalone binaries bundle their own runtime — no Node install needed.

## Run

```sh
defetch --dir ./downloads --port 4040 --relay <public-host>:4040
```

- `--dir` — folder shared with and downloaded from the swarm.
- `--port` — TCP listen port (default 4040).
- `--relay host:port` — tunnel through a publicly reachable peer when behind NAT.
- `--slug <label>` — human-readable name shown in other peers' lists (default: hostname).
- `--ephemeral-id` — use a throwaway peer id for this session.

In the REPL: `peers`, `files` (interactive picker), `get <name>`, `share`,
`version`, `upgrade`, `quit`.

## Upgrade

Type `upgrade` in the REPL to fetch and install the latest release for your
platform, then restart to apply.

## Android TV

`defetch-tv.apk` runs defetch on the TV so Stremio there can play the swarm's
films. Install it once with `adb install defetch-tv.apk`. Then open defetch, enter
your relay, and in Stremio add `http://127.0.0.1:7650/manifest.json`. After that
it starts with the TV and keeps defetch itself up to date. A new APK is only
needed when the app around it changes.

## Changelog

See [CHANGELOG.md](CHANGELOG.md).
