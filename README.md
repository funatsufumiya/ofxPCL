# ofxPCL

PointCloudLibrary for openFrameworks

- tested with openFrameworks v0.11.2 / PCL 1.13.0
    - Visual Studio 2022 / Windows 11 (22H2)
    - Xcode 14.2 / macOS Ventura 13.2.1, M1 2020

- if linux, you will need to modify `addon_config.mk` to specify include / lib files (planning to test them in the future)

## Usage

### Windows

- Install PCL via AllInOne exe: https://github.com/PointCloudLibrary/pcl/releases/

- Copy `include, bin, lib` dirs to ofxPCL dir from `C:\Program Files\PCL 1.13.0\`

- Use ProjectGenerator to generate your project (include ofxPCL in addons)

- Modify your Visual Studio project to use `Visual Studio 2022 (v143)` Platform Toolset (and also openFrameworksLib project)

### Mac

```bash
$ brew install pcl
$ cd /your/path/to/ofxPCL
$ cp -r /opt/homebrew/Cellar/pcl/1.13.0_2/include include
$ cp -r /opt/homebrew/Cellar/pcl/1.13.0_2/lib lib
$ cp -r /opt/homebrew/Cellar/eigen/3.4.0_1/include/* include
```

- Use ProjectGenerator to generate your project (include ofxPCL in addons)

- Modify your XCode project to use `C++14` (or more): `Build Settings > Apple Clang - Language - C++ > C++ Language Dialect` set to C++14
