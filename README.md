# dectris-neggia
Here is a precompiled Neggia XDS plugin for Apple Silicon macOS. It enables XDS to read HDF5 files written by Dectris Eiger detectors.

```bash
➜  lib file dectris-neggia.so
dectris-neggia.so: Mach-O 64-bit bundle arm64
➜  lib otool -L dectris-neggia.so
dectris-neggia.so:
	/usr/lib/libc++.1.dylib (compatibility version 1.0.0, current version 2100.43.0)
	/usr/lib/libSystem.B.dylib (compatibility version 1.0.0, current version 1356.0.0)
➜  lib otool -hv dectris-neggia.so
dectris-neggia.so:
Mach header
      magic  cputype cpusubtype  caps    filetype ncmds sizeofcmds      flags
MH_MAGIC_64    ARM64        ALL  0x00      BUNDLE    16       1448   NOUNDEFS DYLDLINK TWOLEVEL WEAK_DEFINES BINDS_TO_WEAK
➜  lib

```
