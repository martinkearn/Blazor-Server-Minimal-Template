# Blazor Server Minimal Template
A Visual Studio 2019 template that creates a minimal Blazor Server project with a lot of the example code removed. This includes, but is not limited to removal of the following default artifacts:
- Counter page
- Weather forecast service and page
- Bootstrap
- Ionic
- Most of the markup in `MainLayout.razor` and `Index.razor` 
- Navigation
- Most of the default `site.css`

Some fundamental features are left intact such as the default error pages, a basic layout and a minimal `site.css` as well as the typical `startup.cs` functionality. What you are left with is a clean, minimal Blazor server project which you can use as a starting point to build your preferred functionality.

## Use the template
1. Install the [BlazorServerMinimal.vsix](BlazorServerMinimal.vsix) file.
2. Open Visual Studio 2019
3. Create a new project
4. Search for "Blazor"
5. Choose "Blazor Server Minimal"
6. Set the project name, location etc and create the project as usual
7. Sometimes Visual Studio does not replace the namespace correctly which is `BlazorServerMinimalTemplate` by default. If this happens, just replace it with your own namespace manually. This usually occrs in `_Imports.razor`
