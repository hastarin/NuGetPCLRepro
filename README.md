# NuGetPCLRepro
Simple example to demonstrate a bug in NuGet.exe (2.8.60717.93 or 3.1.0.0 Beta) with nuspec package generation, token replacement, and PCL packages.

Generation via a project works as expected:
Using NuGet.exe 2.8.60717.93 we get the following:
> nuget pack
Attempting to build package from 'NuGetPCLRepro.csproj'.
Packing files from 'C:\Users\jon.benson\Documents\GitHub\NuGetPCLRepro\NuGetPCLRepro\bin\Release'.
Using 'NuGetPCLRepro.nuspec' for metadata.
Successfully created package 'C:\Users\jon.benson\Documents\GitHub\NuGetPCLRepro\NuGetPCLRepro\NuGetPCLRepro.1.0.0.0.nup
kg'.

Generation via a nuspec files:
> nuget pack NuGetPCLRepro.nuspec
Attempting to build package from 'NuGetPCLRepro.nuspec'.
The replacement token 'id' has no value.
