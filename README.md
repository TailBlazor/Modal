# TailBlazor.Model
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

Add line to your \_Imports.razor

```
@using TailBlazor.Modal
```

### 2. Create Modal Component

Simply open up a component and add your content. Sizes include Small, Medium, Large, ExtraLarge

```
<TailBlazorModals IsOpen="[OPEN_FLAG]" ModelWidth="TailBlazorModals.Size.Large">
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