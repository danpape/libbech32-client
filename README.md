# libbech32-client

This is a simple client application for testing the [libbech32 library.](https://github.com/dcdpr/libbech32)

## Building libbech32-client

To build libbech32-client, you will need:

* cmake
* g++, clang or Visual Studio (community edition)

libbech32-client uses a pretty standard cmake build system. If you have already built and installed [libbech32](https://github.com/dcdpr/libbech32) you should be able to execute:

```
mkdir build
cd build
cmake ..
make
```

If you have installed libbech32 to some special location you can try:

```
mkdir build
cd build
cmake -DCMAKE_PREFIX_PATH=/tmp/bech32-install ..
make
```

You can then run the simple "hello world" application:

```
> ./libbech32_client
bech32 encoding of human-readable part 'hello' and data part '[14, 15, 3, 31, 13]' is:
hello1w0rldjn365x
```
