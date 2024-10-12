# Mile.Project.Configurations

[![NuGet Package](https://img.shields.io/nuget/vpre/Mile.Project.Configurations)](https://www.nuget.org/packages/Mile.Project.Configurations)

Simplified MSBuild configurations distributed with NuGet package.

## Usage

You only need to import the props/targets you want with the following way.

```
<Import Sdk="Mile.Project.Configurations" Version="Please replace to the Mile.Project.Configurations package version you want" Project=""Please replace to the props/targets you want in the Mile.Project.Configurations package you want" />
```

## Available props/targets

### Mile.Project.Platform

- Mile.Project.Platform.ARM.props
- Mile.Project.Platform.ARM64.props
- Mile.Project.Platform.ARM64EC.props
- Mile.Project.Platform.x64.props
- Mile.Project.Platform.x86.props

### Mile.Project.Cpp

- Mile.Project.Cpp.Default.props
- Mile.Project.Cpp.props
- Mile.Project.Cpp.targets
  
### Mile.Project.Wap

- Mile.Project.Wap.props
- Mile.Project.Wap.targets

## Available Options

### How to define the project type in the "Globals" label property group.

- If the project is a console application project.

```
<MileProjectType>ConsoleApplication</MileProjectType>
```

- If the project is a windows application project.

```
<MileProjectType>WindowsApplication</MileProjectType>
```

- If the project is a dynamic library project.

```
<MileProjectType>DynamicLibrary</MileProjectType>
```

- If the project is a static library project.

```
<MileProjectType>StaticLibrary</MileProjectType>
```

- If the project is a WDM driver project.

```
<MileProjectType>WDMDriver</MileProjectType>
```

- If the project is a KMDF driver project.

```
<MileProjectType>KMDFDriver</MileProjectType>
```

- If the project is a UMDF driver project.

```
<MileProjectType>UMDFDriver</MileProjectType>
```

### How to define the manifest file in the "Globals" label property group.

```
<MileProjectManifestFile>C:\Folder\Manifest.manifest</MileProjectManifestFile>
```

### How to enable the version information support.

```
<MileProjectUseProjectProperties>true</MileProjectUseProjectProperties>
<MileProjectCompanyName>TODO: Company Name</MileProjectCompanyName>
<MileProjectFileDescription>TODO: File Description</MileProjectFileDescription>
<MileProjectInternalName>$(TargetName)</MileProjectInternalName>
<MileProjectLegalCopyright>© TODO: Company Name. All rights reserved.</MileProjectLegalCopyright>
<MileProjectOriginalFilename>$(TargetName)$(TargetExt)</MileProjectOriginalFilename>
<MileProjectProductName>$(TargetName)</MileProjectProductName>
<MileProjectVersion>1.0.0.1</MileProjectVersion>
<MileProjectVersionTag>Preview 1</MileProjectVersionTag>
```

### How to enable VC-LTL support.

```
<MileProjectEnableVCLTLSupport>true</MileProjectEnableVCLTLSupport>
```

Note: YY-Thunks support will be enabled if you have enabled VC-LTL support.

### How to enable C++/WinRT support.

```
<MileProjectEnableCppWinRTSupport>true</MileProjectEnableCppWinRTSupport>
```

### How to use LLVM clang-cl toolset instead of MSVC toolset.

```
<MileProjectUseClangCLToolset>true</MileProjectUseClangCLToolset>
```

### How to use Windows Driver Kit in non-driver projects

```
<MileProjectUseWindowsDriverKit>true</MileProjectUseWindowsDriverKit>
```

### How to define the project as kernel mode project in non-driver projects

```
<MileProjectUseKernelMode>true</MileProjectUseKernelMode>
```

### How to enable YY-Thunks support.

```
<MileProjectEnableYYThunksSupport>true</MileProjectEnableYYThunksSupport>
```
