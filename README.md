mcu-threads
===========
Version: 1.0.0

Small and compact library that implements multitasking
in embedded systems with constrained resources.
This library can run even on chips with less
than 1K of ram!

In order to use mcu-threads your chip needs to support the following:

* at least one hardware timer
* at least 512 bytes of ram (it's possible to run with
        even less but it's not practical).

Supported devices
-----------------
The lib was designed to support different devices;
New devices can be easily added simply by coding against
an interface. Please refer to arch/ directory for a list
of supported devices.

Building
--------
To build invoke:

    make ARCH=<your arch> CPU=[optional cpu variant]

This will produce a static library and a header in `out/`

Usage
-----

For details on using the library, please read `doc/API`

Adding support for other architectures and devices
--------------------------------------------------

Please refer to:
* `doc/ARCH`
* `doc/ARCH_API`

Contact
-------

author: Vladislav Levenetz

email: octal.s@gmail.com

https://github.com/OctalS/mcu-threads.git
