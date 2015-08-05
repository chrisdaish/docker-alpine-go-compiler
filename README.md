Alpine Linux Go Compiler
========================

This image exists to assist in compiling Go binaries for Alpine Linux. Alpine Linux does not use glibc, instead it uses musl, thus we need to compile custom binaries.

How to use
----------

```
docker run  -v $PWD/<goSRC>:/go/src \
            -w /go/src \
            --rm \
           chrisdaish/alpine-go-compiler go build -o <binary>
```
