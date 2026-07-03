# javinizer scoop bucket

Scoop bucket for [javinizer](https://github.com/javinizer/javinizer-go) — a JAV metadata scraper and organizer (CLI, TUI, REST API, and web UI).

## Install (Windows)

```powershell
scoop bucket add javinizer https://github.com/javinizer/scoop-javinizer
scoop install javinizer
```

Update to the latest stable release later:

```powershell
scoop update javinizer
```

## How it works

The manifest installs the prebuilt `javinizer-windows-amd64.exe` binary. This bucket is updated **automatically** on every stable release by the [`cli-release`](https://github.com/javinizer/javinizer-go/blob/main/.github/workflows/cli-release.yml) workflow in the main repo. Prereleases (`v1.0.0-rc.*`) never reach the bucket, so `scoop update` never hands you a release candidate.

The manifest includes `autoupdate` configuration, so Scoop can fetch new versions and their checksums from `checksums.txt` without a manual bucket update.

## Files

- `bucket/javinizer.json` — the manifest (auto-generated from `checksums.txt` on each stable release)

## Links

- Main repo: [javinizer/javinizer-go](https://github.com/javinizer/javinizer-go)
- Releases: [github.com/javinizer/javinizer-go/releases](https://github.com/javinizer/javinizer-go/releases)
- Issues: [github.com/javinizer/javinizer-go/issues](https://github.com/javinizer/javinizer-go/issues)
