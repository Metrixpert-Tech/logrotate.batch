# Log rotation for Microsoft Windows

::

### Usage: ``` logrotate.bat filename maxfilecount [maxfilesize] ```

filename    : The file name to rotate.

maxfilecount: Number of backup files.

maxfilesize : Rotated if the size of file exceeds specified size. (Default is 0. Unit notation is available (K, M and G))


## Example:

##### logrotate.bat path\to\file 1

:: The file is renamed to path\to\file.1.

:: The file path\to\file.1 is deleted if exists.

##### logrotate.bat path\to\file 100 128

:: The file is rotated from path\to\file.1 to file\to\file.100

:: if the size exeeds 128 bytes.

##### logrotate.bat path\to\file 10 10M

:: The file is rotated from path\to\file.1 to file\to\file.10

:: if the size exeeds 10 Mega-bytes.
