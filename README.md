# Blazor Server Minimal Template
A Visual Studio 2019 template that creates a minimal Blazor Server project with a lot of the example code removed. This includes, but is not limited to removal of the following default artefacts:
- Counter page
- Weather forecast service and page
- Bootstrap
- Ionic
- Most of the mark-up in `MainLayout.razor` and `Index.razor` 
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
7. Visual Studio does not replace the namespace correctly in `_Imports.razor` which prevents the application from building, presumably because this is a mark-up file rather than compiled code. To correct this, just replace `BlazorServerMinimalTemplate` with your own namespace manually in `_Imports.razor`.

## Projects

This repository has three projects:

- **BlazorServerMinimalTemplate**: This is the template that the VSIX is created from; a minimal Blazor Server project template.
- **BlazorServerDefaultTemplate_v3-1-6**: This is the default Blazor Server template with the counter, weather forecast, style and other items. This s based on v3.1.6 of the official default template.
- **BlazorServerMinimal**: This is the Visual Studio project template that is used to create the VSIX.

## Updating the VSIX

If you wish to create your own variation of this template and update the VSIX file, you can follow these steps

1. Create your template project and export it: https://docs.microsoft.com/en-us/visualstudio/ide/how-to-create-project-templates?view=vs-2019
2. Create a VSIX project which uses the ZIP created in step 1: https://docs.microsoft.com/en-us/visualstudio/extensibility/getting-started-with-the-vsix-project-template?view=vs-2019