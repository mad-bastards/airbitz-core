# git-sync

This is a tiny library and command-line utility for syncing files using Git.
The library runs inside the mobile app,
and the command-line utility runs on the server.

## Building

You will need the following tools to build the library:

```
brew install cmake git libtool pkgconfig
```

First, install libgit2 v0.23.4 on your computer:

```sh
git clone git@github.com:libgit2/libgit2.git
cd libgit2
git checkout v0.23.4

# Now follow the libgit2 readme file:
mkdir build && cd build
cmake ..
cmake --build .
cmake --install .
```

Now run `make` in this folder to build the `sync` executable. Note that some users prefer to rename the `sync` binary to `ab-sync`.
