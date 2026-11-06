<p align="center"><img src="branding/banner.svg" alt="Project banner" width="100%"/></p>

# FrankenSPO.WebApi

> **Status: skeleton — no runtime behavior yet.** Solution, CI and tests build against a pinned [FrankenSPO](https://github.com/skvorc-dev/FrankenSPO) pre-release. There is no public API until a feature works and is tested.

ASP.NET Core model-driven API generation for registered FrankenSPO business objects.

The planned WebAPI automatically exposes configured registered entity endpoints using standard HTTP and OpenAPI, with optional OData functionality. Clients use ordinary HTTP libraries; no special FrankenSPO runtime is needed. Automatic endpoint generation does not imply unauthenticated access.

## Development readiness

The skeleton started on 2026-11-06. The first release of this repository still waits for the [M0 gate](https://github.com/skvorc-dev/FrankenSPO.WebApi/issues/1); nothing here is usable before it.

## Build

```bash
scripts/fetch-frankenspo.sh   # downloads and checksum-verifies the FrankenSPO packages named in Directory.Build.props
dotnet build FrankenSPO.WebApi.slnx -c Release
dotnet test FrankenSPO.WebApi.slnx -c Release --no-build
```

## Contributions

Generic, application-neutral code only, under MIT (see [CONTRIBUTING.md](CONTRIBUTING.md)). Agree the shape in an issue before a large change.

## Examples and documentation

Working shared-domain samples, provider tests, getting-started instructions, language/platform demonstrations and machine-readable supported-feature documentation will be maintained as implementation progresses.

See [planned readiness requirements](docs/READINESS.md), [contributor guidance](CONTRIBUTING.md) and [security policy](SECURITY.md).

Licensed under [MIT](LICENSE).
