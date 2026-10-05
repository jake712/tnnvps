git clone https://gitlab.com/Tritonn204/tnn-miner.git

cd tnn-miner

mkdir build

cd build

cmake -DCMAKE_BUILD_TYPE=Release -DBUILD_SHARED_LIBS=OFF -DCMAKE_EXE_LINKER_FLAGS="-static" ..

make -j$(nproc)
