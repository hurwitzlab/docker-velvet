# docker-velvet

To make a working Docker image:

* Build velvet[g|h] into a "bin" directory here
* docker build -t velvet .

To run:

    $ docker run --rm -v ~/data:/data -w /data velvet \
    velveth velvet-out 21 mouse.fa

    $ docker run --rm -v ~/data:/data -w /data velvet \
    velvetg velvet-out -cov_cutoff 4
