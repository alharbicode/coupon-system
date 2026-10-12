# Coupon System API

A REST API for managing coupons and recording coupon usage. The repository contains an ASP.NET Core Web API project with Entity Framework Core and SQL Server.

## Features

- Create, list, update, and delete coupons.
- Record and review coupon usage.
- Use Entity Framework Core migrations.
- Explore the API with Swagger in the Development environment.

## Tech stack

- .NET 8
- ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- Swagger / OpenAPI

## Project layout

```text
coupon-system/
├── Controllers/
│   ├── CouponsController.cs
│   └── CouponUsagesController.cs
├── Migrations/
├── data/
├── models/
├── Program.cs
└── appsettings.json
```

## Run locally

1. Install the .NET 8 SDK and SQL Server.
2. Update `ConnectionStrings:DefaultConnection` in `coupon-system/appsettings.json` to point to your SQL Server instance.
3. From the repository root, run:

```bash
dotnet restore coupon-system/coupon-system.csproj
dotnet run --project coupon-system/coupon-system.csproj
```

When running in Development, open the Swagger URL printed by the application to inspect and try the API endpoints. Apply database migrations before using the API if the database has not been initialized.

## Notes

The project currently targets .NET 8. Configure a database connection appropriate for your local environment before running it.
