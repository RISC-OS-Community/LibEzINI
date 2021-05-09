# LibEzINI
This is a RISC OS port of EzINI a small adn easy to use ANSI C library implementing INI file reading and writing.
This library is intended to be easy to use and build upon.  It is
small in size, thus not as feature complete as other libraries, but should be sufficient to meet most requirements.

## Build the lib
To build from the source just git clone this repo and then go to LibEzINI -> src directory.

### Using GCC
To build these files with GNU make and gcc, simply double click on the file called MkGCC, before you do that make sure that your RISC OS device Filer has seen where your copy of !GCC is (usually in Apps.Development.

### Using ROOL DDE
To build these files with ROOL DDE, simply click on the file called MkDDE, before you do that please make sure your RISC OS device Filer has executed the !SetPaths from DDE which shoul dbe placed in AcornC/C++ directory.

## Using LibEzINI in your code
Have a look at the file called sample in src.c, it demonstrates the usage of ezini functions.

(section, key, value) triples are stored in entry structures (ini_entry_t) and
multiple entry structures may be linked together in an entry list
(ini_entry_list_t).

Read an INI file by calling GetEntryFromFile until it returns 0.

Write an INI file by using AddEntryToList to build an entry list, then call
MakeINIFile to make a file from the entry list.  Call FreeList when you are
done.

## Feedback
Feedback is always welcome!

### In case of problems
For any issue you may encounter please use the Issues option here on GitHub on the top. Please do not try to contact us directly, the RISC OS Community handles all the communications here on github.

### Requesting new features
As for the problems reporting please use the Issues option here on GitHub also to request new features.

### Contributing
We welcome improvements and new ideas, before you submit your changes please have a look at the Contributing Guidelines [here](CONTRIBUTING.md)

## Official ExINI Documentation
See https://michaeldipperstein.github.io/ezini/

## License
The original EzINI is released under GPLv3, so is LibEzINI port here.

## Contributors
[![Michael](https://avatars2.githubusercontent.com/u/30029592?s=42&v=4)](https://github.com/MichaelDipperstein) - The EzINI original author
[![Paolo](https://avatars2.githubusercontent.com/u/8824337?s=42&v=4)](https://github.com/pzaino) - RISC OS Porting
