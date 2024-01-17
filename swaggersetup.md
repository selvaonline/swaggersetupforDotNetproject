# Implementing Swagger in ASP.NET Core Web API

This guide provides steps to integrate Swagger into an ASP.NET Core Web API project for API documentation and testing.

## Steps

### 1. Install NuGet Packages

First, add the necessary NuGet package to your project:

- `Swashbuckle.AspNetCore`: This package integrates Swagger with ASP.NET Core Web API.

You can install it using the NuGet Package Manager or the Package Manager Console:

```shell
Install-Package Swashbuckle.AspNetCore

2. Configure Swagger in Startup.cs
Next, configure Swagger in the Startup.cs file of your project.

In the ConfigureServices method:
Add the following code to enable and configure Swagger:

services.AddSwaggerGen(c =>
{
    c.SwaggerDoc("v1", new OpenApiInfo { Title = "Your API Name", Version = "v1" });
});

In the Configure method:
Enable the Swagger UI endpoint with the following code:
