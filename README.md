# Node Manager Builder

Make building [HPC Pack Linux Node Manager](https://github.com/coolmay/whpc-linux-communicator) super easy!

## Quick Start

```bash
git clone --recursive https://github.com/coin8086/node-manager-builder.git
cd node-manager-builder
./build-in-docker
```

All done! Check the release dir for result!

## Build Latest Source Code

```bash
git clone --recursive https://github.com/coin8086/node-manager-builder.git
cd node-manager-builder/src/whpc-linux-communicator
git fetch && git checkout origin/v2
cd ../..
./build-in-docker
```

The Node Manager Builder uses Git Submodule to manage the source code of [HPC Pack Linux Node Manager](https://github.com/coolmay/whpc-linux-communicator) and its dependencies: [C++ REST SDK](https://github.com/EvanCui/cpprestsdk) and [spdlog](https://github.com/EvanCui/spdlog). By default it locks the Git revision of these submodules. So if you want to get the latest code of any of them, go into the subdirectory(a git repo) of src, and check out the revision you want.
