#### dump-jpeg-coeffs.exe
Usage:
```
usage:dump-jpeg-coeffs <input.jpg> [output.dctdump]
```

Dumps the raw DCT blocks of the input image into a binary file. The output file follows the following liear layout:
1. The number of components as `UInt16`
2. For each block:
  2.1 widthInBlocks as `UInt16`
  2.2 heightInBlocks as `UInt16`
3. The block data as a raw `UInt16` dump
