sudo apt update

git clone --recursive https://github.com/dmlc/tvm

sudo apt install git

git clone --recursive https://github.com/dmlc/tvm

sudo apt update

sudo apt install -y python3 python3-dev python3-setuptools gcc libtinfo-dev zlib1g-dev build-essential cmake

cd tvm

mkdir build

cp cmake/config.cmake build

sudo apt install vim

==================================================

vi build/config.cmake

"set(USE_LLVM ON)"

==========================================

sudo apt install clang

cd build

cmake ..

make -j4

=========================================

vi ~/.bashrc

export TVM_HOME=/home/aquapapaya/tvm

export PYTHONPATH=$TVM_HOME/python:$TVM_HOME/topi/python:$TVM_HOME/nnvm/python:${PYTHONPATH}

============================================

sudo apt install python3-pip

pip3 install --user numpy decorator attrs

================================================

pip3 install https://download.pytorch.org/whl/cpu/torch-1.1.0-cp36-cp36m-linux_x86_64.whl

pip3 install torchvision

=============================================================================================

TVM可以稱為許多工具集的集合，其中這些工具可以組合起來使用，來實現我們的一些神經網絡的加速和部署功能。這也是為什麼叫做TVM Stack

TVM可以優化的訓練好的模型，並將你的模型打包好，然後你可以將這個優化好的模型放在任何平台去運行

TVM源碼是由C++和Pythoh共同搭建

=============================================================================================

pip3 install jupyter

"restart your PC"

jupyter notebook
