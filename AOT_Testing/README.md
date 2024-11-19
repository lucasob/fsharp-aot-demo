# AOT Testing

DotNet 8.0 AOT (ahead of time) compilation magic. This program is intentionally bare, but I can imagine I'll want to
look back on it.

### Build

OS Options:

* osx-arm64
* osx-x64
* linux-x64 (I think)

```shell
dotnet publish -r osx-arm64 -c Release -p:PublishAot=true --self-contained
```

### Invoke

Assuming you ran build and are on linux/mac (windows you're on your own sorry)

```shell
./AOT_Testing/bin/Release/net8.0/osx-arm64/AOT_Testing --name Lucas --age 27
```
