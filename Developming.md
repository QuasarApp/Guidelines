# Developing in the QuasarApp group

QuasarApp group developing guid. This page collected all guides for using programming languages. 

## C++

For build c++ projects QuasarApp group use the CMake build system.
1. All new projects should be created using our [cmake](https://github.com/QuasarApp/CMakeProject) tempalte. 
2. All projects files must be copyrighted.
    > Copyright example:
    ``` cpp

    //#
    //# Copyright (C) 2021-2021 QuasarApp.
    //# Distributed under the lgplv3 software license, see the accompanying
    //#
    ```
3. All projects must have a tests, main shared and static library and executable file for using a main library. For more information about structure projects see [this](ProjectStructure.md) guide. 

4. All projects should be support next cmake targets: 
    * test - for run tests.
    * deploy - for create a distribution kits.
    * release - for prepare signed distro packages and update repositories
    * doc - for generate technical documentation.
    > Do not worry. All targets alredy support in our [CMake](https://github.com/QuasarApp/CMake) toolchains and [CMakeProject](https://github.com/QuasarApp/CMakeProject) templates. 
5. All functions and classes must be documented using doxygen comments. For more information about syntaxis of the doxygen comments see the [doxygen](https://www.doxygen.nl/manual/docblocks.html) documentation
    > Example:
    ``` cpp
    /**
    * @brief qHash are Simple hash function of the Random object
    * @param rand are Input data.
    * @return crc32 hash code.
    */
    uint qHash(Random rand);
    ```
6. All develops library classes must be implemented on the library namespace to avoid conflicts with the names of other libraries.
    > Example 
    ``` cpp
    namespace QH {

        /**
        * ...
        */
        class PKG {
            // ...
        }
    }
    ``` 

## Submudules
Almost all quasarapp projects are written so that they can be used as separate modules for new projects. Therefore, the use of submodules is inevitable.
Here are the basic rules for connecting them. 

1. All submodules must be storaged in the **submodules** folder.
2. Do not include dublicate submodules.
3. Use submodules recursive.
    > If you have other submodules in one submodule, you must use the submodules already included recursively in place of adding new ones.
4. In Cmake build system you must be include submodules only there wher ou using it.


# And good luck it will be useful to you 😉 
