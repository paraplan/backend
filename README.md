<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/brand/logo-dark.svg">
    <img alt="Paraplan" src="docs/brand/logo-light.svg" width="320">
  </picture>
</p>

# Paraplan Backend

ASP.NET Core Web API on .NET 10.

## Layout

```
Paraplan.slnx                 solution
src/Paraplan.Api/             web API host
tests/Paraplan.Api.Tests/     xUnit integration tests (WebApplicationFactory)
Directory.Build.props         shared build settings (net10.0, nullable, analyzers, warnings as errors)
global.json                   pinned .NET SDK
```

## Getting started

```bash
dotnet build
dotnet test
dotnet run --project src/Paraplan.Api
```

The API listens on `http://localhost:5297` (`https://localhost:7246` with the `https` profile).

- `GET /health` – health check
- `GET /openapi/v1.json` – OpenAPI document (Development only)

## Docs

- [Database ER diagram](docs/database/er-diagram.md)
