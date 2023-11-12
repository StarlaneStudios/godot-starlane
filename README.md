# Starlane Studios Godot Builds

This repository houses the Godot builds and compiling workflows for the modified version of Godot used by Starlane Studios. You may make use of these builds yourself, however they are tailored to our personal needs and may not be suitable for your own projects.

## Notable modifications
- Only builds .NET enabled builds
- Includes [Godot Voxel](https://github.com/Zylann/godot_voxel) module
- Modified branding

## NuGet packages
In order to use the NuGet packages published to GitHub, you will have to execute the following command

```
dotnet nuget add source \
	--username YOUR_GITHUB_USERNAME \
	--password YOUR_GITHUB_PAT \
	--store-password-in-clear-text \
	--name GitHub \
	"https://nuget.pkg.github.com/macjuul/index.json"
```

Set `YOUR_GITHUB_PAT` to a personal access token generated with access to packages.

## Patches
The Starlane Studios Godot builds are modified using patches. These patches are stored in the `patches` directory. The patches are applied automatically during the build process.

When adding patches, make sure the patch uses `LF` line endings and is defined in `UTF-8` encoding.