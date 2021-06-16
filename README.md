# awesome-cosmo
![logo](awesome-cosmo.png)

This is a curated list of apps compiled for [Cosmopolitan Libc](https://github.com/jart/cosmopolitan):

> Cosmopolitan Libc makes C a build-once run-anywhere language, like Java, except it doesn't need an interpreter or virtual machine. Instead, it reconfigures stock GCC and Clang to output a POSIX-approved polyglot format that runs natively on Linux + Mac + Windows + FreeBSD + OpenBSD + NetBSD + BIOS with the best possible performance and the tiniest footprint imaginable.

## The List

### Redbean
[Redbean: single-file distributable web server](https://justine.lol/redbean/)

[Direct Download 1.3](https://justine.lol/redbean/redbean-1.3.com)

> All you need to do is download the redbean.com program below, change the filename to .zip, add your content in a zip editing tool, and then change the extension back to .com.

> redbean can serve 1 million+ gzip encoded responses per second on a cheap personal computer. 

> It embeds the Lua programming language which lets you write dynamic pages.

> It embeds Sqlite 3.35.5.

> All in 1.1mb.  not gb.  mb.  1,149,201 bytes.

>features
>HTTP v0.9
>HTTP v1.0
>HTTP v1.1
>Lua v5.4
>SQLite 3.35.5
>Pipelining
>Monitoring
>Accounting
>Content-Encoding
>Range / Content-Range
>Last-Modified / If-Modified-Since

### SQLite 3.35.5
> SQLite is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine. SQLite is the most used database engine in the world.

[SQLite3 Page](https://github.com/burggraf/awesome-cosmo/tree/main/apps/sqlite3)

[Direct Download from justine.lol](https://justine.lol/redbean/sqlite3.com)

- Compile directions here (requires linux environment): https://github.com/jart/cosmopolitan/pull/162
- [SQLite Home Page](https://www.sqlite.org)

### Wasm3
> The fastest WebAssembly interpreter, and the most universal runtime.

[Wasm3 Github Page](https://github.com/wasm3/wasm3)

[Direct Download](https://github.com/wasm3/wasm3/releases/download/v0.4.9/wasm3-cosmopolitan.com)

### Lua

[Compiling Lua Comment](https://github.com/jart/cosmopolitan/issues/61#issuecomment-814394064)
```
git clone git@github.com:jart/cosmopolitan.git
cd cosmopolitan
make -j8 o//third_party/lua/lua.com
```

[Direct Download](https://justine.lol/cosmopolitan/lua.com)

### QuickJS
> QuickJS is a small and embeddable Javascript engine. It supports the ES2020 specification including modules, asynchronous generators, proxies and BigInt.

[QuickJS Javascript Engine](https://bellard.org/quickjs)

[Official Repo](https://github.com/jart/cosmopolitan/tree/master/third_party/quickjs)

[Direct Download](https://github.com/burggraf/awesome-cosmo/raw/main/apps/QuickJS/qjs.com)

[Direct Zip Download](https://github.com/burggraf/awesome-cosmo/raw/main/apps/QuickJS/qjs.zip)

### Python 2.7
> This repo contains the source code of Python 2.7.18 customized to compile with Cosmopolitan libc. Meant for experimental purposes only.

[Repo: Compiling Python2.7 with Cosmopolitan](https://github.com/ahgamut/cpython/tree/cosmo_py27)

[Direct Zip Download](https://github.com/burggraf/awesome-cosmo/raw/main/apps/python2.7/python.zip)
- NOTE: There is a required file inside the zip,lib/python27.zip, which contains Python built-in libraries.


