# ofxPCL

PointCloudLibrary for openFrameworks

- tested with openFrameworks v0.11.2 / PCL 1.13.0 / Visual Studio 2022 / Windows

- if mac or linux, you will need to modify `addon_config.mk` to specify include / lib files (planning to test them in the future)

## Usage

for Windows:

- Install PCL via AllInOne exe: https://github.com/PointCloudLibrary/pcl/releases/

- Copy `include, bin, lib` dirs to ofxPCL dir from `C:\Program Files\PCL 1.13.0\`

- Use ProjectGenerator to generate your project (include ofxPCL in addons)

- Modify your Visual Studio project to use `Visual Studio 2022 (v143)` Platform Toolset (and also openFrameworksLib project)