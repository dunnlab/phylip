# phylip

This repo contains the source code of phylip, written by Joe Felsenstein et al., and downloaded on January 8, 2021 from https://evolution.genetics.washington.edu/phylip/getme-new1.html .

## Compiling

Generally builds on https://evolution.genetics.washington.edu/phylip/install.html .

    docker run -it dunnlab/ubuntu-dev:20.04 /bin/bash
    git clone https://github.com/dunnlab/phylip.git
    cd phylip/phylip-3.697/src/
    make -f Makefile.unx install
    export PATH="/phylip/phylip-3.697/exe:$PATH"

# Running

I include a few datasets
- `test.phy` is from the [dnaml documetnation](https://evolution.genetics.washington.edu/phylip/doc/dnaml.html)
- `siph16s.phy` is a quick siphonophore dataset I made
- `alignment.phy` is from [this primer](https://evolution.genetics.washington.edu/phylip/tuimala3.pdf)

To run a test datasets:

    cd /phylip
    dnaml

Then enter the name of the dataset.

