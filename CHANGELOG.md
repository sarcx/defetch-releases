# Changelog

## v0.10.1 — 2026-08-19

- Show torrent contents that no peer holds yet

## v0.10.0 — 2026-08-19

- Read .torrent files beside the shared data
- Bump checkout and setup-node from v5 to v7
- Bump checkout and setup-node to v5
- Strip whitespace from the release token everywhere
- Publish release assets without Actions storage

## v0.9.0 — 2026-08-18

- Add NAT traversal so peers can leave the relay
- Make every shared directory removable
- Add multiple shared directories to shared command
- Show shared folder path in shared command
- Rename share command to shared
- Remove get command in favor of files picker
- Add background downloads with live status view
- Retain CI build artifacts for one day

## v0.8.5 — 2026-07-23

- Extract commit-message cleanup into cleanMessage helper

## v0.8.4 — 2026-07-22

- Fix interactive file picker by resuming stdin

## v0.8.3 — 2026-07-22

- Add fallback when commit generator returns a bump line

## v0.8.2 — 2026-07-22

- Trim whitespace from the releases token so CI can push docs

## v0.8.1 — 2026-07-22

- Publish release docs to the public releases repo

## v0.8.0 — 2026-07-22

- Add interactive file picker for the files command

## v0.7.0 — 2026-07-22

- Remove announce command and require peer slug

## v0.6.0 — 2026-07-22

- Add human-readable slug label for peers

## v0.5.9 — 2026-07-22

- Show a progress bar while upgrading

## v0.5.8 — 2026-07-22

- Poll for updates every minute using conditional GET

## v0.5.7 — 2026-07-22

- Add CLAUDE.md and note auto-generated commit msgs

## v0.5.6 — 2026-07-22

- Add one-command release script

## v0.5.5 — 2026-07-22

- Show peer count instead of chunks in progress bar

## v0.5.4 — 2026-07-22

- Show a download progress bar with speed

## v0.5.3 — 2026-07-22

- Show an update notice in the status line

## v0.5.2 — 2026-07-22

- Show human-readable file sizes in the files list

## v0.5.1 — 2026-07-19

- Evict relay peers on tunnel close and stop re-gossip
- Drop Intel Mac build from the release workflow

## v0.5.0 — 2026-07-19

- Add upgrade command pulling from public releases repo

## v0.4.0 — 2026-07-19

- Reject peerId collisions and add ephemeral ids

## v0.3.0 — 2026-07-19

- Add relay tunneling for peers behind NAT
- Add tests for config, handlers, and end-to-end transfer

## v0.2.0 — 2026-06-10

- Add updated-dev command
- Add status line
- Add command version
- Make test command Windows-friendly

## v0.1.0 — 2026-05-25

- Add release workflow building binaries on tag push
- Initial defetch: serverless P2P file-sharing CLI

