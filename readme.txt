Synopsis:
  Periodically reads data from a block device keeping it busy

Usage:
  bdbusy [options] BLOCK_DEVICE

Options:
  --blocks N
    Read N blocks per round. Default 256 blocks.
  --blocksize N
    Set the block size to N bytes. Default 4096 bytes.
  --delay N
    Set the delay between reads to N seconds. Default 5 seconds.
  -h, --help
    Display this help message and exit.
  -n N
    Sets the niceness to N (default 0).
  -v
    Show each read round. The same as --verbose 1.
  --verbose #
    Use more or less verbose output. Valid values are from 0 to 1 inclusive:
      0  Default. No output
      1  Show each read round

Examples:
  bdbusy /dev/disk/by-id/ata-ST8000AS0002-1NA17Z_00000000
  bdbusy -v /dev/disk/by-id/ata-ST8000AS0002-1NA17Z_00000000

Version:
  bdbusy 1.1.0.0
  Copyright (C) 2012 Nathan Shearer
  Licensed under GNU General Public License 2.0
