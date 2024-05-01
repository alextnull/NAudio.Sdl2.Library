# NAudio.Sdl2.Library
This package contains native SDL2 libraries

---
# .NET
Include the package using the `PackageReference` tag or simply install using the nuget package manager
```xml
 <ItemGroup>
  <PackageReference Include="NAudio.Sdl2.Library" Version="2.26.0" />
 </ItemGroup>
```
---
# .NET Framework
Include the package using the `PackageReference` tag. Set `GeneratePathProperty` to `true` and `ExcludeAssets` to `all`.
```xml
 <ItemGroup>
  <PackageReference Include="NAudio.Sdl2.Library" Version="2.26.0" GeneratePathProperty="true" ExcludeAssets="all"/>
 </ItemGroup>
```
---

Copy `SDL.dll` to the output directory using the `None` tag.

Windows x86
```xml
 <ItemGroup>
  <None Include="$(PkgNAudio_Sdl2_Library)\runtimes\win-x86\native\SDL2.dll">
   <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
  </None>
```

Windows x64
```xml
 <ItemGroup>
  <None Include="$(PkgNAudio_Sdl2_Library)\runtimes\win-x64\native\SDL2.dll">
   <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
  </None>
```
