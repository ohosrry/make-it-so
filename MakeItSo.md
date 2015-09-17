### Overview ###
MakeItSo converts Visual Studio solutions to gcc makefiles. Its aim is to support all recent versions of Visual Studio, and to be able to convert many types of projects including:
  * VS2008 and VS2010 support.
  * C and C++ executables, static libraries and dlls.
  * C# executables and class-library assemblies.
  * Projects with libraries linked implicitly via project dependencies.
  * Libraries that link in dependent libraries.
See the [project roadmap](ProjectRoadmap.md) the current state of the project.

### Links to further details ###

  * [The MakeItSo command line.](CommandLine.md)
  * [Description of the makefiles generated by MakeItSo.](GeneratedMakefiles.md)
  * [How to convert more complex projects that need extra information provided as a MakeItSo.config file.](MakeItSoConfig.md)
  * [Building for cygwin.](BuildingForCygwin.md)
  * [Paths with spaces.](PathsWithSpaces.md)
  * [Converting DLLs to build as gcc shared-objects libraries](ConvertingDLLs.md)
  * [Merging static libraries](MergingStaticLibraries.md)


### One-off vs. continuous conversion ###
There are two main ways you can use MakeItSo:
  * One-off conversion of a solution, so that you can then maintain the makefile manually after that.
  * Working in Visual Studio, and continually converting the solution to a makefile to cross-compile for Linux.

Many solutions can be converted by MakeItSo with no extra information needed. But for some projects you may need or want to provide extra information that is not found in the Visual Studio solution or project files. For example, you may want to change preprocessor definitions or libraries and library paths.

To perform continuous conversion of solutions that need extra information, you can provide a `MakeItSo.config` file.


### Contributing ###
Please get in touch if you would like to contribute to the project.