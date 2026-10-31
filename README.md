# AxonHub Infrlo Launcher

Runs the pinned AxonHub `v1.0.0-beta11` release on Infrlo using an external
PostgreSQL database.

The launcher downloads the official Linux release archive, verifies both the
archive and extracted binary SHA-256 hashes, and starts AxonHub on Infrlo's
assigned `PORT`.

Required environment variables:

- `AXONHUB_DB_DSN`: PostgreSQL connection string.

Optional environment variables:

- `AXONHUB_DB_DIALECT`: defaults to `postgres`.
- `AXONHUB_LOG_OUTPUT`: defaults to `stdio`.
- `SSL_CERT_FILE`: defaults to the bundled Mozilla CA bundle.

Infrlo build command:

```sh
bash ./prepare.sh
```

Infrlo run command:

```sh
bash ./start.sh
```

AxonHub is Apache-2.0 licensed. Its license is included in `LICENSE`.
