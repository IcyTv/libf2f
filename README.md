# LibF2F

libf2f is a (work-in-progress) C++ boost/asio library for building p2p networks

## Provides:
* network servent/router
* connection handling and abstraction
* message class that is marshalled to/from the network
* very simple test app (only supports ping+pong)

## Does not provide:
* high level protocol, you have to design implement this yourself
  (ie, extend the Protocol class)

## Build instructions
```bash
# This is just to keep your files clean
mkdir build
cd build

#This generates the files you need to build
cmake ..

#This builds the library
make

##(Optional) This installs the library.
sudo make install
```

# Usage
To use the library in your project add
`-lf2f` to your compiler instructions after installing it
