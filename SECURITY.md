# Security Policy

This policy covers every repository in the [ophymx](https://github.com/ophymx)
organization unless a repository ships its own `SECURITY.md`.

## Reporting a vulnerability

Use GitHub's private vulnerability reporting: open the **Security** tab on the
affected repository and choose **Report a vulnerability**. That opens an
advisory visible only to the maintainer.

Please don't open a public issue for a security report. If private reporting
is unavailable to you, open an issue saying only that you have a security
report and how to reach you privately — no details.

## What to expect

This is a small organization maintained by one person. Expect an
acknowledgement within a week. Valid reports get a fix and a published
advisory crediting you unless you'd rather stay anonymous; invalid ones get an
explanation of why.

There is no bounty program.

## Where reports are most valuable

A few repositories handle material where a flaw has real consequences —
signing keys, TLS private keys, package integrity, and database failover:

- [vault-pgp-sign](https://github.com/ophymx/vault-pgp-sign) — OpenPGP signing via Vault transit
- [vault-cert-agent](https://github.com/ophymx/vault-cert-agent) — Vault-issued TLS material on disk
- [apt-wharf](https://github.com/ophymx/apt-wharf) — building, signing and serving apt repositories
- [rsmpv](https://github.com/ophymx/rsmpv) — FFI over a C library, so memory safety at the boundary matters

Issues in key handling, signature verification, package integrity, path
traversal during extraction, or privilege boundaries are the ones most worth
your time.

Most other repositories here are libraries with no network surface and no
privileged operation. A panic or crash on malformed input is a bug worth
filing publicly, not a vulnerability — though if it's reachable from untrusted
input in a way that isn't obvious, err toward reporting it privately and we'll
sort it out.

## Supported versions

Everything here is pre-1.0. Only the newest tagged version of a given
repository receives fixes, and there are no backports.
