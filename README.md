# Demo

[![asciicast](https://asciinema.org/a/IArEDLTrQyabI3agSSpINoqNu.svg)](https://asciinema.org/a/IArEDLTrQyabI3agSSpINoqNu)

**In project root:**

```bash
# show help
make
# run auto demo
make auto
```

# Homomorphic hashing in golang

Package **tz** containts pure-Go implementation of hashing function described by Tillich and Źemor in [1] .

There are existing implementations already (e.g. [2]), however it is written in C.

Package **gf127** contains arithmetic in GF(2^127) with _x^127+x^63+1_ as reduction polynomial.

# Description

It can be used instead of Merkle-tree for data-validation, because homomorphic hashes
are concatable: hash sum of data can be calculated based on hashes of chunks.

The example of how it works can be seen in tests.

# Contributing

At this moment, we do not accept contributions. Follow us.

# Makefile

```
→ make
  Usage:

    make <target>

  Targets:

    attach   Attach to existing container
    auto     Auto Tillich-Zémor hasher demo
    down     Stop demo container
    help     Show this help prompt
    up       Run Tillich-Zémor hasher demo
```

# Links

[1] https://link.springer.com/content/pdf/10.1007/3-540-48658-5_5.pdf

[2] https://github.com/srijs/hwsl2-core