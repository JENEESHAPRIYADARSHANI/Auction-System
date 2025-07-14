# SA Auction System

A web-based Auction System built with ASP.NET Core and Entity Framework Core, targeting .NET 8.0.

## Overview

This project provides an online platform for listing and bidding on auction items. The system is designed with modern ASP.NET technologies and integrates with authentication providers and payment services.

## Features

- User authentication and management (ASP.NET Identity)
- Entity Framework Core with SQL Server for data storage
- Google authentication support
- PayPal integration for payment processing
- MVC architecture with Razor views
- Modern UI with CSS bundling and minification
- Cart and checkout functionality
- Listings management (create, edit, delete, view details, my bids)
- Secure user secrets management for local development

## Getting Started

### Prerequisites

- [.NET 8.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- SQL Server (local or cloud instance)
- Visual Studio 2022 or newer (recommended)

### Setup

1. **Clone the Repository**
    ```bash
    git clone https://github.com/JENEESHAPRIYADARSHANI/Auction-System.git
    cd Auction-System
    ```

2. **Restore Packages**
    ```bash
    dotnet restore
    ```

3. **Configure User Secrets**  
    Set up your local secrets for sensitive configuration (e.g., connection strings, API keys):
    ```bash
    dotnet user-secrets init
    dotnet user-secrets set "ConnectionStrings:DefaultConnection" "<your-connection-string>"
    ```

4. **Update Database**
    ```bash
    dotnet ef database update
    ```

5. **Run the Application**
    ```bash
    dotnet run
    ```

6. **Access the App**  
    Visit `https://localhost:5001` in your browser.

## Project Structure

- `Areas/Identity` - Identity and authentication logic
- `Views` - Razor views (UI)
- `wwwroot` - Static files (CSS, JS, images)
- `SA Auction.csproj` - Project configuration and dependencies

## Dependencies

- Microsoft.AspNetCore.Authentication.Google
- Microsoft.AspNetCore.Identity.EntityFrameworkCore
- Microsoft.EntityFrameworkCore.SqlServer
- PayPalButtonManagerSDK

## Customization

- Update CSS in `wwwroot` or use the bundled/scoped CSS files for layout and theming.
- Extend listings, bids, or checkout logic in the corresponding controllers and views.

## License

This project currently does not specify a license.

---

> **Note:** Some project details may be incomplete due to limited code search results. For a full overview, explore the [GitHub repository](https://github.com/JENEESHAPRIYADARSHANI/Auction-System).
