# hello

This is a hello world demo .NET Nuget package.

## Build & Publish

1. Download dotnet-install script.

```sh
curl -fsSLO https://dot.net/v1/dotnet-install.sh
mv dotnet-install.sh ~
chmod +x ~/dotnet-install.sh
```

2. Install the latest LTS version (6) of .NET SDK and its runtimes.

```sh
~/dotnet-install.sh --channel LTS
dotnet --list-sdks
dotnet new globaljson --sdk-version 6.0.415
```

3. Generate class library project.

```sh
dotnet new classlib
```

Update package metadata in `dotnet.csproj` accordingly.

4. Build.

```sh
dotnet build --configuration Release
dotnet pack --configuration Release
```

5. Publish.

```sh
dotnet nuget push bin/Release/com.pacroy.hello.1.0.0.nupkg --api-key your_api_key
vyimc4wwgji --source https://api.nuget.org/v3/index.json
```

## Install

```sh

```

## Usage

```python

```

## References

- [Create and publish a NuGet package with the dotnet CLI | Microsoft Learn](https://learn.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package-using-the-dotnet-cli)
- [Install .NET on Windows, Linux, and macOS | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/core/install/)
- [global.json overview - .NET CLI | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/core/tools/global-json)
- [Individual accounts - NuGet.org | Microsoft Learn](https://learn.microsoft.com/en-us/nuget/nuget-org/individual-accounts#add-a-new-individual-account)
- [Install and use a NuGet package with the dotnet CLI | Microsoft Learn](https://learn.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-using-the-dotnet-cli)