<p align="center"><img src="https://raw.githubusercontent.com/go-net-health/brand/main/social/go-net-health.png" alt="go-net-health" width="720"></p>

# go-net-health.github.io

The [go-net-health](https://github.com/go-net-health) organization landing page,
built with [Hugo](https://gohugo.io) and served at <https://go-net-health.github.io>.
It links to the [documentation](https://go-net-health.github.io/docs/) and the
[health](https://github.com/go-net-health/health) library.

## Local preview

```bash
hugo server
```

The page ships a light / dark / system theme toggle (default = system).

## The design is not here

It comes from the shared Hugo module
[`go-fleettools/landingkit`](https://github.com/go-fleettools/landingkit),
pinned in `go.mod` (Renovate bumps it); `kit.go` keeps `go mod tidy` from
deleting that requirement. `[params.brand]` in `hugo.toml` is read from the logo by
`landingkit brand`. A file under `layouts/partials/` with the name of one of the
kit's would silently override it.
