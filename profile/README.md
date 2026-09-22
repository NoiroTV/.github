# NOIRO

**Open-source media software built around Noiro Core and Noiro TV Engine.**

NoiroTV is building a cross-platform media experience for the television, desktop, and mobile devices. The project combines a portable product core, a remote-first TV interaction layer, and native platform shells.

## Architecture

```text
Noiro Core
  ├─ media domain and library model
  ├─ provider and service contracts
  ├─ metadata, search, settings and sync
  └─ shared diagnostics and test fixtures
        ↓
Noiro TV Engine
  ├─ playback integration
  ├─ remote input and focus restoration
  ├─ Home, Details, Library and Search behavior
  └─ subtitles, overlays and transport controls
        ↓
Platform shells
  ├─ Android / Android TV
  ├─ Linux and Windows
  └─ macOS, iOS and tvOS
```

## Repositories

| Repository | Role | Status |
| --- | --- | --- |
| [`Noiro`](https://github.com/NoiroTV/Noiro) | Public monorepo for Noiro Core, clients, and integrations | Open development |
| [`noiro-kodi-engine`](https://github.com/NoiroTV/noiro-kodi-engine) | Kodi upstream fork pinned by the Noiro monorepo | Upstream integration |
| `noiro-core` | Reserved scaffold for a future independently versioned core | Private scaffold |
| `noiro-tv-engine` | Reserved scaffold for a future independently versioned TV engine | Private scaffold |
| `noiro-skins` | Reserved scaffold for skins and interface specifications | Private scaffold |

## Principles

- **Open source by design.** Distributed Noiro builds and their corresponding source stay traceable.
- **TV is a first-class surface.** Remote navigation, focus restoration and readable distance are product requirements.
- **One domain, native delivery.** Shared behavior does not require identical UI code on every platform.
- **Evidence before claims.** Source, builds, signed packages, store releases and physical-device acceptance are separate milestones.
- **Local-first where it matters.** A user's library, settings and playback state should remain understandable and portable.

## Current stage

Noiro is in foundation development. The source monorepo and Kodi fork are now
public; production binaries, store releases, and full platform support are not
yet claimed.

## Licensing and upstreams

Noiro is being developed as GPL-compatible open-source software. Kodi-derived work remains clearly attributed to its upstream project and retains all applicable licenses and notices.

NoiroTV is an independent project and is not affiliated with or endorsed by the Kodi Foundation or XBMC Foundation. Kodi and related marks belong to their respective owners.
