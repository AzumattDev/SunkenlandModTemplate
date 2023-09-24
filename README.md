# Sunkenland Mod Template

Welcome to the Sunkenland Mod Template by Azumatt! This repository provides a .NET template for quickly scaffolding mods
for Sunkenland.

## Prerequisites

- .NET SDK (version you're targeting, e.g., .NET 5.0 or later)
- Git
- JetBrains Rider or Visual Studio (optional for GUI-based installation)

## Features

- This mod template automatically packages your mod into a .zip file when in Release mode for Thunderstore as well as
  Nexus.
- The contents of the zip file come from the Thunderstore folder. Make sure you're updating the `manifest.json` with
  your relevant information for Thunderstore.
- The README.md at the project root is auto copied to the Thunderstore folder, to keep both the same and auto-packaging
  a breeze.
- The zip files will auto append the version string when you change the version in the `Plugin.cs` file and places it
  inside of the project's Thunderstore/Nexus folders (respectively).
- A copy of the compiled mods will be placed in your specified output folders from the `environment.props` file.
- It also includes a .gitignore file for use with Git.

### New to cloning repositories?

If you're new to cloning repositories, you can follow this link to get more familiar with the process:
https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository

## Once you have the repository cloned, you may follow the installation methods below.

## Installation

### Using Command Line

1. Clone this repository:
   ```bash
   git clone https://github.com/AzumattDev/SunkenlandModTemplate.git
   ```

2. Navigate to the directory:
   ```bash
   cd SunkenlandModTemplate
   ```

3. Install the template:
   ```bash
   dotnet new install ./
   ```

This will install the Sunkenland Mod Template locally and make it available as a dotnet template.

### Installing Using JetBrains Rider

1. Open JetBrains Rider.
2. Go to `File` > `New Solution`.
3. On the left, click `More templates`.
4. Click on the button in the middle that says "Install Template".
   ![](https://i.imgur.com/pLzWEzl.png)
5. Navigate to the directory where you cloned the `SunkenlandModTemplate` repository and select the root folder. Usually
   in the path of `C:\Users\YourName\RiderProjects\SunkenlandModTemplate`
   folder.
6. The template should now be available in the list.
7. Now, when you create a new project, you can select the template from the list on the left after stating you want to
   create a new solution. Make sure that you select the checkbox for `Put solution and project in the same directory`
   for the template to work properly.
8. If everything is done correctly, you will follow the prompts and the template will create a new project for you full
   of predefined configurations and code.

![](https://i.imgur.com/yVcYC4K.png)

### Installing Using Visual Studio

1. Open the template's repo in Visual Studio.
2. Under `Tools` > `Command Line` > Choose `Developer Command Prompt`.
   ![https://i.imgur.com/P3qwJlF.png](https://i.imgur.com/P3qwJlF.png)
3. Run the command listed above in the command line installation `dotnet new install ./`, you should see that the template is now installed.
   ![https://i.imgur.com/rbxRUml.png](https://i.imgur.com/rbxRUml.png)
4. Now for any new project, you can search for the template (or optionally pin it to the left after you find it).
   ![https://i.imgur.com/y010m2O.png](https://i.imgur.com/y010m2O.png)
5. Now, when you create a new project, you can select the template from the list on the left after stating you want to
   create a new solution. Make sure that you select the checkbox for `Put solution and project in the same directory`
   for the template to work properly.
6. If everything is done correctly, you will follow the prompts and the template will create a new project for you full
   of predefined configurations and code.

## Usage

### Using Command Line

Once installed, create a new project with the template:

```bash
dotnet new slmt -n YourModName --AuthorName "Your Name"
```

Replace `YourModName` with the desired name for your mod project and "Your Name" with your desired author name. The
author name will default to "Azumatt" if not specified.

## Parameters

- `-n` or `--name`: Name of the output directory and the project.
- `--AuthorName`: The name of the mod's author. Default is "Azumatt".

## Feedback and Contributions

Feedback and contributions are welcome! If you find a bug or wish to request a feature, please open an issue.

For contributions:

1. Fork the repository.
2. Create a new branch with your changes.
3. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE.txt).