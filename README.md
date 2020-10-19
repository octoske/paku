paku is a collection of decompressors and decompressor adapters in pure Rust with no unsafe code in paku itself

##### Goals
1. Pure Rust. No unsafe code.
2. Support all reasonably modern popular formats for decompression. 
3. No dependency on external decompression code.
4. Be reasonably fast. Currently unknown.

##### Distant future goals
1. Support some specific compression format or two. Tbd which one. Most likely zstd.
2. Provide no_std support.
3. ARM and x86 asm.

##### Supported formats
format | status | notes
--- | --- | ---
lzf | fully implemented | 
lz4 in LZ4Block | lz4_jblock implements format compatible with https://github.com/lz4/lz4-java/blob/master/src/java/net/jpountz/lz4/LZ4BlockInputStream.java | this format does not seem to be supported by any other libraries, however there are unfortunately compressed files using it around
