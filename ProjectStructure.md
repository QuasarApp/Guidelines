# Structure of QuasarApp Projects

## Strict observance

* All Projects created after 01/01/2020 must be new structure:
```
Main git repository
├── Main build system file (cmake or qmake)
├── ProjectDir(src)
|   ├── Private submodule for Project
|   ├── src
│   │   ├── sources files
|   |   └── resources files (or folder with resources files)
|   └── Build system file (cmake or qmake)
├── Tests
│   ├── Private submodule for tests
│   ├── src
│   │   ├── sources files
|   |   └── resources files (or folder with resources files)
|   └── Build system file (cmake or qmake)
├── Doc/Docs
│   ├── Private submodule for documentation
│   └── Documentation files
└── Global submodule for all projects

```

## Recommendations
* Use CMake build system


# For create new repositoy use the [CMakeProject](https://github.com/QuasarApp/CMakeProject) template.
