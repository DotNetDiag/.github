# DotNetDiag

**DotNetDiag** is the home of the actively maintained fork of [AspNetCore.Diagnostics.HealthChecks](https://github.com/Xabaril/AspNetCore.Diagnostics.HealthChecks), providing production-ready health check packages, a rich UI dashboard, and Kubernetes integration for ASP.NET Core applications.

## What We Build

- **50+ Health Check Packages** — Ready-to-use checks for databases, message brokers, cloud services, and infrastructure dependencies. Install any package from NuGet and register it in minutes.
- **HealthChecks UI** — A real-time dashboard for visualizing liveness and readiness endpoints across multiple services, with configurable storage providers, polling, and failure notifications.
- **Kubernetes Integration** — Operator workflows, in-cluster service discovery, and liveness/readiness probe support to keep your workloads healthy at scale.

## Quick Start

```bash
dotnet add package DotNetDiag.HealthChecks.SqlServer
```

Register your checks and expose the endpoints:

```csharp
builder.Services.AddHealthChecks()
    .AddSqlServer(connectionString);

app.MapHealthChecks("/health");
```

## Resources

| Resource | Link |
|----------|------|
| 📦 NuGet Packages | [nuget.org/packages?q=DotNetDiag.HealthChecks](https://www.nuget.org/packages?q=DotNetDiag.HealthChecks) |
| 📖 Reference Manual | [dotnetdiag.github.io](https://dotnetdiag.github.io/) |
| 💻 Source Code | [github.com/DotNetDiag/HealthChecks](https://github.com/DotNetDiag/HealthChecks) |

## Contributing

We welcome issues, pull requests, and documentation improvements. See the [contributing guide](https://github.com/DotNetDiag/HealthChecks/blob/master/README.md) for details.
