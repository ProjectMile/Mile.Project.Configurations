# Mile.Project.Configurations Release Notes

**Mile.Project.Configurations 1.0.2060.0**

- Rollback C++/WinRT to 2.0.250303.1 because 
  https://github.com/microsoft/cppwinrt/issues/1605.

**Mile.Project.Configurations 1.0.2059.0**

- Fix the LanguageStandard_C variable selection logic issue.
- Decouple more project configurations from specific configuration profiles.
- Simplify the condition logic for project configurations.
- Update C++/WinRT to 3.0.260520.1.
- Update YY-Thunks to 1.2.2-Beta.2.

**Mile.Project.Configurations 1.0.1917.0**

- Add workaround for using NuGet Package References Support in Visual Studio
  2026 version 18.3 or later. (Cooperated with AndromedaMelody.)
- Update VC-LTL to 5.3.1.
- Update YY-Thunks to 1.2.1-Beta.1.

**Mile.Project.Configurations 1.0.1827.0**

- Fix the issue when using MileProjectUseClangCLToolset option. (Thanks to
  dinhngtu.)
- Update VC-LTL to 5.3.1-Beta2.
- Update YY-Thunks to 1.1.9.

**Mile.Project.Configurations 1.0.1768.0**

- Add workaround to Mile.Project.Wap.targets for solving the issue that
  unnecessary XAML files contained in the final MSIX package.
- Add workaround to Mile.Project.Cpp.targets for solving the App.xaml resource
  not found issue if users want to put App.xaml to dynamic library project
  instead of application project.

**Mile.Project.Configurations 1.0.1766.0**

- Adapt to Visual Studio 2026 via fixing the C and C++ language standard
  configurations. (Contributed by dongle-the-gadget.)
- Update C++/WinRT to 2.0.250303.1.
- Update VC-LTL to 5.2.2.
- Update YY-Thunks to 1.1.8.
- Fix the source code file header comment format.

**Mile.Project.Configurations 1.0.1622.0**

- Remove unnecessary customization support for PlatformToolset option in Windows
  driver projects to fix some issues. (Contributed by MiroKaku.)

**Mile.Project.Configurations 1.0.1621.0**

- Fix the condition check for Mile.Project.Build.
- Update VC-LTL and YY-Thunks to their latest stable version. (Contributed by
  MiroKaku.)
- Add customization support for WindowsTargetPlatformVersion option. (Suggested
  by sonyps5201314.)
- Add customization support for PlatformToolset option. (Suggested by
  sonyps5201314.)

**Mile.Project.Configurations 1.0.1426.0**

- Initial release.
- Inherit and integrate Mile.Project.Platform from
  https://github.com/ProjectMile/Mile.Project.Windows/tree/20241012-BeforeNuGetSDK.
- Fix the condition check for Mile.Project.Platform x86.
- Add empty SDK configurations for simplifying the configurations.
- Fix the file header for Mile.Project.Platform.
- Inherit and integrate Mile.Project.Version from
  https://github.com/ProjectMile/Mile.Project.Windows/tree/20241012-BeforeNuGetSDK.
- Inherit and integrate Mile.Project.Manifest from
  https://github.com/ProjectMile/Mile.Project.Windows/tree/20241012-BeforeNuGetSDK.
- Inherit and integrate Mile.Project.Cpp from
  https://github.com/ProjectMile/Mile.Project.Windows/tree/20241012-BeforeNuGetSDK.
- Inherit and integrate Mile.Project.Wap from 
  https://github.com/ProjectMile/Mile.Project.Windows/tree/20241012-BeforeNuGetSDK.
- Inherit and integrate Mile.Project.Build from
  https://github.com/ProjectMile/Mile.Project.Windows/tree/20241012-BeforeNuGetSDK.
- Set BackgroundTaskDebugEngines to NativeOnly in Mile.Project.Wap.props.
- Introduce MileProjectOutputPath, MileProjectCppDisablePackageReferencesSupport
  and MileProjectWapDisableNativeProjectWorkarounds options.
