Install the required NuGet packages:

Swashbuckle.AspNetCore: This package provides the necessary libraries for integrating Swagger into your ASP.NET Core Web API project.
Configure Swagger in the Startup.cs file:

In the ConfigureServices method, add the following code to enable Swagger and configure the Swagger UI:
In the Configure method, add the following code to enable the Swagger UI endpoint:
Add XML comments (optional):

If you want to include XML comments in the Swagger documentation, enable XML documentation generation in your project properties. Then, add the following code to the ConfigureServices method in Startup.cs:
;
Build and run the project:

Build the project to ensure there are no compilation errors.
Run the project by selecting "Debug" > "Start Debugging" or pressing F5.
Access the Swagger UI:

Open a web browser and navigate to the Swagger UI endpoint. By default, it is available at https://localhost:<port>/swagger.
You should now see the Swagger UI page, where you can explore and test your API endpoints. The Swagger UI provides a user-friendly interface to interact with your API and view the available endpoints, request/response models, and even allows you to test the API directly from the UI.
