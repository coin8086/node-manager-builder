# Node Manager Builder

Build [HPC Pack Linux Node Manager](https://github.com/coolmay/whpc-linux-communicator) super easy:

```bash
git clone --recursive https://github.com/coin8086/node-manager-builder.git
cd node-manager-builder
./build-in-docker
```

All done! Check the release dir for result!

## Known issue:
Since some fault in underlying repo, you may need to run `build-in-docker` again to get complete result, otherwise some dependent libraries may be missing. Anyway, it takes only seconds to run `build-in-docker` again.
