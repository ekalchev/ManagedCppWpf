# ManagedCppWpf
Proof of concept how to create cpp executable that runs WPF

# Additional resources: 
https://social.msdn.microsoft.com/Forums/vstudio/en-US/0a0342e4-caec-42d0-bfe5-e0930883f141/how-do-i-invoke-net-assembly-from-native-c-code?forum=vcgeneral
https://github.com/sphinxlogic/All-In-One-Code-Framework/tree/cf711261c52d51d1c9e903d2395d7f200b392743
Look for CppCallNETAssemblyWrapper

# VisualStudio 2022 Managed entry point
Microsoft.VisualStudio.Platform.AppDomainManager.dll
VsAppDomainManager.OnStartup

It seems visual studio uses technique where they have pure C++ exe and they call C++/CLI assembly with wrapper around the managed code
