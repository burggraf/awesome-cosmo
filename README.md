# awesome-cosmo
![logo](awesome-cosmo.png)

This is a curated list of apps compiled for [Cosmopolitan Libc](https://github.com/jart/cosmopolitan):

> Cosmopolitan Libc makes C a build-once run-anywhere language, like Java, except it doesn't need an interpreter or virtual machine. Instead, it reconfigures stock GCC and Clang to output a POSIX-approved polyglot format that runs natively on Linux + Mac + Windows + FreeBSD + OpenBSD + NetBSD + BIOS with the best possible performance and the tiniest footprint imaginable.

## The List

### Redbean
[Redbean: single-file distributable web server](https://justine.lol/redbean/)

[Direct Download](https://justine.lol/redbean/redbean-1.0.com)

> All you need to do is download the redbean.com program below, change the filename to .zip, add your content in a zip editing tool, and then change the extension back to .com.

> redbean can serve 1 million+ gzip encoded responses per second on a cheap personal computer. 

> It embeds the Lua programming language which lets you write dynamic pages.

> All in 592kb.  kb.  not mb.  not gb.  kb.  592,145 bytes.

### SQLite 3.35.5
> SQLite is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine. SQLite is the most used database engine in the world.

[SQLite3 Page](https://github.com/burggraf/awesome-cosmo/tree/main/apps/sqlite3)

[Direct Download](https://github.com/burggraf/awesome-cosmo/raw/main/apps/sqlite3/sqlite3.35.5.com)

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

