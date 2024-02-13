# gtest
### googletest
git clone https://github.com/google/googletest.git -b v1.14.0
sudo apt-get install libgtest-dev
cmake -Bbuild
cmake --build build
sudo cmake --build build --target install




### cmake install
sudo apt purge --autoremove cmake
mkdir cmake
cd cmake/
wget https://github.com/Kitware/CMake/releases/download/v3.28.3/cmake-3.28.3.tar.gz
tar -xvf cmake-3.28.3.tar.gz
cd cmake-3.28.3/
./bootstrap
make -j$(nproc)
sudo make install
sudo apt install libssl-dev
sudo ln -s /usr/local/bin/cmake /usr/bin/cmake
cmake --version


##

cmake -S . -B build && cmake --build build
