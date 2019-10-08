MongoDB F# Driver Prototype
===========================

This is a continuation of the development on a prototype MongoDB driver 
written for F#. The original project was never advanced beyond a POC,
but it did establish a pattern from using MongoDB from F# more natural 
by defining new ways to express database/collection operations 
that are idiomatic to the language.  As such, this fork is intended to
carry on that work and provide a stable version of the library that can 
ultimately be used in a Production system.

#### Note

The API and implementation are still in early development and may change.
You probably won't want use this driver in production, as it has not been 
tested and is in no way supported by MongoDB, Inc.

Dependencies
------------

  * F# 3.0

Building
--------

The F# driver has been developed on top of the refactored [Core .NET
driver](https://github.com/mongodb/mongo-csharp-driver/tree/v2.0).
This new ***Core .Net driver*** is still in development as well, and
hence unavailable on NuGet. Thus, the branch has been setup as a
submodule. This is intended to change in the future.

    git submodule update --init
    <compile mongo-csharp-driver>
    <compile mongo-fsharp-driver-prototype>

License
-------

[Apache v2.0](LICENSE)
