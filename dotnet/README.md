# hello

This is a hello world demo .NET Nuget package.

## Install

```sh

```

## Usage

```python

```

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

3. aaa

## References

- [Install .NET on Windows, Linux, and macOS | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/core/install/)
- [Create and publish a NuGet package with the dotnet CLI | Microsoft Learn](https://learn.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package-using-the-dotnet-cli)