# How to use static sfml on windows with vcpkg? 

Clone this repo and the vcpkg submodule by running `git clone --recurse-submodules https://github.com/autoantwort/sfml-vcpkg-static.git` 

Then configure and build the project. You can use the `windows static` preset or pass the following options to cmake: `-DCMAKE_TOOLCHAIN_FILE=<path to vcpkg>/scripts/buildsystems/vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-windows-static`. 
