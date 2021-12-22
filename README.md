# ndnSIM
Named Data Networking(NDN) is one of the architecture of Information-Centric Networking. T
## Installation of Required Packages
I have used Ubuntu 20.04 to run and simulate it.
1. ##### sudo apt install build-essential libsqlite3-dev libboost-all-dev libssl-dev git python3-setuptools castxml
2. ##### sudo apt install gir1.2-goocanvas-2.0 gir1.2-gtk-3.0 libgirepository1.0-dev python3-dev python3-gi python3-gi-cairo python3-pip python3-pygraphviz python3-pygccxml 
3. ##### sudo pip3 install kiwi

## Download the Source Code of ndnSIM
Make the directory called ndnSIM and navigate inside it. Then download the following source codes.
1. ##### git clone https://github.com/named-data-ndnSIM/ns-3-dev.git ns-3
2. ##### git clone https://github.com/named-data-ndnSIM/pybindgen.git pybindgen
3. ##### git clone --recursive https://github.com/named-data-ndnSIM/ndnSIM.git ns-3/src/ndnSIM

## Compiling and Running ndnSIM with Visualizer.
1. ##### cd ns-3
2. ##### ./waf configure --enable-examples
3. ##### ./waf
Note: Due to the hardware specification of my laptop, the installation ran infinitely. The latop RAM was just 4GiB. It used up 100% of it. So, the reason was due to the compilation of visualizer. Therefore, I decided to disable the visualizer and install it.
### Compiling and Running ndnSIM without Visualizer.
1. ##### cd ns-3
2. ##### ./waf configure --disable-python --enable-examples
3. ##### ./waf

Now I was able to compile and build the source code successfully.
## Running Simulation
