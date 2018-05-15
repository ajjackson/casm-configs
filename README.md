# CASM configs

Dockerfiles and related notes for working with CASM

Derived from [this
post](https://github.com/prisms-center/CASMcode/issues/96#issuecomment-349442379)
by Brian Puchala to the CASM issue tracker

## Usage
Copy dockerfile to an empty directory and rename it _Dockerfile_.
Within that directory

``` shell
sudo docker build -t my-casm-test .
```

To begin an interactive session

``` shell
sudo docker run -it my-casm-test
```
where _my-casm-test_ is the label given when building the Docker image.
If there is not a shell command at the end of the Dockerfile,
append it to the run command (i.e. `sudo docker run -it my-casm-test /bin/bash`)
