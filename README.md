# Gotify for LazyCat

Gotify is a simple server for sending and receiving messages. This repository packages `gotify/server` as a LazyCat LPK v2 application.

## Configuration

The installation wizard configures the local administrator password, time zone, and optional OpenID Connect login. The OIDC redirect URL is generated automatically as:

```text
https://<application-domain>/auth/oidc/callback
```

Application data is stored persistently under `/lzcapp/var/data`.

## Publishing

GitHub Actions checks stable `gotify/server` releases, verifies the configured mirror digest, creates versioned GitHub Release assets, and publishes only to the MiaoMiao private store.

Upstream: <https://gotify.net>
