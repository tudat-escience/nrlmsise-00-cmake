# nrlmsise-00

This repository has been copied directly from https://www.brodo.de/space/nrlmsise/ for use in the TU Delft Astrodynamics Toolbox (Tudat) ecosystem. The copyright of the code belongs to Dominik Brodowski.

* For more details on Tudat, we refer to the [project website](https://docs.tudat.space/en/latest/) and our [project Github main page](https://github.com/tudat-team)
* Conda package for this repository are available on [anaconda](anaconda.org/tudat-team/nrlmsise-00/), which is built through the [tudat-feedstock](https://github.com/tudat-team/nrlmsise-00-feedstock) on [Azure](https://dev.azure.com/tudat-team/feedstock-builds/_build?definitionId=7)

## Build, test and install

To build and test this code locally:

```bash
cmake -S . -B build
make -C build
```

This creates both the `nrlmsise-00.so` shared library and the `nrlmsise-00_test` executable.

To install (for example in `~/.local`), run

```bash
cmake -S . -B build -DCMAKE_INSTALL_PREFIX=${HOME}/.local && make install
```

## License

FIXME. There is currently no proper license attached to this work.

