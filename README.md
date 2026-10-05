git clone https://gitlab.com/Tritonn204/tnn-miner.git
cd tnn-miner
mkdir build
cd build
# 💡 優化點：加上靜態編譯參數，確保打包所有依賴在庫中
cmake -DCMAKE_BUILD_TYPE=Release -DBUILD_SHARED_LIBS=OFF -DCMAKE_EXE_LINKER_FLAGS="-static" ..
make -j$(nproc)
