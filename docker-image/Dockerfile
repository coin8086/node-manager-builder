From ubuntu:14.04
Run apt-get update
Run apt-get -y install g++ git make zlib1g-dev libboost-all-dev libssl-dev cmake

# Install GCC & G++ 4.9 to support C++14
Run apt-get -y install software-properties-common
Run add-apt-repository -y ppa:ubuntu-toolchain-r/test
Run apt-get update
Run apt-get -y install gcc-4.9 g++-4.9
Run update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-4.9 60 --slave /usr/bin/g++ g++ /usr/bin/g++-4.9

Workdir /app
