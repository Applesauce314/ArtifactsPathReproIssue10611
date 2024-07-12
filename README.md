reproduces the bug desribed in https://github.com/dotnet/razor/issues/10611.

Edit the line 
```xml
    <ArtifactsPath>$(MSBuildThisFileDirectory)..\artifacts</ArtifactsPath>
```
to
```xml
    <ArtifactsPath>$(MSBuildThisFileDirectory)artifacts</ArtifactsPath>
```
and observe the difference in LSP functionality
