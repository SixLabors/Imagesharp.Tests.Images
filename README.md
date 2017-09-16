# Imagesharp.Tests.Images
External image repository to support ImageSharp testing. It's main purpose is to hold reference images for regression tests.


### ReferenceOutput
Contains images to validate against in ImageSharp tests. In most cases the file hierarchy follows the hierarchy of `ActualOutput`

### tools
Various utilities to help dealing with images.
- `optipng.exe`: [lossless PNG compressor](http://optipng.sourceforge.net/), to keep the `ReferenceImages` repository as small as possible
- `optimize-all.cmd`: Runs lossless optimizer for reference PNG-s. Currently it has to be manually edited to add new test class directories.
- [`dump-jpeg-coeffs.exe`](https://github.com/SixLabors/Imagesharp.Tests.Images/blob/master/tools/jpeg/README.md)
