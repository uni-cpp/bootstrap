mkdir build
cd build
cmake -G'CodeBlocks - Ninja' -DCMAKE_BUILD_TYPE=Debug ..
cmake --build .
cmake --build . -- install
