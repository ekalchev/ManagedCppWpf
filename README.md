# ManagedCppWpf
Proof of concept how to create cpp executable that runs WPF

# Additional resources: 
This is example from microsoft how to do it with .net framework
- https://github.com/sphinxlogic/All-In-One-Code-Framework/tree/cf711261c52d51d1c9e903d2395d7f200b392743/Visual%20Studio%202010/CppHostCLR

This is example from microsoft how to do it with coreclr
- https://github.com/dotnet/samples/tree/main/core/hosting
- https://github.com/dotnet/coreclr/blob/master/src/coreclr/hosts/corerun/corerun.cpp

How to debug
- https://github.com/dotnet/coreclr/blob/master/Documentation/building/debugging-instructions.md

# VisualStudio 2022 Managed entry point
Microsoft.VisualStudio.Platform.AppDomainManager.dll
VsAppDomainManager.OnStartup

It seems visual studio uses technique where they have pure C++ exe and they call C++/CLI assembly with wrapper around the managed code
