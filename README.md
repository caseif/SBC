\# SBC
The **S**tructured **B**lob **C**ontainer format is a specification for storing arbitrary binary data in a hierarchical
manner within a single byte blob. The full specification for the format may be found in the
[wiki](https://github.com/caseif/SBC/wiki/Specification) of this repository.

This repository will also house utilities for working with the format in the near future.

## What SBC *Isn't*
Here is a small list of things SBC is **not** designed to do:

- Store metadata for blobs
  - SBC is designed exclusively to hold binary data, without the bells and whistles. The above task is more suited for a
    multi-purpose format such as [NBT](http://wiki.vg/NBT).
- Compress data
  - SBC is literally just a container format. The data chunk will be slightly larger than all input data. However, it
    should be trivial to run a data chunk through `gzip`.
- Your taxes

## Why?
Partly because I need a format for storing byte data compactly, and partly because it gives me the opportunity to
practice my skill in various programming languages.
