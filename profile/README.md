## Ophymx

Small, focused libraries and tools in Rust and Go. Most of these exist because
the thing they replace was a shell script, a shim, or a dependency that did
too much.

Everything here is MIT or Apache-2.0. Go libraries are on
[pkg.go.dev](https://pkg.go.dev/github.com/ophymx); Rust crates build from
source for now.

### Reading & e-ink

| | |
| --- | --- |
| [chapbook](https://github.com/ophymx/chapbook) | Lightweight ereader core in Rust — EPUB 3, CBZ and PDF on stylo + cosmic-text + tiny-skia, no webview |
| [opds](https://github.com/ophymx/opds) | OPDS 1.2 + 2.0 catalog services from a single model |
| [mezzotint](https://github.com/ophymx/mezzotint) | E-ink and framebuffer output: waveform-aware refresh over a vendor-neutral panel contract |
| [formulary](https://github.com/ophymx/formulary) | Native MathML Core layout — OpenType MATH metrics in, resolution-independent display list out |
| [longbox](https://github.com/ophymx/longbox) | CBZ comic archives with ComicInfo.xml metadata |
| [screentone](https://github.com/ophymx/screentone) | Prepare manga and comic pages for e-ink readers |
| [splash](https://github.com/ophymx/splash) | Fixed-layout EPUB3 from full-page images — deterministic, RTL-aware, stdlib only |
| [webanno](https://github.com/ophymx/webanno) | W3C Web Annotation Data Model and Protocol, zero dependencies |

### Media & playback

| | |
| --- | --- |
| [rsmpv](https://github.com/ophymx/rsmpv) | Clean-room Rust bindings for libmpv, built from mpv's ISC client headers |
| [mpv-engine](https://github.com/ophymx/mpv-engine) | Toolkit-agnostic libmpv embedding core: lifecycle, commands, typed events, render seams |
| [iced_mpv](https://github.com/ophymx/iced_mpv) | Hardware-accelerated video widget for iced |
| [muxmix](https://github.com/ophymx/muxmix) | Composable FFmpeg pipelines in Go |
| [fillscreen](https://github.com/ophymx/fillscreen) | Fill any monitor with a solid color — blank a spare screen, or make a soft key light |

### Text processing

| | |
| --- | --- |
| [quarry](https://github.com/ophymx/quarry) | Declarative HTML extraction — selectors that fail loud when the page changes |
| [semblance](https://github.com/ophymx/semblance) | Text-similarity sketching: shingling, MinHash, SimHash, LSH indexing |
| [normtext](https://github.com/ophymx/normtext) | Deterministic, composable text normalization — the preprocessing companion to semblance |

### Infrastructure & packaging

| | |
| --- | --- |
| [apt-wharf](https://github.com/ophymx/apt-wharf) | Build, sign and serve Debian apt repositories without re-hosting vendor binaries |
| [wharf-action](https://github.com/ophymx/wharf-action) | GitHub/Gitea actions to package apt-wharf configured releases |
| [aptly-webui](https://github.com/ophymx/aptly-webui) | Web UI for an [aptly](https://www.aptly.info/) instance |
| [vault-cert-agent](https://github.com/ophymx/vault-cert-agent) | Keeps Vault-issued TLS material refreshed on disk for local consumers |
| [vault-pgp-sign](https://github.com/ophymx/vault-pgp-sign) | OpenPGP signing CLI backed by Vault transit, with key rotation, expiration and revocation |
| [incus-wifi](https://github.com/ophymx/incus-wifi) | Attach wifi devices to Incus containers |

### Distributed systems

| | |
| --- | --- |
| [odradek](https://github.com/ophymx/odradek) | Kafka-protocol Rust crates: sans-I/O protocol, client, conformance suite, web bridges |
| [saltator](https://github.com/ophymx/saltator) | Self-clustering Matrix homeserver in Rust — native HA, no external database |
| [pg-agent-rs](https://github.com/ophymx/pg-agent-rs) | High-availability agent for PostgreSQL behind pgpool-II — promotion is a compare-and-swap on a Raft lease, no external DCS |

### Hardware

| | |
| --- | --- |
| [powermate-rs](https://github.com/ophymx/powermate-rs) | Clean-room userspace Linux driver, tray daemon and config GUI for the Griffin PowerMate USB knob |
