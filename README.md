# ManagedCppWpf
Proof of concept how to create cpp executable that runs WPF

# Additional resources: 
This is example from microsoft how to do it with coreclr
- https://github.com/dotnet/samples/tree/main/core/hosting

# VisualStudio 2022 Managed entry point
Microsoft.VisualStudio.Platform.AppDomainManager.dll
VsAppDomainManager.OnStartup

It seems visual studio uses technique where they have pure C++ exe and they call C++/CLI assembly with wrapper around the managed code
