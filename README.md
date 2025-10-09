# TailBlazor.Modal
Basic Blazor Modal which can have a customizable header, body, and footer for Tailwindcss

Without passing it anything you'll get very basic styles, however giving it it's base classes and you can really make a customizable list component that Tailwind is capable of.

![Nuget](https://img.shields.io/nuget/v/TailBlazor.Modal.svg)

![Demo](screenshot.png)

## Getting Setup

You can install the package via the NuGet package manager just search for TailBlazor.Modal. You can also install via powershell using the following command.

`Install-Package TailBlazor.Modal`

Or via the dotnet CLI.

`dotnet add package TailBlazor.Modal`

### 1. Add Imports

Add line to your \_Imports.razor if you're not already using implicit global usings.

```
@using TailBlazor.Modal
```

### 2. Create Modal Component

Simply open up a component and add your content. Sizes include Small, Medium, Large, Larger, Largest

```
<TailBlazorModals IsOpen="@IsModalOpenXl" ModelWidth="TailBlazorModals.Size.Largest">
    <Header>
        ...
    </Header>
    <Body>
        ...
    </Body>
    <Footer>
        ...
    </Footer>
</TailBlazorModals>

```

The component targets .NET 9 and is compatible with Blazor's new Auto render mode, so it can light up interactivity whether your app prerenders on the server or runs entirely on WebAssembly.
